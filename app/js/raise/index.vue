<template lang="html">
    <div>
        <Heador/>
        <Slider/>
        <Daily/>
        <In/>
        <Welfare/>
        <Footor/>
        <Navbar/>
    </div>
</template>

<script>
import Heador from '../public/header.vue'
import Slider from './rslider.vue'
import Daily from './daily.vue'
import In from './in.vue'
import Welfare from './welfare.vue'
import Footor from '../public/footor.vue'
import Navbar from '../public/navbar.vue'
export default {
  components:{
    Heador,
    Slider,
    Daily,
    In,
    Welfare,
    Footor,
    Navbar,
  }
}
</script>

<style lang="scss" module>
  
</style>
