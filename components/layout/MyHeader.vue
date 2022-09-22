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
  margin: 34px 0 66px;
  display: flex;
  justify-content: space-between;
}

@media (max-width: 768px){
  header{
    margin-bottom: 64px;
  }
}
</style>