<template lang="html">
    <Panel tittle="In货推荐" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.item" v-for="item in items" :key="item.href">
                <img :src="item.href" alt="">
                <label>精选</label>
                <section :class="$style.list">
                    <div :class="$style.product" v-for="list in item.lists" :key="list.href">
                        <img :src="list.href" alt="">
                        <p :class="$style.title">{{list.title}}</p>
                        <p :class="$style.price"><em>{{list.price}}</em>起</p>
                        <article>
                            <div :class="$style.wrapper">
                                <div :class="$style.inner" :style="{width:list.progress+'%'}"></div>
                            </div>
                            <p>{{list.progress}}%</p>
                        </article>
                    </div>
                </section>
            </div>
        </section>
    </Panel>
</template>

<script>
    import Panel from '../core/panel.vue'
    export default {
        components: {
            Panel,
        },
        data(){
            return{
                items:[{
                    href:"//img12.360buyimg.com/jrpmobile/jfs/t3406/210/2247820735/50952/86016eea/5846d8e7N20446dbd.png?width=750&height=200",
                    lists:[{
                        href:"//img30.360buyimg.com/cf/s250x250_jfs/t14881/283/656508232/143980/9b606acf/5a33a171N18c9c80a.jpg",
                        title:"双响炮蓝牙音箱",
                        price:"29.00",
                        progress:40,
                    },{
                        href:"//img30.360buyimg.com/cf/s250x250_jfs/t15529/308/632300625/135123/adb9c6d0/5a37676dNc31da9ea.jpg",
                        title:"脑波相机",
                        price:"998.00",
                        progress:67,
                    },]
                },{
                    href:"//img12.360buyimg.com/jrpmobile/jfs/t3739/82/2244582797/54399/746c7d79/5846a953N66b67d05.png?width=750&height=200",
                    lists:[{
                        href:"//img30.360buyimg.com/cf/s250x250_jfs/t11257/287/2281727659/55759/e00b90a/5a138f21N32dca834.jpg",
                        title:"智能电动牙刷",
                        price:"19.00",
                        progress:23,
                    },{
                        href:"//img30.360buyimg.com/cf/s250x250_jfs/t14209/293/662014092/61635/bba5c330/5a33a983N077cac56.jpg",
                        title:"烟草加热电子烟",
                        price:"258.00",
                        progress:200,
                    },]
                },{
                    href:"//img12.360buyimg.com/jrpmobile/jfs/t3214/113/4408032436/61548/ce316eef/5846d310Ne93f00c9.png?width=750&height=200",
                    lists:[{
                        href:"//img30.360buyimg.com/cf/s250x250_jfs/t15007/47/884045069/149879/17987250/5a3cb182N15868ea1.jpg",
                        title:"赖公高淮封藏老酒",
                        price:"99.00",
                        progress:45,
                    },{
                        href:"//img30.360buyimg.com/cf/s250x250_jfs/t14197/160/546457496/134173/4e1baccd/5a30ccc5Na44f7492.jpg",
                        title:"阳澄湖闸蟹",
                        price:"58.00",
                        progress:32,
                    },]
                }]
            }
        }
    }
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel {
        @include panel;
        .content {
           @include flex(column);
            .item{
                margin-bottom: 40px;
                >img{
                    display: block;
                    width: 100%;
                    height: 170px;
                }
                >label{
                    display: inline-block;
                    color: #ff0000;
                    background: #C1C1C1;
                    font-size: 20px;
                    line-height: 40px;
                    height: 40px;
                    padding: 0 10px;
                }
                .list{
                    @include flex(row);
                    .product{
                        width: 50%;
                        height: 396px;
                        text-align: center;
                        background: rgba(0, 0, 0, 0.02);
                        img{
                            width: 180px;
                            height: 180px;
                            margin-bottom: 20px;
                        }
                        .title{
                            font-size: 28px;
                            color: #444;
                        }
                        .price{
                            line-height: 48px;
                            height: 48px;
                            font-size: 20px;
                            color: #999;
                            em{
                                margin-right: 10px;
                                font-size: 36px;
                                color: #ff3232;
                                &:before{
                                    content: "￥";
                                    font-size: 28px;
                                }
                            }
                        }
                        article{
                            @include flex(row);
                            align-items: center;
                            justify-content: space-around;
                            padding: 0 20px;
                            line-height: 30px;
                            height: 30px;
                            margin-top: 20px;
                            .wrapper{
                                width:144px;
                                height: 10px;
                                background: #f6e6e6;
                                border-radius: 22px;
                                .inner{
                                    max-width: 100%;
                                    height: 10px;
                                    background-image: linear-gradient(270deg, #F55 1%, #FF9C31 100%);
                                    border-radius: 22px;
                                }
                            }
                            p{
                                font-size: 24px;
                                color: #999;
                            }
                        }
                    }
                }
            }
        }
    }
</style>