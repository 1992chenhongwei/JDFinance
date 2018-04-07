<template lang="html">
    <Panel tittle="生活服务" :class="$style.panel">
        <ul :class="$style.content">
            <li :class="$style.item">
                <div>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108" alt="">
                    <p>客户端</p>
                </div>
                <div>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2824/256/2966087355/831/188bfa25/577cf3dcN18aadbf2.png?width=108&height=108" alt="">
                    <p>触屏版</p>
                </div>
                <div>
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2920/282/1283157010/1040/23f1430b/577cf3e5N53f740b8.png?width=108&height=108" alt="">
                    <p>电脑版</p>
                </div>
            </li>
            <li :class="$style.item">
                <p>Copyright © 2004-2018 京东JD.com 版权所有</p>
            </li>
            <li :class="$style.item">
                <p>投资有风险，购买需谨慎</p>
            </li>
            <li :class="$style.item">
                <p>京东金融平台服务协议</p>
            </li>
            <li :class="$style.item">
                <p>京东金融隐私政策</p>
            </li>
        </ul>
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
    .panel{
        @include panel;
        >h4{
            display: none;
        }
        margin-bottom:100px;
        .content{
           @include flex();
           .item{
                background: #F5F5F5;
                text-align: center;
                font-size: 24px;
                color: #999;
               &:nth-child(1){
                   @include flex(row);
                   div{
                       padding-top: 20px;
                       width: 33.3333%;
                       img{
                           width: 80px;
                       }
                       p{
                           border: 0px;
                           height: 60px;
                           line-height: 60px;
                       }
                   }
               }
               img{
                   width: 100%;
               }
               p{
                    height: 80px;
                    line-height: 80px;
                    box-sizing: border-box;
                    border-top: 1px solid #ddd;
               }
               
           }
        }
    }  
</style>