<template lang="html">
    <div>
        <Heador/>
        <Slider/>
        <Ada/>
        <Money/>
        <Adb/>
        <Finance/>
        <Adc/>
        <Footor/>
        <Navbar/>
    </div>
</template>

<script>
import Heador from '../public/header.vue'
import Slider from './mslider.vue'
import Ada from './ada.vue'
import Money from './money.vue'
import Adb from './adb.vue'
import Finance from './finance.vue'
import Adc from './adc.vue'
import Footor from '../public/footor.vue'
import Navbar from '../public/navbar.vue'
export default {
  components:{
    Heador,
    Slider,
    Ada,
    Money,
    Adb,
    Finance,
    Adc,
    Footor,
    Navbar,
  }
}
</script>

<style lang="scss" module>
  
</style>
