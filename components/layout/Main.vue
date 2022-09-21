<template>
  <main>
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
      width: 752px;
      text-align: center;
      margin: 0 auto 80px;
      h1{
        margin-bottom: 23px;
        @include font-heading-l;
      }
    }
    
</style>