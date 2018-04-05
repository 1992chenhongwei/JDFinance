<template lang="html">
    <Panel tittle="理财精选" :class="$style.panel">
        <section :class="$style.content">
            <dl :class="$style.item" v-for="item in items" ::key="item.title">
                <dt>{{item.title}}<span :class="$style.red">{{item.sub}}</span></dt>
                <dd :class="$style.rate">{{item.rate}}</dd>
                <dd :class="$style.text">{{item.text}}</dd>
            </dl>
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
            return {
                items:[{
                    title   :"定期理财",
                    sub     :"理财首选",
                    rate    :"5.60%",
                    text    :"七日年化收益率"
                },{
                    title   :"小白理财",
                    sub     :"理财首选",
                    rate    :"5.60%",
                    text    :"七日年化收益率"
                },{
                    title   :"月月盈",
                    sub     :"养老保障",
                    rate    :"5.60%",
                    text    :"七日年化收益率"
                },{
                    title   :"小白基金",
                    sub     :"天天赚钱",
                    rate    :"5.60%",
                    text    :"七日年化收益率"
                }]
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
            @include flex(row);
            &:after{
                content: " ";
                display: block;
                width: 100%;
                height: 0px;
                box-sizing: border-box;
                border-bottom: 1px solid #ddd;
                position: relative;
                top: -190px;
            }
            .item{
            width: 50%;
            padding-top: 20px;
            padding-left: 20px;
            box-sizing: border-box;
            margin-bottom: 20px;
            position: relative;
            &:after{
                content:" ";
                height: 136px;
                width: 0px;
                display: block;
                position: absolute;
                border-right: 1px solid #ddd;
                right: 0;
                top:30px;
            }
            &:nth-child(2n){
                &:after{
                    display: none;
                }
            }
            dt{
                font-size: 28px;
                line-height: 50px;
                height: 50px;
                font-weight: bold;
                color: #333;
                .red{
                    margin-left: 5px;
                    font-size: 22px;
                    color: #FF5155;
                    border: 1px solid #FF5155;
                    padding: 0 6px 0 6px;
                }
            }
            .rate{
                color: #FF5155;
                line-height: 50px;
                height: 50px;
                font-weight: bold;
            }
            .text{
                color: #999;
                line-height: 50px;
                height: 50px;
                font-size: 24px;
            }
        }
        }
}
</style>