<template lang="html">
    <Panel tittle="下载APP" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.header">
                <p>会赚钱 懂生活的人</p>
                <p>都在这里</p>
            </div>
            <div :class="$style.body">
                <p>新人首次登陆领888礼包</p>
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t10054/120/2165982932/56512/574e4766/59f031f3N1a75e42d.png?width=1125&height=890" alt="">
            </div>
            <div :class="$style.footor">
                <div :class="$style.img">
                    <img src="//m.jr.jd.com/spe/downloadApp/images/logo.png" alt="">
                    <span>安装京东金融</span>
                </div>
                <p>已安装，点击这里直接打开</p>
            </div>
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue'
export default {
    components:{
        Panel,
    }
}
</script>


<style lang="scss" module>
    @import "../../css/element.scss";
    body,html{
                background: #fff;
                margin: 0 auto;
            }
    .panel{
        @include panel;
        margin: 0!important;
        text-align: center;
        >h4{
            display: none;
        }
        .content{
            .header{
                width: 100%;
                color: #444;
                margin: 50px auto 30px;
                p{
                    font-size: 42px;
                    line-height: 56px;
                    height: 56px;
                }
            }
            .body{
                width: 100%;
                color: #999;
                font-size: 24px;
                img{
                    width: 80%;
                }
            }
            .footor{
                position: absolute;
                width: 100%;
                bottom: 60px;
                .img{
                    @include flex(row);
                    align-items: center;
                    justify-content: center;
                    background: #F55C33;
                    background-image: linear-gradient(270deg,#F55C33 0,#EE2D1B 75%);
                    color: #fff;
                    line-height: 100px;
                    height: 100px;
                    margin: 20px 10%;
                    width: 80%;
                    img{
                        width: 54px;
                        height: 54px;
                        margin: 23px;
                    }
                }
                p{
                    color: #F4552F;
                    font-size: 32px;
                    line-height: 40px;
                    height: 40px;
                }
            }
        }
    }
</style>
