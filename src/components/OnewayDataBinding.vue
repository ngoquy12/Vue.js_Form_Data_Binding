<template>
  <div>
    <h1>Oneway data binding</h1>
    <h3>Username: {{ userName }}</h3>
    <input type="text" :value="userName" />
    <button @click="handleChangeName">Change Name</button>
  </div>
</template>

<script setup>
import { ref } from "vue";

const userName = ref("Nguyễn Văn B");

const handleChangeName = () => {
  userName.value = "Nguyễn Văn A";
};
</script>

<style></style>
