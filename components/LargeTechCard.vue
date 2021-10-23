<template>
  <div
    class="tech-card"
  >
    <div class="right">
      <div class="flex items-center mb-1">
        <div class="w-10">
          <img
            :alt="titleClassName + ' logo'"
            :src="imageSrc"
          >
        </div>
        <h4
          class="tech__title"
          :class="titleClassName"
        >
          {{ title }}
        </h4>
      </div>
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    titleClassName: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    imageSrc: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.tech-card {
  @apply flex flex-col p-4 rounded-lg md:flex-row rounded shadow-lg;
}

.tech-card .left {
  width: 100%;
  flex: 1;
  @apply p-6 flex;
}

.tech-card .left img {
  @apply max-h-40 md:max-h-full;
}

.tech-card .right {
  @apply p-2 flex flex-col;
  flex: 3;
}

.tech-card .tech__title {
  @apply text-2xl mb-2 mt-2 font-extrabold ml-2;
}
</style>
