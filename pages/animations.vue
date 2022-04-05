<template>
    <div class="h-screen overflow-hidden">
        <div class="grid grid-cols-2 p-12">

            <!-- Demo view -->
            <div class="h-screen overflow-auto text-white">

                <List/>

            </div>
            
            <!-- Code view -->
            <div class="text-white items-center justify-center flex">
                <div>
                <div class="text-white text-center text-5xl font-bold">
                    Animation name
                </div>
                <div class="m-12 p-12 bg-black rounded-lg">
                    Here is where the code of the animation will be showed
                </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
::-webkit-scrollbar {
  width: 3px;
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

