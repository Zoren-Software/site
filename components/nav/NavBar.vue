<template>
  <nav
    class="flex flex-wrap items-center justify-between bg-white border-t-2 border-blue-700 border-solid shadow lg:px-12"
  >
    <div
      class="flex justify-between w-full pb-5 pl-6 pr-2 border-b-2 border-gray-300 border-solid lg:w-auto lg:border-b-0 lg:pb-0"
    >
      <div class="flex items-center flex-shrink-0 mr-16 text-gray-800">
        <img
          class="w-20 h-30"
          src="~/assets/img/zoren-software-lith.jpg"
          alt="Logo Zoren Software"
        />
      </div>
      <div class="block lg:hidden ">
        <button
          id="nav"
          class="flex items-center px-3 py-2 text-blue-700 border-2 border-blue-700 rounded hover:text-blue-700 hover:border-blue-700"
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
      class="flex-grow w-full menu lg:block lg:flex lg:items-center lg:w-auto lg:px-3"
    >
      <div class="relative hidden mx-auto text-gray-600 lg:block"></div>
      <div
        class="flex-row-reverse flex-grow w-full px-8 menu lg:block lg:flex lg:items-center lg:w-auto lg:px-3 "
      >
        <a v-for="(link, index) in links" :key="index"
          :to="link.to"
          class="block btn btn-primary lg:inline-block lg:mt-0 hover:text-white hover:bg-blue-700"
        >
          {{link.title}}
        </a>
        <a
          href="#responsive-header"
          class="block btn btn-primary lg:inline-block lg:mt-0 hover:text-white hover:bg-blue-700"
        >
          Soluções
        </a>
        <a
          href="#responsive-header"
          class="block btn btn-primary lg:inline-block lg:mt-0 hover:text-white hover:bg-blue-700"
        >
          Home
        </a>
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
  }
}
</script>
