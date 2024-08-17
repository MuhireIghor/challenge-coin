<template>
  <div class="w-[10%] bg-black p-2 h-full flex flex-col items-center justify-center  gap-y-4">
    <div class="flex flex-col hover:bg-white hover:border-l-[#2a96fa] w-full hover:cursor-pointer py-2 group border-2 border-transparent">
      <Icon
        name="tabler:template"
        style="color: white"
        class="text-3xl mx-auto group-hover:bg-[#333333]"
      />
      <p class="text-white font-semibold text-sm text-center group-hover:text-[#333333]">Templates</p>
    </div>
    <div class="flex flex-col hover:bg-white hover:border-l-[#2a96fa] w-full hover:cursor-pointer py-2 group border-2 border-transparent">
      <Icon
        name="hugeicons:text"
        style="color: white"
        class="text-3xl mx-auto group-hover:bg-[#333333]"
      />
      <p class="text-white font-semibold text-sm text-center group-hover:text-[#333333]">Add Text</p>
    </div>
    <div class="flex flex-col hover:bg-white hover:border-l-[#2a96fa] w-full hover:cursor-pointer py-2 group border-2 border-transparent">
      <Icon
        name="tabler:photo"
        style="color: white"
        class="text-3xl mx-auto group-hover:bg-[#333333]"
      />
      <p class="text-white font-semibold text-sm text-center group-hover:text-[#333333]">Add Clip Art</p>
    </div>

    <div class="flex flex-col hover:bg-white hover:border-l-[#2a96fa] w-full hover:cursor-pointer py-2 group border-2 border-transparent">
      <Icon
        name="lucide:layers"
        style="color: white"
        class="text-3xl mx-auto group-hover:bg-[#333333]"
      />
      <p class="text-white font-semibold text-sm text-center group-hover:text-[#333333]">Layers</p>
    </div>
    <div class="flex flex-col hover:bg-white hover:border-l-[#2a96fa] w-full hover:cursor-pointer py-2 group border-2 border-transparent">
      <Icon
        name="ion:cloud-upload-outline"
        style="color: white"
        class="text-3xl mx-auto group-hover:bg-[#333333]"
      />
      <p class="text-white font-semibold text-sm text-center group-hover:text-[#333333]">Upload</p>
    </div>
  </div>
</template>
