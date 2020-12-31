<template>
  <div>
    <h1 class="px-10 mt-4 mb-5 font-sans text-2xl font-bold sm:my-10 md:pt-20 sm:text-4xl md:text-3xl lg:text-5xl">{{title}}</h1>
    <!-- description -->
    <div
      class="w-full px-10 pb-10 text-gray-500 sm:pb-5 md:text-2xl sm:text-2xl text-md description sm: md:w-2/3"
    >
      {{text}}
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      required: true,
      type: String
    },
    text: {
      required: true,
      type: String
    }
  }
}
</script>
