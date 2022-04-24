<template>
    <div>

        <div class="text-white grid grid-cols-3 gap-4">
            <div v-for="animation of animations" class="p-10 text-center items-center">
                <div :class="getAnimation(animation.class)">
                    <span>{{animation.name}}</span>
                </div>
                
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
                {name: 'float', id: 0, class: 'h-float'},
                {name: 'rotate180', id: 1, class: 'h-rotate-180'},
                {name: 'rotate360', id: 2, class: 'h-rotate-360'},
                {name: 'flex', id: 3, class: 'h-flex'},
                {name: 'transLeft', id: 4, class: 'h-transLeft'},
                {name: 'transRight', id: 5, class: 'h-transRight'},
                {name: 'transUp', id: 6, class: 'h-transUp'},
                {name: 'transDown', id: 7, class: 'h-transDown'},
                {name: 'toStretch', id: 8, class: 'h-toStretch'},
                {name: 'rotate360', id: 9, class: 'h-rotate360'},
                {name: 'skew', id: 10, class: 'h-skew'},
                {name: 'skewX', id: 11, class: 'h-skewX'},
                {name: 'skewY', id: 12, class: 'h-skewY'},
                {name: 'floatFluid', id: 13, class: ''},
                {name: 'grow', id: 14, class: ''},
                {name: 'flipUp360', id: 15, class: ''},
                {name: 'flipUp180', id: 16, class: ''},
                {name: 'flipSide180', id: 17, class: ''},
                {name: 'flipSide360', id: 18, class: ''},
                {name: 'shake', id: 19, class: ''},
                {name: 'shakeFix', id: 20, class: ''},
                {name: 'bounceShakeX', id: 21, class: ''},
                {name: 'bounceShakeY', id: 22, class: ''},
                {name: 'surprise', id: 23, class: ''},
                {name: 'jello', id: 24, class: ''},
                {name: 'swing', id: 25, class: ''},
                {name: 'hinge', id: 26}
                
            ]
        }
    },
    methods: {
        getAnimation(animationClass){
            let className = 'p-5 cursor-pointer bg-transparent border border-primary bg-primary text-white font-bold rounded';
            return `${className} ${animationClass}`;
        }
    },
    computed: {

    }
}
</script>