<template lang="html">
    <Panel tittle="白条福利" :class="$style.panel">
            <div :class="$style.content">
                    <dl>
                        <dt>
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4378/62/155957680/9017/16463551/58affd58Nb5c9198e.jpg?width=120&height=120" alt="">
                        </dt>
                        <dt>
                            <p>开通白条</p>
                            <p>送188元礼包</p>
                        </dt>
                        <dt>立即开通 ></dt>
                    </dl>
                    <dl>
                        <dt>
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4150/330/141981421/9147/604e3e04/58affc3bNbfa8f9d7.jpg?width=120&height=120" alt="">
                        </dt>
                        <dt>
                            <p>白条闪付</p>
                            <p>新手享158元礼包</p>
                        </dt>
                        <dt>随机立减 ></dt>
                    </dl>
                    <dl>
                        <dt>
                            <img src="//img12.360buyimg.com/jrpmobile/jfs/t4270/96/1102370053/8651/58b7fa5a/58bd2e10N453e9464.jpg?width=120&height=120" alt="">
                        </dt>
                        <dt>
                            <p>白条提额</p>
                            <p>金融app专享提额礼包</p>
                        </dt>
                        <dt>去提额 ></dt>
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
                              color: #999;
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
