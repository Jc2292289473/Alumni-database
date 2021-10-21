<template>
  <div class="recommends">
    <div class="mayknow">
      <p class="p-may">可能认识的人</p>
      <p class="p-more">更多+</p>
      <!-- <p>gd==</p> -->
    </div>
    <div v-for="p in 4" :key="p.id" class="mayPerson">
      <div class="recommendImage">
        <img src="../assets/pogw3.jpg" />
      </div>
      <div class="recommendInfo">
        <p class="recommendName">测试信息</p>
        <p class="recommendIntroduce">来自:2019级软件工程</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "recommendCard",
  data() {
    return {};
  },
};
</script>

<style scoped>
/* 推荐 */
.recommends {
  border: rgb(139, 139, 139) 1px solid;
  width: 250px;
  height: 280px;
}

.mayknow {
  display: flex;
  align-items: center;
  justify-content: space-between;
  /* 两个是上下和左右 */
  padding: 0 10px;
  height: 40px;
  background: white;
}
.mayPerson {
  display: flex;
  padding-left: 10px;
  height: 60px;
  background: white;
}
.p-may {
  display: flex;
  margin: 0px;
  font-size: 14px;
}
.p-more {
  font-size: 14px;
}
/* 推荐头像 */
.recommendImage {
  width: 30%;
}
.recommendImage > img {
  border-radius: 50%;
  width: 50px;
  height: 50px;
}
/* 推荐信息 */
.recommendInfo {
  display: flex;
  flex-direction: column;
  width: 70%;
}
.recommendInfo > p {
  margin: 0px;
}
.recommendName {
  margin-top: 2px !important;
  font-size: 15px;
}
.recommendIntroduce {
  margin-top: 7px !important;
  font-size: 12px;
  font-weight: lighter;
}
</style>