<template>
  <nav
    class="flex flex-wrap items-center justify-between mb-3 bg-white border-t-2 border-blue-700 border-solid shadow sm:px-12"
  >
    <div
      class="flex justify-between w-full pb-5 pl-6 pr-2 border-b-2 border-gray-300 border-solid sm:w-auto sm:border-b-0 sm:pb-0"
    >
      <div class="flex items-center flex-shrink-0 mr-10 text-gray-800">
        <img
          class="w-20 mt-4 h-30 sm:mt-0"
          src="~/assets/img/zoren-software-lith.jpg"
          alt="Logo Zoren Software"
        />
      </div>
      <div class="block mt-8 sm:hidden">
        <button
          id="nav"
          class="flex items-center px-3 py-2 text-blue-700 border-2 border-blue-700 rounded hover:text-blue-700 hover:border-blue-700"
          @click="openMenu()"
        >
          <svg
            class="w-3 h-3 fill-current"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <title>Menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
          </svg>
        </button>
      </div>
    </div>
    <div
      :class="`flex-grow w-full menu sm:block sm:items-center sm:w-auto sm:px-3 transition-colors ${styleMenu}`"
    >
      <div class="relative hidden mx-auto text-gray-600 sm:block"></div>
      <div
        class="flex-row-reverse flex-grow w-full px-8 menu sm:block sm:flex sm:items-center sm:w-auto sm:px-3 "
      >
        <NuxtLink
          v-for="(link, index) in links"
          :key="index"
          :to="link.to"
          class="block btn btn-primary sm:inline-block sm:mt-0 hover:text-white hover:bg-blue-700"
        >
          {{ link.title }}
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  props: {
    links: {
      type: Array,
      required: true
    }
  },
  data() {
    return {
      styleMenu: 'hidden'
    }
  },
  methods: {
    openMenu() {
      if(this.styleMenu == 'hidden'){
        this.styleMenu = 'block'
      } else {
        this.styleMenu = 'hidden'
      }
    }
  },
};
</script>
