<template>
  <div class="p-8 pt-12 text-gray-900 pb-8">
    <h1 class="text-4xl font-bold mb-2">
      About me
    </h1>
    <div class="intro mb-8">
      <p>
        Hello World! This site is primarily built to satisfy my more creative
        side. I like to code, but not always on "work" things. So the goal is to
        use this site to play with new technologies, blog, and just have fun.
      </p>
    </div>
    <div class="tech-stuff mb-8">
      <h4 class="text-2xl mb-4 text-gray-800">
        Favorite Technologies
      </h4>
      <div class="grid lg:grid-cols-2 gap-4 mb-4">
        <large-tech-card
          title="Laravel"
          background-class-name="border-red-100"
          title-class-name="text-red-600"
          :image-src="require('~/assets/images/laravel-400-logo.png')"
        >
          <p>
            Probably my favorite fullstack framework for the last 7 or 8 years.
            If you have a hobby project or a start up, I cannot recommend
            Laravel enough. The community is fantastic, the code is clean and
            elegant, and it'll teach ya concepts that you can bring to other
            environments. The docs are event a joy to read, which is rare to
            find.
          </p>
        </large-tech-card>

        <large-tech-card
          title="Vue"
          background-class-name="border-green-100"
          title-class-name="text-green-600"
          :image-src="require('~/assets/images/vue-400-logo.png')"
        >
          <p>
            Vue feels like a natural extension of the web. You can use the same
            old HTML and CSS that you're familiar with, sprinkle in some
            javascript, and you got a reactive application. Initially, I was not
            sold on single page applications. They seemed unnecessary when you
            have good-old server rendered pages. But I've learned to love it
            over time, and now prefer SPA's over traditional server-rendered
            pages any day. All that was thanks to Vue.
          </p>
        </large-tech-card>
        <large-tech-card
          :image-src="require('~/assets/images/dot-net-300-logo.png')"
          title=".NET Core (C#)"
          background-class-name="border-purple-100"
          title-class-name="text-purple-600"
        >
          <p>
            One of my earliest experiences programming was using the .NET framework for web
            applications. Over the years, I've worked with .NET's MVC 3, 4, 5, and now .NET Core.
            I find it a really elegantly designed framework with an intuitive language (C#).
          </p>
        </large-tech-card>
      </div>
    </div>

    <div>
      <h4 class="text-2xl mb-4 text-gray-800">
        Honorable Mentions
      </h4>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <small-tech-card
          :image-src="require('~/assets/images/forge-400-logo.png')"
          title="Forge"
          background-class-name="bg-gray-100"
          title-class-name="text-gray-600"
        />
        <small-tech-card
          :image-src="require('~/assets/images/tailwind-400-logo.png')"
          title="Tailwind CSS"
          background-class-name="bg-blue-100"
          title-class-name="text-blue-600"
        />
        <small-tech-card
          :image-src="require('~/assets/images/sql-400-logo.png')"
          title="SQL"
          background-class-name="bg-yellow-100"
          title-class-name="text-yellow-600"
        />
        <small-tech-card
          :image-src="require('~/assets/images/swift-400-logo.png')"
          title="Swift"
          background-class-name="bg-red-100"
          title-class-name="text-red-600"
        />
        <small-tech-card
          :image-src="require('~/assets/images/storybook-300-logo.png')"
          title="Storybook"
          background-class-name="bg-pink-100"
          title-class-name="text-pink-600"
        />
        <small-tech-card
          :image-src="require('~/assets/images/react-400-logo.png')"
          title="React Native"
          background-class-name="bg-blue-100"
          title-class-name="text-blue-400"
        />
      </div>
    </div>
  </div>
</template>

<script>
import LargeTechCard from "../components/LargeTechCard";
import SmallTechCard from "~/components/SmallTechCard";

export default {
  components: {
    LargeTechCard,
    SmallTechCard
  }
};
</script>

<style scoped>
.large-tech-card {
  @apply flex p-2 rounded-lg mb-6;
}

.large-tech-card .left {
  width: 100%;
  flex: 1;
  @apply p-6 justify-center items-center flex;
}

.large-tech-card .right {
  @apply p-2;
  flex: 3;
}

.large-tech-card .tech__title {
  @apply text-2xl mb-2 mt-2 font-extrabold;
}
</style>
