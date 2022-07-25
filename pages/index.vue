<template>
  <div class="h-screen overflow-hidden">
    <div class="grid grid-cols-1 gap-y-8 lg:gap-y-0 lg:grid-cols-2 py-12 pl-0 2xl:pl-12">
      <!-- Demo view -->
      <div class="h-72 lg:h-screen overflow-auto">
        <nav class="py-4 space-x-4 text-center">
          <a v-for="(type, index) in types" :key="type" :class="selectedItemStyle(index)" @click="itemIndex(index)">{{ type }}</a>
        </nav>
        <HoverAnimations @getAnimationName="listDataName" @getAnimationCode="listDataCode" />
        <OneTimeAnimations @getAnimationName="listDataName" @getAnimationCode="listDataCode" />
        <LoopsAnimations @getAnimationName="listDataName" @getAnimationCode="listDataCode" />
        <AnimatedButtons @getAnimationName="listDataName" @getAnimationCode="listDataCode" />
      </div>

      <!-- Code view -->
      <div class="text-white items-center justify-center xl:flex">
        <CodePreview :animation-name="animationName" :animation-code="animationCode" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      animationName: null,
      selectedItem: 0,
      animationCode: null,
      types: ['Hover', 'One Time', 'Loops', 'Buttons']
    }
  },
  methods: {
    selectedItemStyle (index) {
      const className = 'p-2 target font-bold inline-block cursor-pointer transition-all duration-200 ease-in-out'
      return (index === this.selectedItem) ? `${className} border-b-4 text-primary-catto border-primary-catto` : `${className} border-b text-white border-white`
    },
    listDataName (value) {
      this.animationName = value
    },
    listDataCode (value) {
      this.animationCode = value
    },
    itemIndex (i) {
      this.selectedItem = i
    }
  }

}
</script>

<style scoped>

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

:target{
  @apply text-primary-catto;
}

</style>
