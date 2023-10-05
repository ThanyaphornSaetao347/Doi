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

const travellist=ref([
{name: 'ดอยค้ำฟ้า', img:"https://www.reviewchiangmai.com/wp-content/uploads/2022/06/doi-kamfha-1536x1024.jpg", quantity: 0 ,
text_box:'เดินทางโดยสวัสดิภาพ'
}])


</script>

<style>

.card-img-top{
height: 100%;
padding: 25px;

}
.box_all{
justify-content: center;
align-items: center;
margin-left: 30%;
text-align: center
}

</style>
