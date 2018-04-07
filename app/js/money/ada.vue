<template lang="html">
    <Panel tittle="神券满减" :class="$style.panel">
        <section :class="$style.content">
            <router-link :to="{name :'home'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t5842/235/8356236245/38364/2112fd7e/597a95d4Ne01da140.png?width=750&height=270" alt="">
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