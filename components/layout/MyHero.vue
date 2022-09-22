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

    section{
      margin-top: 100px;
      display: flex;
      flex-direction: column;
      align-items: center;
      img{
        width: 300px;
        height: 300px;
      }

      div{
        margin-top: 40px;
        display: flex;
        flex-direction: column;
        align-items: center;
        h2{
          @include mobile-font-heading-m ;
          text-align: center;
        }
        p{
          margin-top: 24px;
          text-align: center;
        }
        button{
          margin-top: 24px;
        }
      }
    }
  
  @media (min-width: 768px){
    .container{
      padding: 0px;
    }

    section{
      width: 772px;
      margin-left: auto;
      margin-right: auto;
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 69px;

      img{
        width: 364px;
        height: 364px;
      }
      
      div{
        width: 339px;
        align-items: start;
        h2{
          text-align: initial;
        }
        p{
          @include tablet-font-body;
          text-align: initial;
        }
      }
    }
  }

  @media (min-width: 1440px){

    section{
      margin-top: 136px;
      width: 1110px;
      gap: 125px;

      img{
        width: 445px;
        height: 445px;
      }
      
      div{
        width: 540px;
        h2{
          @include desktop-font-heading-m ;
        }
        p{
          margin-top: 34px;
          @include desktop-font-body;
        }
        button{
          margin-top: 32px;
        }
      }
    }
  }

</style>