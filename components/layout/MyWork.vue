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
    margin-top: 100px;

    h3{
        text-align: center;
        @include mobile-font-heading-s;
    }

    .slider{
        margin-top: 32px;
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        gap: 15px;
        overflow: auto;

        img{
            width: 270px;
            height: 180px;
            border-radius: 8px;
        }
    }

    .slider-controls{
        margin-top: 32px;
        display: flex;
        justify-content: center;

        button{
            margin: 0 8px;
        }
    }   
}

@media (min-width: 768px){
    section {
        margin-top: 138px;
        h3{
            @include tablet-font-heading-s;
        }
        .slider{
            margin-top: 56px;
            gap: 30px;
            img{
                width: 540px;
                height: 360px;
            }
        }
        .slider-controls{
            margin-top: 56px;
            button{
                margin: 0 8px;
            }
        }  
    }    
}

@media (min-width: 1440px){
    section {
        margin-top: 88px;
        h3{
            @include desktop-font-heading-s;
        }  
    }    
}

</style>