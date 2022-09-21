<template>
  <div>
    <my-header/>

    <my-main/>

    <my-patterns/>

    <my-hero/>

    <my-work/>  

    <my-footer/>

    <my-header/>
    
  </div>
</template>

<script>
import MyHeader from '~/components/layout/MyHeader'
import MyPatterns from '~/components/layout/MyPatterns'
import MyHero from '~/components/layout/MyHero'
import MyMain from '~/components/layout/MyMain'
import MyWork from '~/components/layout/MyWork'
import MyFooter from '~/components/layout/MyFooter'

export default {
  components:{
    MyHeader,
    MyPatterns,
    MyHero,
    MyMain,
    MyWork,
    MyFooter
  }

}
</script>

<style lang="scss" scoped>

</style>