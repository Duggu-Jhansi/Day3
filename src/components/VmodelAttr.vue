<script setup>
import { ref } from 'vue'

const message = ref('')
const password=ref('')
const selected=ref('')
</script>

<template>
    <div>
    <div class="bg">
     <h1>About Form</h1>
	<input  v-model="message"  type="text" placeholder="enter your name" class="input1" />
    <br/>
    <textarea v-model="password"  type="text" placeholder="write about You" class="input2"></textarea>
    <br/>

<div>
<p>{{ message }}</p>
<p>{{ password }}</p>
</div>
</div>
<div>
    <h1>Quiz</h1>
    <span>Who is founder of Vue: {{ selected }}</span>

<select v-model="selected">
 
  <option>Evan You</option>
  <option>Guido van Rossum</option>
  <option>Jordan Walke</option>
</select>

</div>
</div>
</template>
<style>
.input1{
    margin:2px;
}
.input2{
    margin:4px
}
.bg{
    background-image: linear-gradient(#2E3192, #1BFFFF);
    width:50%;
    text-align: center;
    margin:0 auto;
}
h1{
    color:white;
}
</style>