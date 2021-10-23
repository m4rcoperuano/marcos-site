<template>
  <div class="bg-white grid grid-cols-1 lg:grid-cols-4">
    <nav class="sidebar">
      <div class="menu">
        <div class="logo-container">
          <font-awesome-icon
            icon="sun"
            style="font-size:25px;"
          />
          <p class="pl-2 text-xl font-bold">
            Marco L.
          </p>
        </div>

        <div class="links">
          <ul>
            <li>
              <nuxt-link to="/">
                About Me
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/posts">
                Posts
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/contact">
                Contact
              </nuxt-link>
            </li>
            <li>
              Other

              <div>
                <font-awesome-icon
                  :icon="['fab', 'linkedin']"
                />
              </div>
            </li>
          </ul>
        </div>
      </div>
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
  @apply lg:h-screen lg:pt-12 lg:border-r lg:border-b-0
    2xl:pl-32
    col-span-1 px-8 py-8
    border-b bg-gray-100 ;
}

.content {
  @apply md:px-2
  lg:h-screen lg:overflow-scroll lg:col-span-3
  2xl:px-12 2xl:pr-52
  col-span-4 px-0;
}


.logo {
  height:55px;
}

.logo-container {
  @apply flex flex-row items-center mb-3;
}

.links {
  @apply text-gray-600;
}

.links li {
  @apply mb-2;
}

.links li a.nuxt-link-exact-active {
  @apply font-bold text-gray-700;
}
</style>
