<template>
  <div class="h-screen overflow-hidden">
    <div class="grid grid-cols-1 gap-y-8 lg:gap-y-0 lg:grid-cols-2 py-12 pl-0 2xl:pl-12">
      <!-- Demo view -->
      <div class="h-72 lg:h-screen overflow-auto text-white">
        <nav class="py-4 space-x-4 text-center">
          <a v-for="type in types" id="{type}" :key="type" href="#hover" class="p-2 target font-bold inline-block cursor-pointer border-b-4 border-primary-catto">{{ type }}</a>
        </nav>
        <List @getAnimationName="listDataName" @getAnimationCode="listDataCode" />
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
      animationCode: null,
      types: ['Hover', 'One Time', 'Loops', 'Buttons']
    }
  },
  methods: {
    listDataName (value) {
      this.animationName = value
    },
    listDataCode (value) {
      this.animationCode = value
    },
    acive (index = 0) {

    }
  }

}
</script>

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

:target{
  @apply text-primary-catto;
}

</style>
