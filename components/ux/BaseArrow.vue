<template>
  <button @click="submit">
    <img :src="directionRow" :alt="direction">
  </button>
</template>

<script>
export default {
    props: {
        direction: {
            type: String,
            require: true
        }
    },
    computed:{
        directionRow(){
            return this.direction === 'right' 
                ?  '/icon-arrow-right.svg' 
                : '/icon-arrow-left.svg' 
        }
    },
    methods: {
        submit(){
            this.$emit('submitButton')
        }
    }

}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main';

button{
    width: 64px;
    height: 64px;
    border-radius: 50%;
    border: none;
    background-color: $black;
    &:hover{
        background-color: $galactic-blue;
    }
}

img{
    height: 16px;
}
</style>