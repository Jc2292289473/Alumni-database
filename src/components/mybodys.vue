<template>
  <div>
    <!-- 背景图 -->
    <img id="beijing1" src="../assets/beijing1.png" />

    <!-- 功能 -->
    <div class="feature">
      <!-- 头像 -->
      <img id="headPortrait" src="../assets/pogw3.jpg" />
      <!-- 创作、关注、收藏、最近浏览 -->
      <!-- 创作中心 -->
      <div class="theTitle">
        <!-- <el-breadcrumb separator="/">
          <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
          <el-breadcrumb-item><a href="/">活动管理</a></el-breadcrumb-item>
          <el-breadcrumb-item>活动列表</el-breadcrumb-item>
          <el-breadcrumb-item>活动详情</el-breadcrumb-item>
        </el-breadcrumb> -->
        <div>
          <div class="quantity">1</div>
          <div class="littleTitle">创作中心</div>
        </div>
        <div class="Delimiter">|</div>
        <div>
          <div class="quantity">6</div>
          <div class="littleTitle">关注</div>
        </div>
        <div class="Delimiter">|</div>
        <div>
          <div class="quantity">18</div>
          <div class="littleTitle">收藏夹</div>
        </div>
        <div class="Delimiter">|</div>
        <div>
          <div class="quantity">107</div>
          <div class="littleTitle">最近浏览</div>
        </div>
        <el-button class="set" type="primary" round>主要按钮</el-button>
      </div>
    </div>
    <!-- 内容 -->
    <div class="mycont">
      <!-- 个人信息 -->
      <div class="info">
        <ul class="myInfo">
          <li id="infoName">测试账号</li>
          <li>2019级:</li>
          <li>工作:</li>
          <li>专业:</li>
          <li>学院:</li>
          <li>城市:</li>
          <li>个人简介:</li>
        </ul>
      </div>
      <!-- 内容区 -->
      <div class="createContent">
        <contentCard v-for="p in 3" :key="p.id" />
      </div>
      <!-- 推荐区 -->
      <div class="recommend">
        <recommendCard/>
      </div>
    </div>
  </div>
</template>

<script>
import contentCard from "./contentCard.vue";
import recommendCard from './recommendCard.vue';

export default {
  name: "mybody.vue",
  components: {
    contentCard,
    recommendCard,
  },
};
</script>


<style scoped>
/* 背景图 */
#beijing1 {
  margin: 0px;
  width: 100%;
  height: 300px;
}
/* 功能区 */
.feature {
  display: flex;
  align-items: center;
  margin: 0px;
  width: 100%;
  height: 80px;
  background: white;
}
/* 功能区头像 */
#headPortrait {
  position: relative;
  left: 90px;
  bottom: 20px;
  width: 170px;
  height: 170px;
}
/* 功能区标题 */
.theTitle {
  display: flex;
  align-items: center;
  position: relative;
  left: 200px;
  font-weight: lighter;
}
/* 数量 */
.quantity {
  display: flex;
  justify-content: center;
  font-size: 25px;
}
/* 三级标题 */
.littleTitle {
  display: flex;
  justify-content: center;
  font-size: 10px;
}
/* 分隔符 */
.Delimiter {
  margin-left: 30px;
  margin-right: 30px;
}
/* 设置按钮 */
.set {
  margin-left: 500px;
}
/* 个人信息 */
.myInfo {
  list-style: none;
}
/* 信息列表 */
.myInfo li {
  font-weight: lighter;
  font-size: 15px;
  margin-bottom: 6px;
}
/* 列表标题 */
#infoName {
  font-weight: 500;
  font-size: 23px;
}
/* infodiv */
.info {
  display: flex;
  padding-left: 10px;
  margin-top: 25px;
  margin-left: 40px;
  width: 270px;
  height: 300px;
}
/* 创作内容 */
.createContent {
  display: flex;
  flex-direction: column;
  padding: 5px;
  margin-top: 30px;
  margin-left: 50px;
  border: rgb(105, 105, 105) 1px solid;
  width: 750px;
  height: auto;
}

/* 内容 */
.mycont {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
}
/* 推荐区 */
.recommend {
  border: rgb(139, 139, 139) 1px solid;
  margin-top: 30px;
  margin-left: 50px;
  width: 250px;
  height: 290px;
}
</style>