<template>
  <div
    class="tech-card"
  >
    <div class="left">
      <img
        :alt="titleClassName + ' logo'"
        :src="imageSrc"
      >
    </div>
    <div class="right">
      <h4
        class="tech__title"
        :class="titleClassName"
      >
        {{ title }}
      </h4>
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
    backgroundClassName: {
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
  @apply flex flex-row p-2 rounded-lg border;
}

.tech-card .left {
  width:50px;
  @apply p-2 flex;
}

.tech-card .left img {
  max-height:45px;
}

.tech-card .right {
  @apply p-2 flex flex-col justify-center;
  flex: 3;
}

.tech-card .tech__title {
  @apply text-xl font-bold;
}
</style>
