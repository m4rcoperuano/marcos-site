<template>
  <div class="bg-white grid grid-cols-4">
    <nav class="sidebar">
      <h5 class="brand text-lg font-bold text-gray-500">
        Marco Ledesma.site
      </h5>
    </nav>
    <div class="content">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {
  head: {
    bodyAttrs: {
      class: "bg-white",
    },
  },
};
</script>

<style scoped>
.sidebar {
  @apply hidden lg:block bg-gray-100 h-screen col-span-1 pl-8 2xl:pl-32 pt-12;
}

.content {
  @apply h-screen overflow-scroll col-span-4 lg:col-span-3 px-0 md:px-2 2xl:px-12 2xl:pr-52;
}
</style>
