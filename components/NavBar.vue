<template>
  <nav class="relative z-50 h-24 select-none">
    <div class="container relative flex flex-wrap items-center justify-between h-24 mx-auto overflow-hidden font-medium border-b border-gray-200 md:overflow-visible lg:justify-center px-4 md:px-2">
      <div class="flex items-center justify-start w-1/4 h-full pr-4">
        <a class="inline-block py-4 md:py-0">
          <NuxtLink to="/">
            <img src="/catto3.png" class=" md:inline w-10 inline align-middle" alt="">
            <span class="align-middle p-1 text-2xl font-black leading-none text-gray-900"><span class="text-white">catto</span><span class="text-primary-catto">css</span></span>
          </NuxtLink>
        </a>
      </div>
      <div class="top-0 left-0 items-start hidden w-full h-full p-4 text-sm bg-gray-900 bg-opacity-50 md:items-center md:w-3/4 md:absolute lg:text-base md:bg-transparent md:p-0 md:relative md:flex">
        <div class="flex-col w-full h-auto overflow-hidden bg-white rounded-lg md:bg-transparent md:overflow-visible md:rounded-none md:relative md:flex md:flex-row">
          <a class="inline-flex items-center w-auto h-16 px-6 text-xl font-black leading-none text-gray-900 md:hidden">tails<span class="text-primary-catto">.</span></a>
          <div class="flex flex-col items-start justify-center w-full space-x-6 text-center lg:space-x-8 md:w-2/3 md:mt-0 md:flex-row md:items-center">
            <!-- <NuxtLink class="inline-block w-full py-2 mx-0 ml-6 font-medium text-left text-primary-catto md:ml-0 md:w-auto md:px-0 md:mx-2 lg:mx-3 md:text-center" to="/">
              Animations
            </NuxtLink> -->
            <!-- <NuxtLink to="/animations">
              <a class="inline-block w-full py-2 mx-0 font-medium text-left md:w-auto md:px-0 md:mx-2 hover:text-primary-catto lg:mx-3 md:text-center text-white">Animations</a>
            </NuxtLink> -->
            <!-- <NuxtLink to="/about">
              <a class="inline-block w-full py-2 mx-0 font-medium text-left md:w-auto md:px-0 md:mx-2 hover:text-primary-catto lg:mx-3 md:text-center text-white">About</a>
            </NuxtLink> -->
            <!-- <a class="inline-block w-full py-2 mx-0 font-medium text-left md:w-auto md:px-0 md:mx-2 hover:text-primary-catto lg:mx-3 md:text-center text-white">Contribute</a> -->
            <!-- <a class="absolute top-0 left-0 hidden py-2 mt-6 ml-10 mr-2 lg:inline-block md:mt-0 md:ml-2 lg:mx-3 md:relative text-white">
              <svg
                class="inline w-5 h-5"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                viewBox="0 0 24 24"
                stroke="currentColor"
              ><path d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" /></svg>
            </a> -->
          </div>
          <div class="flex flex-col items-start justify-end w-full pt-4 md:items-center md:w-1/3 md:flex-row md:py-0">
            <NuxtLink to="/avalojandro">
              <a href="#" class="w-full px-6 py-2 mr-0 md:px-0 lg:pl-2 md:mr-4 lg:mr-5 md:w-auto text-white">Avalojandro?</a>
            </NuxtLink>
            <a href="https://ko-fi.com/avalojandro" target="_blank" class="">
              <img class="w-40 rounded-3xl" src="/coffee.png" alt="">
            </a>
          </div>
        </div>
      </div>
      <div class="absolute right-0 mr-4 flex flex-col items-center items-end justify-center w-10 h-10 bg-white rounded-full cursor-pointer md:hidden hover:bg-gray-100">
        <svg
          class="w-6 h-6 text-gray-700"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path d="M4 6h16M4 12h16M4 18h16" />
        </svg>
        <svg
          class="w-6 h-6 text-gray-700"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          style="display: none;"
        >
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </div>
    </div>
  </nav>
</template>

<style>
a.nuxt-link-active {
  font-weight: bold;
}
</style>
