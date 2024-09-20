<template>
  <div>
    <b>Họ và tên: {{ fullName }}</b>
  </div>
</template>

<script setup>
import { ref } from "vue";

const user = {
  firstName: "Nguyễn Đình",
  lastName: "Dương",
};

const formatName = (user) => {
  return `${user.firstName} ${user.lastName}`;
};

const fullName = ref(formatName(user));
</script>

<style></style>
