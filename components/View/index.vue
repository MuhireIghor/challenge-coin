<script setup>
const icons = ref([
  {
    icon: "eva:undo-fill",
    text: "Undo",
  },
  {
    icon: "ion:arrow-redo",
    text: "Redo",
  },
  {
    icon: "hugeicons:text",
    text: "Text",
  },
  {
    icon: "ion:cloud-upload-outline",
    text: "Upload",
  },
  {
    icon: "bx:save",
    text: "Save",
  },
]);

const count = ref(0);
function handleIncrease() {
  count.value += 1;
}

function handleDecrease() {
  if (count.value > 0) count.value -= 1;
}
</script>
<template>
  <div
    class="bg-[#e6e6e6] h-[calc(100vh-140px)] w-full pt-3 flex flex-col overflow-y-scroll"
  >
    <div class="flex justify-center w-full gap-x-8">
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="ph:copy"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Copy"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="line-md:arrow-align-center"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Center"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="solar:flip-vertical-bold"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Flip"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="ci:layer"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Layer"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="pixelarticons:grid"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Grid"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="icon-park-twotone:group"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Group"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="mdi:draw-pen"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Pen"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="ant-design:clear-outlined"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Clear"
        />
      </div>
      <div
        class="hover:bg-white p-[3px] rounded flex items-center justify-center"
      >
        <Icon
          name="pepicons-pop:keyboard"
          style="color: black"
          class="text-3xl hover:cursor-pointer"
          title="Shortcut Key "
        />
      </div>
    </div>
    <div class="w-full flex pt-1 p-8">
      <div class="flex flex-col gap-y-2 w-[30%]">
        <p class="text-[#333333] font-semibold">
          Custom Blank Smooth Edge Coin
        </p>
        <div class="flex flex-col gap-y-1">
          <ViewSelectors toogle="true" text="Front" />
          <ViewSelectors toogle="false" text="Back" />
        </div>
      </div>
      <div class="w-[68%] flex flex-col justify-center-center">
        <img
          src="~/assets/images/canva.png"
          alt="canva"
          width="230"
          height="40"
        />
        <div class="w-full flex justify-end pt-12 pr-12">
          <div
            class="bg-[#f3f3f3] flex gap-x-6 rounded p-2 px-4 text-[#a3a3a3] text-lg"
          >
            <button @click="handleDecrease">-</button>
            <span>{{ count }}%</span>
            <span>Fit</span>
            <button @click="handleIncrease">+</button>
          </div>
        </div>
      </div>
      <div class="flex flex-col gap-y-1 relative">
        <ActionButton
          v-for="(icon, index) in icons"
          v-bind:key="index"
          v-bind="icon"
        />
        <div class="fixed bottom-16">
          <a href="#">
            <img alt="email us" src="~/assets/images/email.png" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
