<template lang="html">
    <Panel tittle="理财精选" :class="$style.panel">
            <div :class="$style.content">
                    <dl>
                        <dt>
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t3670/58/543125556/2606/a65096b9/580d80afN63b1085a.png?width=76&height=76" alt="">
                        </dt>
                        <dt>
                            <p>月度理财</p>
                            <p>预期年化收益率4.50%</p>
                        </dt>
                        <dt>去赚钱 ></dt>
                    </dl>
                    <dl>
                        <dt>
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t3679/44/511862277/2728/c1c6b2bf/580d8189N6b6f8052.png?width=76&height=76" alt="">
                        </dt>
                        <dt>
                            <p>季度理财</p>
                            <p>历史年化回报率5.50%</p>
                        </dt>
                        <dt>去赚钱 ></dt>
                    </dl>
                    <dl>
                        <dt>
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t3331/69/580199498/3074/d5bb21c5/580d7f6cN7f35e596.png?width=76&height=76" alt="">
                        </dt>
                        <dt>
                            <p>一年理财</p>
                            <p>历史年化回报率5.80%</p>
                        </dt>
                        <dt>去赚钱 ></dt>
                    </dl>
            </div>
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
            border-bottom: 1px solid #ddd;
        }
        .content{
           @include flex(column);
              dl{
                  &:after{
                      content: " ";
                      box-sizing: border-box;
                      height: 0;
                      width: 100%;
                      margin-left: 150px;
                      border-bottom: 1px solid #ddd;
                  }
                  @include flex(row);
                  align-items: center;
                  dt{
                      &:nth-child(2){
                          width: 50%;
                          
                      }
                      color: #FF801A;
                      font-size: 28px;
                      img{
                          width: 88px;
                          height: 88px;
                          margin: 10px 40px;
                      }
                      p{
                          &:nth-child(1){
                              font-size: 30px;
                              line-height: 40px;
                              height: 40px;
                              color: #333;
                          }
                          &:nth-child(2){
                              font-size: 20px;
                              line-height: 40px;
                              height: 40px;
                              color: #ff3232;
                              white-space: nowrap;
                              overflow: hidden;
                              text-overflow: ellipsis;
                          }
                      }
                  }
              }
        }
    }  
</style>
