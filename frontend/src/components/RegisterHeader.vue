<template>
  <header class="register-header">
    <div class="logo-container">
      <img class="logo-img" src="@/../public/logo.png" alt="">
      <h1 class="logo-title">Lotos</h1>
    </div>
  </header>
</template>

<style scoped lang="scss">
@import "@/assets/base";

.register-header{
  height: 80px;
  display: flex;
  justify-content: center;
  border-bottom: 1px solid $separator-grey;
}

.logo-container{
  height: 100%;
  gap: 18px;
  display: flex;
  align-items: center;

  .logo-img{
    height: 80%;
  }

  .logo-title{
    font-family: Gilroy;
    font-weight: bold;
    color: $text-violet;
    font-size: 42px;
    padding-top: 8px;
    line-height: 42px;
  }
}
</style>
<script setup lang="ts">
</script>