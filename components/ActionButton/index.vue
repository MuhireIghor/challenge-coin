<script setup>
const props = defineProps({
  icon: String,
  text: String,
});
</script>
<template>
  <button
    class="bg-[#f3f3f3] rounded-[6px] flex flex-col items-center aspect-[1] p-1"
  >
    <Icon :name="icon" style="color: #333333" class="text-3xl mx-auto" />

    <p>{{ text }}</p>
  </button>
</template>
