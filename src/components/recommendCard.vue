<template>
  <div>
      <div class="mayknow">
          <p class="p-may">可能认识的人</p>
          <p>更多</p>
        <!-- <p>gd==</p> -->
      </div>
      <div v-for="p in 5" :key="p.id" class="mayPerson" >

      </div>
  </div>
</template>

<script>
export default {
  name: "recommendCard",
  data() {
    return {

    };
  },
};
</script>

<style scoped>
.mayknow{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 10px;
    /* padding-left: 10px;
        padding-right: 10px; */
    height: 40px;
    background: white;
}
.mayPerson{
    height: 50px;
    background: rgb(241, 177, 177);
}
.p-may{
    display: flex;
    margin: 0px;
}
</style>