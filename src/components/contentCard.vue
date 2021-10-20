<template>
  <div>
    <el-card class="box-card">
      <div v-for="o in 4" :key="o" class="text item">
        {{ "列表内容 " + o }}
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
/* 内容卡片 */
.box-card {
  margin-bottom: 30px;
  width: 750px !important;
  height: 300px;
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
</style>