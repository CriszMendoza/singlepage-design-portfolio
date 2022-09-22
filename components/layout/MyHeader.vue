<template>
  <header class="container">
    <img src="/logo.svg" alt="Logo">
    <base-button title="Free Consultation" type='primary'/>
  </header>
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

header{
    display: flex;
    justify-content: space-between;

    img {
      width: 48px;
      height: 48px;
    }
  }

  @media (min-width: 768px) {
    header {
      img {
        width: 64px;
        height: 64px;
      }
      }
  }
</style>