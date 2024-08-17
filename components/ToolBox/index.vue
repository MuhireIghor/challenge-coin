<script setup>
const props = defineProps({
  icon: String,
  text: String,
});
</script>
<template>
  <div
    class="bg-[#f4f4f4] group rounded-[10px] hover:cursor-pointer flex flex-col items-center justify-center aspect-[180/120] transition-all duration-300 font-[14px]"
  >
    <Icon :name="icon" style="color: #333333" class="text-3xl mx-auto group-hover:bg-[#2a96fa]" />
    <p class="text-center text-[#333333] font-light group-hover:text-[#2a96fa]">{{ text }}</p>
  </div>
</template>
