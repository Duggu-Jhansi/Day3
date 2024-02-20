<template>
  <div class="contanier">
    <h1 class="head">Counter</h1>
  <button @click.prevent="decreaseCount">-
  </button>
  <span class="num">{{ count }}</span>
  <button @click.prevent="increaseCount">+
  </button>
  </div>
</template>
<script setup>
import {ref} from 'vue';
const count=ref(0);

function increaseCount(){
  count.value++
}
function decreaseCount(){
  count.value--
}
</script>
<style>
.container{
  text-align: center;
}
.num{
  margin:5px;
  color:black;

}
.head{
  color:black
}
</style>
