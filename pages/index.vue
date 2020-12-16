<template>
  <div class="container mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-2">
      <div>
        <h1 class="px-10 mt-4 mb-5 font-sans text-2xl font-bold sm:my-10 md:pt-20 sm:text-4xl md:text-3xl lg:text-5xl">Desenvolvimento de Software</h1>
        <!-- description -->
        <div
          class="w-full px-10 pb-10 text-gray-500 sm:pb-5 md:text-2xl sm:text-2xl text-md description sm: md:w-2/3"
        >
          Nós ajudamos você a gerenciar e criar o software que contribuirá com o sucesso da sua empresa. Somos profissionais altamente qualificados focados em entregar o melhor software para sua empresa.
        </div>
      </div>
      <div>
        <div class="flex flex-col justify-center pb-6 sm:py-12">
          <div class="relative py-3 sm:max-w-xl sm:mx-auto md:mr-6">
            <div class="absolute inset-0 transform -skew-y-6 shadow-lg bg-gradient-to-r from-blue-400 to-blue-800 sm:skew-y-0 sm:-rotate-6 sm:rounded-3xl"></div>
            <div class="relative px-4 py-10 bg-white shadow-lg sm:rounded-3xl sm:p-20 md:px-8 md:pb-12 md:pt-5">
              <div class="max-w-md mx-auto">
                <div class="divide-y divide-gray-200">
                  <div class="py-8 space-y-4 text-base leading-6 text-gray-700 sm:text-lg sm:leading-7">
                    <p class="px-7">Criamos o software para atender com as suas aspectativas:</p>
                    <ul class="space-y-2 list-disc">
                      <li class="flex items-start">
                        <span class="flex items-center h-6 sm:h-7">
                          <svg class="flex-shrink-0 w-5 h-5 text-blue-500" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                          </svg>
                        </span>
                        <p class="ml-2">
                          Layout personalizado, criando com um forte estudo de
                          <code class="text-sm font-bold text-gray-900">design gráfico</code>.
                        </p>
                      </li>
                      <li class="flex items-start">
                        <span class="flex items-center h-6 sm:h-7">
                          <svg class="flex-shrink-0 w-5 h-5 text-blue-500" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                          </svg>
                        </span>
                        <p class="ml-2">
                          É feita toda uma <code class="text-sm font-bold text-gray-900">documentação</code> de funcionamento do seu projeto.
                        </p>
                      </li>
                      <li class="flex items-start">
                        <span class="flex items-center h-6 sm:h-7">
                          <svg class="flex-shrink-0 w-5 h-5 text-blue-500" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                          </svg>
                        </span>
                        <p class="ml-2">Temos nosso próprio sistema para acompanhamento do andamento do projeto e das entregas a serem feitas para nosso cliente.</p>
                      </li>
                    </ul>
                    <p class="px-7">Estamos sempre em constante contato para entregarmos o melhor sistema, para garantir o sucesso do nosso cliente.</p>
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
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>


