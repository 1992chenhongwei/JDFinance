<template lang="html">
    <div>
        <Heador/>
        <Islider/>
        <Iousfree/>
        <Moreservice/>
        <Help/>
        <Footor/>
        <Navbar/>
    </div>
</template>

<script>
import Heador from '../public/header.vue'
import Islider from './islider.vue'
import Iousfree from './iousfree.vue'
import Moreservice from './moreservice.vue'
import Help from './help.vue'
import Footor from '../public/footor.vue'
import Navbar from '../public/navbar.vue'
export default {
  components:{
    Heador,
    Islider,
    Iousfree,
    Moreservice,
    Help,
    Footor,
    Navbar,
  }
}
</script>

<style lang="scss" module>
  
</style>
