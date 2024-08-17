<template>
  <div class="flex flex-col h-screen bg-[#f0f0f0]">
    <Navbar />
    <div class="w-full flex flex-grow h-[85%]">
      <Sidebar />
      <div class="flex flex-col w-full gap-y-12">
        <Preview />
        <Locator />
      </div>
    </div>
  </div>
</template>
