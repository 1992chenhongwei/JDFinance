<template lang="html">
    <Panel tittle="新品推荐" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.arrow">更多尖货 ></div>
            <Slider :options="swiperOption" :items="items" :cname="$style.slider"/>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue'
import Slider from "../core/slider.vue"
export default {
    components:{
        Panel,
        Slider,
    },
    data(){
        return {
            items:[{
                href    :"home",
                src     :"//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421"
            },{
                href    :"home",
                src     :"//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421"
            },{
                href    :"home",
                src     :"//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421"
            },{
                href    :"home",
                src     :"//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421"
            },{
                href    :"home",
                src     :"//img12.360buyimg.com/jrpmobile/jfs/t13963/267/2355123229/48850/254f797a/5a3c59aeN9cb550f6.jpg?width=335&height=421"
            }],
            swiperOption: {
                slidesPerView: 3,
                spaceBetween: 30,
                freeMode: true,
            }
        }
    }
}
</script>

<style lang="scss" module>
@import "../../css/element.scss";
    .panel{
        @include panel;
        >h4{
            border-bottom: 1px solid #ddd;
        }
        .content{
            padding-bottom: 25px;
            position: relative;
            img{
                width:100%;
            }
            .arrow{
                position: absolute;
                top: -66px;
                right: 20px;
                color: #999;
                font-size: 24px;
            }
        }
    }  
</style>
