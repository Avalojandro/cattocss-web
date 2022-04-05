<template>
    <div>

        <div class="text-white grid grid-cols-3 gap-4">
            <div v-for="animation of animations" class="p-10 text-center items-center">
                <span class="p-5 cursor-pointer bg-transparent border border-primary primary-orange font-bold rounded">{{animation.name}}</span>
            </div>
            <br>
        </div>

    </div>
</template>

<script>
export default {
    setup() {},
    data(){
        return {
            animations: [
                {name: 'float'},
                {name: 'rotate180'},
                {name: 'rotate360'},
                {name: 'flex'},
                {name: 'transLeft'},
                {name: 'transRight'},
                {name: 'transUp'},
                {name: 'transDown'},
                {name: 'toStretch'},
                {name: 'rotate360'},
                {name: 'skew'},
                {name: 'skewX'},
                {name: 'skewY'},
                {name: 'floatFluid'},
                {name: 'grow'},
                {name: 'flipUp360'},
                {name: 'flipUp180'},
                {name: 'flipSide180'},
                {name: 'flipSide360'},
                {name: 'shake'},
                {name: 'shakeFix'},
                {name: 'bounceShakeX'},
                {name: 'bounceShakeY'},
                {name: 'surprise'},
                {name: 'jello'},
                {name: 'swing'},
                {name: 'hinge'}
                
            ]
        }
    }
}
</script>