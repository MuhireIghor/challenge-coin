<template>
  <div class="w-full bg-black p-3 flex justify-between">
    <section class="flex items-center gap-x-8">
      <Logo />
      <Icon
        name="heroicons:bars-4-solid"
        style="color: white"
        class="text-4xl"
      />

      <div class="flex items-center gap-x-1">
        <Icon
          name="line-md:email-opened"
          style="color: white"
          class="text-4xl"
        />
        <div class="flex flex-col text-white text-sm -leading-1">
          <span>1-866-573-4920</span>
          <span>info@gs-jj.com</span>
        </div>
      </div>
      <div class="flex items-center gap-x-1">
        <Icon
          name="fluent-mdl2:telemarketer"
          style="color: white"
          class="text-4xl"
        />
        <div class="flex flex-col text-white text-sm -leading-1">
          <span>Talk to A Real Person</span>
          <span>909-468-4808</span>
        </div>
      </div>
    </section>
    <section>
      <div class="flex items-center gap-x-1">
        <Icon name="iconamoon:profile" style="color: white" class="text-4xl" />
        <p class="text-white ">Log In/Join Free</p>
      </div>
    </section>
  </div>
</template>
