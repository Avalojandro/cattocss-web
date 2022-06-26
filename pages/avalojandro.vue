<template>
  <div>
    <div class="max-w-7xl px-8 xl:px-0 max mx-auto">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 py-12 lg:py-64 items-center">
        <div class="text-center lg:text-left">
          <h1 class="text-primary-catto font-bold text-4xl">
            I'm
          </h1>
          <h1 class="text-white font-bold  text-7xl">
            Avalojandro
          </h1>
          <h1 class="text-gray-500 text-2xl pt-4 lg:px-0 leading-8">
            Front-End Developer, gamer, drummer and creator of cattocss based in LATAM.
          </h1>
          <div class="pt-3 space-x-2">
            <img src="/git.png" class="inline w-7" alt="">
            <img src="/linkedin.png" class="inline w-6" alt="">
            <img src="/yt.png" class="inline w-8" alt="">
          </div>
        </div>
        <div>
          <center class="relative">
            <img src="/avalojandro.png" class="z-20 relative rounded-full p-2 bg-white w-3/4 md:w-2/4" alt="">
            <div class="absolute hidden md:block w-20 xl:w-36 h-20 xl:h-36 bg-blue-700 z-30 rounded blue-sqr">
                       &nbsp;
            </div>
            <div class="absolute hidden md:block triangle rounded z-0 transform left-0 top-0 red-triangle">
                       &nbsp;
            </div>
            <div class="absolute hidden md:block w-12 xl:w-24 h-36 xl:h-72 bg-green-500 right-0 top-0 z-0 rounded green-sqr">
                       &nbsp;
            </div>
          </center>
        </div>
      </div>
    </div>

    <!-- <div class="bg-black py-64">
        <div class="max-w-7xl max mx-auto text-center">
            <h1 class="text-white font-bold text-7xl">Knowledge</h1>
            <center class="py-12">
                <img src="/knowledge/frontend.png" class="w-64 inline" alt="Avalojandro">
                <img src="/knowledge/vue.png" class="w-20 mx-2 inline" alt="Avalojandro">
                <img src="/knowledge/react.png" class="w-20 mx-2 inline" alt="Avalojandro">
                <img src="/knowledge/angular.png" class="w-20 mx-2 inline" alt="Avalojandro">
                <img src="/knowledge/ionic.png" class="w-20 mx-2 inline" alt="Ionic framework">
            </center>
        </div>
    </div> -->

    <!-- <div class="bg-black py-64">
        <div class="max-w-7xl max mx-auto text-center">
            <h1 class="text-white font-bold text-7xl pb-20">My <span class="text-primary-catto">favorite</span> video <span class="text-primary-catto">games</span></h1>
              <div class="grid grid-cols-3 items-center gap-24">
                <div class="relative">
                  <img class="relative  z-10" src="/games/mario.png" alt="">
                  <img class="transform absolute z-0 -translate-y-96 backgrounds" src="/games/mario-bg.png" alt="">
                  <img class="transform absolute right-0 -translate-y-24 w-52 z-20 backgrounds" src="/games/mario-logo.png" alt="">
                </div>
                <div class="relative">
                  <img class="relative  z-10" src="/games/botw.png" alt="">
                  <img class="transform absolute z-0 -translate-y-96 backgrounds" src="/games/botw-bg.jpg" alt="">
                  <img class="transform absolute right-0 -translate-y-52 w-52 z-20 backgrounds" src="/games/botw-logo.png" alt="">
                </div>
                <div class="relative">
                  <img class="relative  z-10 w-52" src="/games/sonic.png" alt="">
                  <img class=" absolute z-0 trans backgrounds" src="/games/sonic-bg.png" alt="">
                  <img class="transform absolute right-0 -translate-y-36 w-52 z-20 backgrounds" src="/games/sonic-logo.png" alt="">
                </div>
              </div>
        </div>
    </div> -->
  </div>
</template>

<style>
.triangle {
  width: 0;
  height: 0;
  border-top: 80px solid transparent;
  border-bottom: 80px solid transparent;

  border-left: 80px solid rgb(218, 8, 8);
}

.backgrounds{
  border-radius: 10px;
}

.trans{
  transform: translateY(-24rem);
}

.blue-sqr{
  animation-name: animation;
  animation-duration: 50s;
  animation-iteration-count: infinite;
}

.green-sqr{
  animation-name: animation2;
  animation-duration: 27s;
  animation-iteration-count: infinite;
}

.red-triangle{
  animation-name: animation3;
  animation-duration: 10s;
  animation-iteration-count: infinite;
}

@keyframes animation {
        0% {transform: rotate3d(0, 0, 1, 15deg) translateX(6rem) translateY(-6rem);}
        25%{transform: rotate3d(0, 0, 1, -10deg) translateX(7rem) translateY(-6rem);}
        50% {transform: rotate3d(0, 0, 1, 5deg) translateX(8rem) translateY(-6rem);}
        75%{transform: rotate3d(0, 0, 1, -5deg) translateX(7rem) translateY(-6rem);}
        100% {transform: rotate3d(0, 0, 1, 15deg) translateX(6rem) translateY(-6rem);}
}

@keyframes animation2 {
        0%{transform: rotate3d(0, 0, 10, -10deg) translateX(-6rem) }
        25%{transform: rotate3d(0, 0, 1, 5deg) translateX(-6rem) }
        50%{transform: rotate3d(0, 0, 1, 0deg) translateX(-6rem) }
        75%{transform: rotate3d(0, 0, 1, 5deg) translateX(-6rem) }
        100%{transform: rotate3d(0, 0, 10, -10deg) translateX(-6rem) }
}

@keyframes animation3 {
        0%{transform: rotate3d(0, 0, 10, -10deg) translateX(8rem) }
        25%{transform: rotate3d(0, 0, 1, 5deg) translateX(8rem) }
        50%{transform: rotate3d(0, 0, 1, 0deg) translateX(8rem) }
        75%{transform: rotate3d(0, 0, 1, 5deg) translateX(8rem) }
        100%{transform: rotate3d(0, 0, 10, -10deg) translateX(8rem) }
}

</style>
