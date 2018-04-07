<template lang="html">
    <Panel tittle="活动中心" :class="$style.panel">
        <section :class="$style.content">
            <swiper :options="options" :class="$style.addbg">
                <swiper-slide :class="$style.addml"><span>百万白条券免费送，速来领取！！</span><em>></em></swiper-slide>
                <swiper-slide :class="$style.addml"><span>签到领流量，1元500M！</span><em>></em></swiper-slide>
            </swiper>
        </section>
    </Panel>
</template>

<script>
    import {swiper,swiperSlide} from 'vue-awesome-swiper'
    import Panel from '../core/panel.vue'
    export default {
        components:{
            Panel,
            swiper,
            swiperSlide
        },
        data(){
            return {
                options: {
                    autoplay:true,
                    loop:true,
                    direction: 'vertical',
                }
            }
        }
    }
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel{
        @include panel;
        margin-top: 120px!important;
        >h4{
            display: none;
        }
        .content{
            height: 72px;
            line-height: 72px;
            overflow: hidden;
            color: #333;
            font-size: 24px;
            .addbg{
                background: url(//m.jr.jd.com/spe/qyy/main/images/scroll_title_img.png) left top no-repeat;
                .addml{
                    margin-left: 180px;
                    overflow: hidden;
                    text-overflow: ellipsis;
                    white-space: nowrap;
                }
                em{
                    float: right;
                    margin-right: 20px;
                    color: #ddd;
                }
            }
        }
    }
</style>