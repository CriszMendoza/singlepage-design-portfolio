<template>
  <div>
    <my-header/>

    <Main/>

    <Patterns/>

    <Hero/>

   

    

    My Work

    Book a call with me

    I'd love to have a chat to see how I can help you. The best first step is for us to discuss your project during a 
    free consultation. Then we can move forward from there.

    Free Consultation

    Free Consultation
    <BaseArrow direction='left'/>
    <BaseArrow direction='right'/>
    <base-button type='primary' title='Free Consultation'/>
  </div>
</template>

<script>
import BaseButton from '~/components/ux/BaseButton'
import BaseArrow from '~/components/ux/BaseArrow'
import MyHeader from '~/components/layout/MyHeader'
import Patterns from '~/components/layout/Patterns'
import Hero from '~/components/layout/Hero'
import Main from '~/components/layout/Main'

export default {
  components:{
    BaseButton,
    BaseArrow,
    MyHeader,
    Patterns,
    Hero,
    Main
  }

}
</script>

<style lang="scss" scoped>

</style>