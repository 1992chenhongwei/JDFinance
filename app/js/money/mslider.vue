<template lang="html">
    <article>
        <Slider :items="items" :cname="$style.slider"/>
    </article>
</template>

<script>
    import Slider from "../core/slider.vue"
    export default {
        components:{
            Slider,
        },
        data(){
            return {
                items   : [{
                    href    : "home",
                    src     : "//img12.360buyimg.com/jrpmobile/jfs/t15097/249/2268830415/20640/397e0ddf/5a976c28Nc5f227d1.jpg?width=750&height=400"
                },{
                    href    : "home",
                    src     : "//img12.360buyimg.com/jrpmobile/jfs/t15097/249/2268830415/20640/397e0ddf/5a976c28Nc5f227d1.jpg?width=750&height=400"
                },{
                    href    : "home",
                    src     : "//img12.360buyimg.com/jrpmobile/jfs/t18787/96/583735472/19041/545127d6/5a976b05N1a6a412a.jpg?width=750&height=400"
                }],
            }
        }
    }
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .slider{
        padding-top: 120px;
        img{
            height: 100%;
            width: 100%;
        }
    }
</style>