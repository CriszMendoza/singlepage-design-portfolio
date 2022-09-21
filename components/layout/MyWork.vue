<template>
  <section>
    <h3>My Work</h3>
    <div class="slider">
        <article v-for="img in slides" :key="img">
            <img :src="img" alt="slide">
        </article>
    </div>
    <div class="slider-controls">
        <base-arrow direction='left'/><base-arrow direction='right'/>
    </div>
  </section>
</template>

<script>
import BaseArrow from '~/components/ux/BaseArrow'

export default {
    components: {
        BaseArrow
    },
    data(){
        return  {
            slides: [
                '/image-slide-1.jpg',
                '/image-slide-2.jpg',
                '/image-slide-3.jpg',
                '/image-slide-4.jpg',
                '/image-slide-5.jpg',
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main';

section{
    margin-top: 88px;

    h3{
        text-align: center;
        @include font-heading-s;
    }

    .slider{
        margin-top: 56px;
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        gap: 30px;
        overflow: hidden;

        img{
            border-radius: 18px;
        }
    }

    .slider-controls{
        margin-top: 56px;
        display: flex;
        justify-content: center;

        button{
            margin: 0 8px;
        }
    }
}

</style>