<template>
  <div class="createContents">
    <el-card class="box-card">
      <!-- <div v-for="o in 4" :key="o" class="text item">
        {{ "列表内容 " + o }}
      </div> -->
      <!-- cardInfo -->
      <div class="cardInfo">
        <!-- 头像 -->
        <div class="cardImage">
          <img src="../assets/pogw3.jpg" alt="" />
        </div>
        <div class="cardinfoFirst">
          <div class="firstOne">
            <!-- 名称 -->
            <div class="cardName">测试名称</div>
            <div class="cardTime">刚刚</div>
          </div>
          <button class="carDel">X</button>
        </div>
      </div>
      <div class="cardContent">
        <!-- <textarea name="" id="" cols="30" rows="10">
          测试数据测
          试数据测试数
          据测试数据测试数据测试数据测试数据
          测试数据测试数据测试数据测试数据
          测试数据测试数据测试数据测试数据
          测试数据测试数据
        </textarea> -->
        <p>
          测试数据测 试数据测试数 据测试数据测试数据测试数据测试数据
          测试数据测试数据测试数据测试数据 测试数据测试数据测试数据测试数据
          测试数据测试数据
        </p>
      </div>
    </el-card>
  </div>
</template>

<script>
export default {
  name: "contentCard",
  data() {
    return {};
  },
};
</script>

<style scoped>
.createContents {
  display: flex;
  flex-direction: column;
  padding: 5px;
  width: 750px;
  height: auto;
}
/* 内容卡片整体 */
.box-card {
  margin-bottom: 30px;
  width: 750px !important;
  height: auto;
}
.text {
  font-size: 14px;
}
.item {
  padding: 18px 0;
}
.box-card {
  width: 480px;
}
/* 卡片内容 */
/* 头像 */
.cardInfo {
  display: flex;
  height: 50px;
}
.cardImage {
  display: flex;
  /* 垂直居中 */
  align-items: center;
  /* 水平居中 */
  justify-content: center;
  width: 50px;
}
.cardImage > img {
  width: 45px;
  height: 45px;
}
/* 用户信息 */
.cardinfoFirst {
  display: flex;
  justify-content: space-between;
  width: 95%;
  height: 50px;
  /* margin-left: 30px; */
  margin-left: 2%;
}
/* 名称时间 */
.firstOne {
  display: flex;
  flex-direction: column;
}
.cardName {
  display: flex;
  width: 150px;
  height: 30px;
}
.cardTime {
  display: flex;
  width: 150px;
  height: 20px;
  font-size: 11px;
  font-weight: lighter;
}
/* 内容 */
.cardContent {
  height: auto;
  margin-left: 65px;
  min-height: 80px;
}
.cardContent > p {
  margin: 0px;
}
.carDel{
  border-radius: 30%;
  width: 40px;
  height: 30px;
}
</style>