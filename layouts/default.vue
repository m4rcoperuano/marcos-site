<template>
  <div class="max-w-2xl mx-auto px-4">
    <nav>
      <div class="left pt-3">
        <h2 class="brand text-4xl font-bold text-black pt-3 mb-3">
          Hey! I'm Marco Ledesma :)
        </h2>
        <div class="links mb-4">
          <ul class="flex flex-row">
            <li>
              <a href="#" class="p-2 mr-2 bg-green-100 text-green-800 rounded"
                >Me</a
              >
            </li>
            <li>
              <a href="#" class="p-2 mr-2 text-gray-600">Projects</a>
            </li>
            <li>
              <a href="#" class="p-2 text-gray-600"> Links and such </a>
            </li>
          </ul>
        </div>
      </div>
      <div class="right"></div>
    </nav>
    <div class="container mx-auto">
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