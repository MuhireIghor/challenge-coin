<script setup>
const tools = ref([
  {
    icon: "ion:cloud-upload-outline",
    text: "Upload",
  },
  {
    icon: "tabler:template",
    text: "Templates",
  },
  {
    icon: "hugeicons:text",
    text: "Add Text",
  },
  {
    icon: "tabler:photo",
    text: "Add Clip Art",
  },
]);
</script>
<template>
  <div class="w-full flex  h-[80%]">
    <!-- tools section -->
    <div class="w-1/3 flex flex-col py-12 gap-y-2 px-8">
      <p class="text-center text-md font-semibold text-xl">What's next</p>
      <div class="grid grid-cols-2 gap-4">
        <ToolBox
          v-for="(tool, index) in tools"
          v-bind:key="index"
          v-bind="tool"
        />
      </div>
    </div>
    <div class="w-2/3">
      <View />

    </div>
  </div>
</template>
