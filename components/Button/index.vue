<script setup>
const props = defineProps({
  text: String,
});
</script>
<template>
  <button
    class="bg-[#0a9a35] rounded-[6px] text-white hover:cursor-pointer font-bold leading-[48px] text-center w-[180px] h-[48px]"
  >
    {{ text }}
  </button>
</template>
