<template>
    <div>
            <div class="max-w-7xl max mx-auto">
        <div class="grid grid-cols-2 gap-8 py-64 items-center">
            <div>
                <h1 class="primary-orange font-bold text-4xl">I'm</h1>
                <h1 class="text-white font-bold  text-7xl">Avalojandro</h1>
                <h1 class="text-gray-500 text-2xl pt-4 leading-8">Front-End Developer, gamer, drummer and creator of cattocss based in LATAM.</h1>
            </div>
            <div>
                <center class="relative">
                   <img src="/avalojandro.png" class="z-20 relative rounded-full p-2 bg-white w-2/4" alt="">
                   <div class="absolute w-36 h-36 bg-blue-700 z-30 rounded transform translate-x-24 -translate-y-24">
                       &nbsp;
                   </div>
                   <div class="absolute triangle rounded z-0 transform left-0 top-0 translate-x-32">
                       &nbsp;
                   </div>
                   <div class="absolute w-24 h-72 bg-green-500 right-0 top-0 z-0 rounded transform -translate-x-24">
                       &nbsp;
                   </div>                   
                </center>
            </div>
        </div>
    </div>

    <div class="bg-black py-64">
        <div class="max-w-7xl max mx-auto text-center">
            <h1><h1 class="text-white font-bold text-7xl">Knowledge</h1></h1>
            <center class="py-12">
                <img src="/knowledge/frontend.png" class="w-64 inline" alt="FrontEnd">
                <img src="/knowledge/vue.png" class="w-20 mx-2 inline" alt="Vuejs">
                <img src="/knowledge/angular.png" class="w-20 mx-2 inline" alt="Angular">
                <img src="/knowledge/ionic.png" class="w-20 mx-2 inline" alt="Ionic framework">                
            </center>
        </div>
    </div>
    
    </div>
</template>

<style scoped>
.triangle {
  width: 0; 
  height: 0; 
  border-top: 80px solid transparent;
  border-bottom: 80px solid transparent;
  
  border-left: 80px solid rgb(218, 8, 8);
}

</style>