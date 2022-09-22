<template>
  <button @click="submit" :class="type">{{title}}</button>
</template>

<script>
export default {
    props: {
        title: {
            type: String,
            require: true
        },
        type: {
            type: String,
            require: true
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
        width: 176px;
        height: 44px;
        display: block;
        padding: 0;
        border: none;
        border-radius: 28px;
        cursor: pointer;
        @include font-button;
    }

    .primary{
        background-color: $black;
        &:hover{
            background-color: $galactic-blue;
        }
    }

    .secondary{
        background-color: $light-red;
        &:hover{
            background-color: $summer-yellow;
        }
    }

    @media (min-width: 768px) {
    button {
        width: 228px;
        height: 56px;
    }
  }

</style>