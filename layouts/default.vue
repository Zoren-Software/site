<template>
  <div>
    <nav class="flex flex-wrap items-center justify-between bg-white border-t-2 border-blue-700 border-solid shadow lg:px-12">
      <div class="flex justify-between w-full pb-5 pl-6 pr-2 border-b-2 border-gray-300 border-solid lg:w-auto lg:border-b-0 lg:pb-0">
        <div class="flex items-center flex-shrink-0 mr-16 text-gray-800">
          <img class="w-20 h-30" src="~/assets/img/zoren-software-lith.jpg" alt="Logo Zoren Software">
        </div>
        <div class="block lg:hidden ">
          <button id="nav" class="flex items-center px-3 py-2 text-blue-700 border-2 border-blue-700 rounded hover:text-blue-700 hover:border-blue-700">
            <svg class="w-3 h-3 fill-current" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <title>Menu</title>
              <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/>
            </svg>
          </button>
        </div>
      </div>
      <div class="flex-grow w-full px-8 menu lg:block lg:flex lg:items-center lg:w-auto lg:px-3">
        <div class="font-bold text-blue-700 text-md lg:flex-grow">
          <a href="#responsive-header" class="block btn btn-primary lg:inline-block lg:mt-0 hover:text-white hover:bg-blue-700">
              Home
          </a>
          <a href="#responsive-header" class="block btn btn-primary lg:inline-block lg:mt-0 hover:text-white hover:bg-blue-700">
              Soluções
          </a>
          <a href="#responsive-header" class="block btn btn-primary lg:inline-block lg:mt-0 hover:text-white hover:bg-blue-700">
              Contato
          </a>
        </div>
        <div class="relative hidden mx-auto text-gray-600 lg:block">
          <input class="h-10 pl-2 pr-8 text-sm bg-white border-2 border-gray-300 rounded-lg focus:outline-none" type="search" name="search" placeholder="Search">
          <button type="submit" class="absolute top-0 right-0 mt-3 mr-2">
            <svg class="w-4 h-4 text-gray-600 fill-current" xmlns="http://www.w3.org/2000/svg" version="1.1" id="Capa_1" x="0px" y="0px" viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 56.966 56.966;" xml:space="preserve" width="512px" height="512px">
              <path d="M55.146,51.887L41.588,37.786c3.486-4.144,5.396-9.358,5.396-14.786c0-12.682-10.318-23-23-23s-23,10.318-23,23  s10.318,23,23,23c4.761,0,9.298-1.436,13.177-4.162l13.661,14.208c0.571,0.593,1.339,0.92,2.162,0.92  c0.779,0,1.518-0.297,2.079-0.837C56.255,54.982,56.293,53.08,55.146,51.887z M23.984,6c9.374,0,17,7.626,17,17s-7.626,17-17,17  s-17-7.626-17-17S14.61,6,23.984,6z"/>
            </svg>
          </button>
        </div>
        <div class="flex ">
          <a href="#" class="block px-4 py-2 mt-4 ml-2 font-bold text-blue-700 rounded text-md hover:text-white hover:bg-blue-700 lg:mt-0">Sign in</a>
          <a href="#" class="block px-4 py-2 mt-4 ml-2 font-bold text-blue-700 rounded text-md hover:text-white hover:bg-blue-700 lg:mt-0">login</a>
        </div>
      </div>
    </nav>
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
