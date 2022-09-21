<template>
  <div>
    <my-header/>
    

    Design solutions made easy

    With over ten years of experience in various design disciplines, I'm your one-stop shop for your design needs.

    Graphic Design
    UI/UX
    Apps
    Photography
    Illustrations
    Motion Graphics

    I'm Amy, and I'd love to work on your next project

    I love working with others to create beautiful design solutions. I've designed everything from brand illustrations 
    to complete mobile apps. I'm also handy with a camera!

    Free Consultation

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

export default {
  components:{
    BaseButton,
    BaseArrow,
    MyHeader
  }

}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main';

div{
  background-color: $light-cream;
}


</style>