<template>
    <div class="container h-full max-w-lg px-4 mx-auto text-left md:max-w-none md:text-center">
        <h1 class="text-5xl px-12 pt-32 font-extrabold leading-10 tracking-tight text-left text-gray-900 md:text-center sm:leading-none md:text-6xl lg:text-7xl">
            <span class="inline md:block primary-orange"><span class="text-white">What</span> is <span class="text-white">catto</span>css<span class="text-white">?</span></span> 
        </h1>

         <p class="text-white px-12 md:px-20 lg:px-20 xl:px-96 py-8 text-lg">
            This project was developed with one goal in mind: that all web developers have a place where they can easily and quickly find css animations to 
            adapt to their websites without the need to install libraries or packages, cattocss contains a generous list of css animations with access to its source code easily and quickly. 
        </p>

        <div class="img-center inline">
            <center>
            <img src="table.svg" class="lg:w-1/4 img-center py-12" alt="">
            </center>
        </div>

        <!-- div 1 -->
        <div class="grid grid-cols-1 xl:grid-cols-2 items-center gap-12 py-20 px-12">
            <div class=" text-left text-white">
                <div class="text-5xl md:text-6xl lg:text-7xl font-extrabold">
                    The <span class="primary-orange">first</span> steps    
                </div>
                <br>
                <div class="text-lg">
                    In 2020 the first version of cattocss was launched on the internet, with a total of 80 animations of different styles. At the time it was thought to be a css animation library that needed to be downloaded.
                    <br><br>
                    It got a considerable amount of views, and was even mentioned in some blogs, however, cattocss stopped receiving updates for almost over a year.
                </div>
            </div>
            <div><img class="rounded-xl" src="/catto-first.png" alt=""></div>
        </div>

        <!-- div 2 -->
        <div class="grid grid-cols-1 xl:grid-cols-2 img-center items-center gap-8 py-20 px-12">
            <div class="img-center order-last xl:order-first">
              <img class="inline rounded-xl w-2/4" src="tommy2.jpg" alt="">
            </div>
            <div class=" text-left text-white">
                <div class="text-5xl md:text-6xl lg:text-7xl font-extrabold">
                    Why <span class="primary-orange">that</span> name?    
                </div>
                <br>
                <div class="text-lg">
                    Some time ago I had a cat called "Misho", we rescued him from the street, and he became a new member of the family, he lived with us for a couple of years, however, he passed away unexpectedly.
                    <br><br>
                    That was a very significant period for me, because it was at the time when I started my path as a developer, so when I decided to create a project that would help me enter the world of development, I didn't want to miss the opportunity. to remember my friend, taking an orange cat as Misho as a logo and creating a name that was the combination of "Cat" and "Gato" (cat in Spanish), this is how the name cattocss was born.
                    <br><br>
                    "Tommy" has helped me get over the loss of "Misho" and I have committed myself to not making the same mistakes I did before, becoming much more responsible, understanding that a pet is much more than food and bed. 
                    <br>
                    Now Tommy and I are very close and I hope we can live many years together.  
                </div>
            </div>
        </div>

    </div>
</template>

<style scoped>
    .floating{
        	animation: float 4s ease-in-out infinite;
    }

    .floating2{
        	animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
        0% {
            box-shadow: 0 5px 15px 0px rgba(0, 0, 0, 0);
            transform: translatey(0px);
             transform:rotate(2deg);
        }
        50% {
            box-shadow: 0 25px 15px 0px rgba(255, 255, 255, 0);
            transform: translatey(-10px);
             transform:rotate(-2deg);
        }
        100% {
            box-shadow: 0 5px 15px 0px rgba(0, 0, 0, 0);
            transform: translatey(0px);
             transform:rotate(2deg);
        }
    }

    @keyframes float2 {
        0% {
            box-shadow: 0 5px 15px 0px rgba(0, 0, 0, 0);
            transform: translatey(-10px);
            transform:rotate(-4deg);
        }
        50% {
            box-shadow: 0 25px 15px 0px rgba(255, 255, 255, 0);
            transform: translatey(0px);
            transform:rotate(2deg);
        }
        100% {
            box-shadow: 0 5px 15px 0px rgba(0, 0, 0, 0);
            transform: translatey(-10px);
            transform:rotate(-4deg);
        }
    }

</style>