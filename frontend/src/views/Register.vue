<script setup>
import RegisterHeader from "@/components/RegisterHeader.vue";
import RegisterForm from "@/components/RegisterForm.vue";
import SignInPopup from "@/components/SignInPopup.vue";

import {useTemplateRef} from "vue";

const popup = useTemplateRef('sign-up-popup');
function openSignUpPopup(){
  popup.value.open();
}
</script>

<template>
  <RegisterHeader/>
  <main>
    <SignInPopup ref="sign-up-popup"/>
    <RegisterForm @open-popup="openSignUpPopup"/>
  </main>
</template>

<style scoped lang="scss">
main{
  display: grid;
  place-items: center;
  height: calc(100vh - 80px);
}
</style>