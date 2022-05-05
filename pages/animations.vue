<template>
    <div class="h-screen overflow-hidden">
        <div class="grid grid-cols-1 gap-y-8 lg:gap-y-0 lg:grid-cols-2 py-12 pl-0 2xl:pl-12">

            <!-- Demo view -->
            <div class="h-72 lg:h-screen overflow-auto text-white">
                <div class="py-4 space-x-4 text-center">
                  <span class="p-2 bg-white primary-orange cursor-pointer rounded-full">Hover</span>
                  <span class="p-2 bg-transparent text-white border border-red-500 cursor-pointer rounded-full">Infinite</span>
                  <span class="p-2 bg-transparent text-white border border-red-500 cursor-pointer rounded-full">Infinite</span>
                  <span class="p-2 bg-transparent text-white border border-red-500 cursor-pointer rounded-full">Infinite</span>
                  
                </div>
                <List @getAnimationName="listDataName" @getAnimationCode="listDataCode"/>
            </div>
            
            <!-- Code view -->
            <div class="text-white items-center justify-center xl:flex">
               <CodePreview :animationName="animationName" :animationCode="animationCode"/> 
            </div>
        </div>
    </div>
</template>

<style>

::-webkit-scrollbar {
  width: 3px;
  height: 3px;
}
::-webkit-scrollbar-track {
  background: #ffffff96;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #f71e1e;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #f71e1e;
}


</style>

<script>
export default {
  data(){
    return {
      animationName: null,
      animationCode: null
    }
  },
  methods: {
    listDataName(value){
      this.animationName = value;
    },
    listDataCode(value){
      this.animationCode = value;
    }
  }

}
</script>
