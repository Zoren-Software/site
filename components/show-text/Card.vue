<template>
  <div class="flex flex-col justify-center pb-6 sm:py-12">
    <div class="relative py-3 sm:max-w-xl sm:mx-auto md:mr-6">
      <div class="absolute inset-0 transform -skew-y-6 shadow-lg bg-gradient-to-r from-blue-400 to-blue-800 sm:skew-y-0 sm:-rotate-6 sm:rounded-3xl"></div>
      <div class="relative px-4 py-10 bg-white shadow-lg sm:rounded-3xl sm:p-20 md:px-8 md:pb-12 md:pt-5">
        <div class="max-w-md mx-auto">
          <div class="divide-y divide-gray-200">
            <div class="py-8 space-y-4 text-base leading-6 text-gray-700 sm:text-lg sm:leading-7">
              <p class="text-lg sm:text-2xl md:text-2xl px-7">{{title}}</p>
              <ul class="space-y-2 list-disc">
                <li v-for="(textCard, index) in textCardOptions" :key="index" class="flex items-start">
                  <span class="flex items-center h-6 sm:h-7">
                    <svg class="flex-shrink-0 w-5 h-5 text-blue-500" viewBox="0 0 20 20" fill="currentColor">
                      <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                    </svg>
                  </span>
                  <p class="ml-2">
                    {{textCard.text}}
                  </p>
                </li>
              </ul>
              <p class="px-7">{{subtitle}}</p>
            </div>
            <div class="pt-6 text-base font-bold leading-6 sm:text-lg sm:leading-7">
              <p>Conheça nossas soluções</p>
              <p>
                <nuxt-link to="/solucoes" class="text-blue-600 hover:text-blue-700"> Soluções &rarr; </nuxt-link>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    textCardOptions:{
      required:true,
      type: Array
    },
    title:{
      required:true,
      type: String
    },
    subtitle:{
      required:true,
      type: String
    }
  }
}
</script>
