<script setup>
const props = defineProps({
  text: String,
  toogle: Boolean,
});
</script>
<template>
  <div
    :class="
      toogle
        ? 'bg-white flex flex-col w-[60px] h-[72px] hover:cursor-pointer'
        : 'bg-[#cccccc] text-[#a3a3a3] flex flex-col'
    "
  >
    <div
      class="w-[80%] h-[70%] mx-auto bg-[#d8d8d8] border border-b-[#2a96fa] flex justify-center items-center"
    >
      <img class="w-6 h-6" src="~/assets/images/circle.png" alt="circle" />
    </div>
    <p
      :class="
        toogle ? 'text-center text-[#333333]' : 'text-center text-[#999999]'
      "
    >{{ text }}</p>
  </div>
</template>
