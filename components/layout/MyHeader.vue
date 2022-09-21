<template>
  <header>
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
    margin-bottom: 66px;
  }

</style>