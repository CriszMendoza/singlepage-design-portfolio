<template>
  <div>
    <my-header/>
    
    <main>
      <h1>Design solutions made easy</h1>
      <p>With over ten years of experience in various design disciplines, I'm your one-stop shop for your design needs.</p>
    </main>

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

export default {
  components:{
    BaseButton,
    BaseArrow,
    MyHeader,
    Patterns,
    Hero
  }

}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main';

main{
  width: 752px;
  text-align: center;
  margin: 0 auto 80px;
  h1{
    margin-bottom: 23px;
    @include font-heading-l;
  }
}






</style>