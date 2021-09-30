<template>
  <div>
    <div class="intro mb-3">
      <p>
        Hello World! This site is primarily built to satisfy my more creative
        side. I like to code, but not always on work things. So the goal is to
        use this site to play with new technologies, blog, and just have fun.
      </p>
    </div>
    <hr class="mb-8 mt-8" />

    <div class="techstuff">
      <h1 class="text-xl font-bold mb-4">Technologies I Love</h1>
      <div class="tech-card bg-red-50">
        <div class="left">
          <img src="~/assets/images/laravel-400-logo.png" />
        </div>
        <div class="right">
          <h4 class="tech__title text-red-600">Laravel</h4>
          <p>
            Probably my favorite fullstack framework for the last 7 or 8 years.
            If you have a hobby project or a start up, I cannot recommend
            Laravel enough. The community is fantastic, the code is clean and
            elegant, and it'll teach ya concepts that you can bring to other
            environments. The docs are event a joy to read, which is rare to
            find.
          </p>
        </div>
      </div>

      <div class="tech-card bg-green-50">
        <div class="left">
          <img src="~/assets/images/vue-400-logo.png" />
        </div>
        <div class="right">
          <h4 class="tech__title text-green-600">Vue</h4>
          <p>
            Vue feels like a natural extension of the web. You can use the same
            old HTML and CSS that you're familiar with, sprinkle in some
            javascript, and you got a reactive application. Initially, I was not
            sold on single page applications. They seemed unnecessary when you
            have good-old server rendered pages. But I've learned to love it
            over time, and now prefer SPA's over traditional server-rendered
            pages any day. All that was thanks to Vue.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tech-card {
  @apply flex p-2 rounded-lg mb-6;
}

.tech-card .left {
  width: 100%;
  flex: 1;
  @apply p-6;
}

.tech-card .right {
  @apply p-2;
  flex: 3;
}

.tech-card .tech__title {
  @apply text-xl mb-2 mt-2 font-extrabold;
}
</style>
