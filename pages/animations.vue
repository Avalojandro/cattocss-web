<template>
    <div class="h-screen overflow-hidden">
        <div class="grid grid-cols-2 p-12">

            <!-- Demo view -->
            <div class="h-screen overflow-auto text-white">

                <List/>

            </div>
            
            <!-- Code view -->
            <div class="text-white items-center justify-center flex">
               <CodePreview/> 
            </div>
        </div>
    </div>
</template>

<style>
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

