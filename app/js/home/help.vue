<template lang="html">
    <Panel tittle="帮助中心" :class="$style.panel">
        <section :class="$style.content">
            <router-link to="{name :'home'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t2842/350/3035567089/14791/5f6ff93d/577cf395N31e76288.png?width=1125&height=252" alt="">
            </router-link>
        </section>
    </Panel>
</template>

<script>
    import Panel from '../core/panel.vue'
    export default {
        components: {
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
        .content{
            img{
            width: 100%;
        }
        }
}
</style>