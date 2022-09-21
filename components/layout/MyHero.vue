<template>
  <section class="container">

    <img src="/image-amy.webp" alt="Hero">

    <div>
        <h2>I'm Amy, and I'd love to work on your next project</h2>

        <p>I love working with others to create beautiful design solutions. I've designed everything from brand illustrations 
        to complete mobile apps. I'm also handy with a camera!</p>
            
        <BaseButton title="Free Consultation" type='secondary'/>
    </div>

  </section>
</template>

<script>
import BaseButton from '~/components/ux/BaseButton'

export default {
    components:{
        BaseButton
    }
}
</script>

<style lang="scss" scoped>
    @import '~/assets/scss/main';

    section {
        display: flex;
        justify-content: space-between;
        img{
            width: 445px;
            height: 445px;
        }
        div{
            width: 540px;
            display: flex;
            flex-direction: column;

            h2{
                margin-top: 70px;
                @include font-heading-m;
            }
            p{
                margin-top: 34px;
                margin-bottom: 32px;
            }
        }
    }

</style>