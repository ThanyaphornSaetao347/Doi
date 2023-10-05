<template>
  <div class="col" v-for="(n) in travellist" :key="n">
    <div class="name">
      <p>{{ n.name }}</p>
    </div>
    <div class="tipark">
      <RouterLink to="ที่พัก">ที่พัก</RouterLink> /
      <RouterLink to="สถานที่เที่ยว">สถานที่เที่ยว</RouterLink>
    </div>
  </div>
</template>

<script setup>

import { ref } from 'vue';
import { RouterLink } from 'vue-router'
const travellist=ref([
{name: 'ดอยหลวงเชียงดาว',  price:500, img:"https://www.reviewchiangmai.com/wp-content/uploads/2022/06/doi-luang-chiang-dao-1536x1024.jpg", quantity: 0 ,
text_box:'เดินทางโดยสวัสดิภาพ'
}])


</script>

<style>
.name{
  text-align: center;
}
.tipark{
  text-align: center;
}

</style>
