<template>
  <main class="container">
      <h1>Design solutions made easy</h1>
      <p>With over ten years of experience in various design disciplines, I'm your one-stop shop for your design needs.</p>
    </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main';

main{
  margin-top: 32px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;

  h1{
    @include mobile-font-heading-l;
  }

  p{
    width: 285px;
    margin-top: 16px;    
  }
}

@media (min-width: 768px) {
  main {
    margin-top: 64px;

    h1{
      @include tablet-font-heading-l;
    }

    p{
      width: 573px;
      margin-top: 27px;
      @include tablet-font-body;
      
    }
  }
}

@media (min-width: 1440px) {
  main {
    margin-top: 66px;

    h1{
      @include desktop-font-heading-l;
    }

    p{
      width: 730px;
      margin-top: 23px;
      @include desktop-font-body;
      
    }
  }
}
    
</style>