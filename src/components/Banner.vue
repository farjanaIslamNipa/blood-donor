<script setup>

</script>
<template>
    <div class="main-bg h-[600px] w-full">
        <div class="flex flex-col lg:flex-row pt-2 lg:pt-5">
            <div class="flex flex-col pt-4 lg:pt-10 px-4 text-justify pl-32">
                <p class="text-xl lg:text-5xl font-extrabold text-black text-center">LET'S UNITE</p>
                <div class="flex justify-center items-center">
                  <p class="text-[#d01d33] text-xl lg:text-4xl font-extrabold text-center">TO SAVE LIVES</p>
                  <img src="../assets/images/custome/Vector.png" alt="" class="hidden lg:block">
                </div>
                <p class="text-black font-semibold text-lg">We are inviting 18 Core Bangladeshis to Become Life Savers. Join us in this mission.</p>
                <div class="flex flex-col gap-y-4 lg:flex-row gap-x-3 justify-center items-center mt-2">
                  <router-link to="register" class="bg-black text-white rounded-md px-4 py-2">Register As A Doner</router-link>
                  <router-link to="donar" class="bg-[#d01d33] text-white rounded-md px-4 py-2">Find A Blood Doner</router-link>
                </div>
                <p class="text-center text-black font-bold mt-2 text-xl lg:text-4xl">Help Line: 1800-108-1080</p>
            </div>
        </div>
    </div>
  
  
  </template>

  <style scoped>
  .main-bg{
      background-image: url('../assets/images/background/banner-bg.png');
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
  }
  </style>