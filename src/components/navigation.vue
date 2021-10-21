<template>
  <div class="navigation">
    <div class="logo">
      <!-- logo -->
      <img id="img_logo" src="../assets/headicon.png" />
      <!-- 搜索框 -->
      <el-input
        prefix-icon="el-icon-zoom-in"
        v-model="input"
        placeholder="请输入内容"
      ></el-input>
      <!-- 头像 -->
      <div class="headPortrait">
        <img src="../assets/pogw3.jpg" />
      </div>
      <!-- 发布按钮 -->
      <div class="btn">
        <el-button type="primary" icon="el-icon-search">搜索</el-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: "",
    };
  },
};
</script>

<style scoped>
.navigation {
  display: flex;
  flex-direction: column;
}

/* 头部div */
.logo {
  display: flex;
  height: 60px;
}
/* logo图片 */
#img_logo {
  width: 300px;
  height: 60px;
}
/* 搜索框 */
.el-input {
  /* el-input是一个div 包裹着input   align-items: center;对里边类容进行垂直居中 */
  display: flex;
  margin-left: 42%;
  width: 300px;
  height: 60px;
  align-items: center;
}
/* 头像 */
.headPortrait {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: 30px;
  width: 60px;
  height: 60px;
}
.headPortrait img {
  width: 40px;
  height: 40px;
}
/* 搜索俺就 */
.btn {
  display: flex;
  margin-left: 30px;
  height: 60px;
  align-items: center;
}
</style>