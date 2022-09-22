<template>
    <section class="container"> 
        <div v-for="pattern in patterns" :key="pattern.class"   :class="pattern.class">
            <img :src="pattern.img" :alt="pattern.name">
            <p>{{pattern.name}}</p>
        </div>
    </section>
</template>

<script>
export default {
    data(){
        return {
            patterns: [
                { 
                    img: '/pattern-graphic-design.svg',
                    name: 'Graphic Design',
                    class: 'design'
                },
                { 
                    img: '/pattern-ui-ux.svg',
                    name: 'UI/UX',
                    class: 'ui-ux',
                },
                { 
                    img: '/pattern-apps.svg',
                    name: 'Apps',
                    class: 'apps',
                },
                { 
                    img: '/pattern-photography.svg',
                    name: 'Photography',
                    class: 'photography',
                },
                { 
                    img: '/pattern-illustrations.svg',
                    name: 'Ilustrations',
                    class: 'ilustrations'
                },
                { 
                    img: '/pattern-motion-graphics.svg',
                    name: 'Motion Graphics',
                    class: 'graphics',
                }

            ] 
        }
    }

}
</script>

<style lang="scss" scoped>
    @import '~/assets/scss/main';

    section{
        margin-top: 32px;
        height: 1164px;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: repeat(6, 1fr);
        grid-template-areas: 
        "design       design"
        "design       design"
        "ui-ux        apps"
        "ilustrations ilustrations"
        "photography  photography"
        "graphics     graphics";
        gap: 24px;

        div{
            padding: 24px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;

            img{   
                align-self: end;
            }

            p{
                color: #ffffff;
                font-weight: 700;
                font-size: 24px;
                line-height: 30px;
            }
        }
    }

    .design{
        background-color: $galactic-blue;
        grid-area: design;
    }

    .ui-ux{
        background-color: $summer-yellow;
        grid-area: ui-ux;
    }
    .apps{
        background-color: $pink;
        grid-area: apps;
    }
    .photography{
        background-color: $cyan;
        grid-area: photography;
    }
    .ilustrations{
        background-color: $light-red;
        grid-area: ilustrations;
    }
    .graphics{
        background-color: $dark-purple;
        grid-area: graphics;
    }

    @media (min-width:768px) {
        section{
            margin-top: 64px;
            height: 690px;
            grid-template-columns: repeat(4, 1fr);
            grid-template-rows: repeat(3, 1fr);
            grid-template-areas: 
            "design       design      ui-ux        apps"
            "design       design      ilustrations ilustrations"
            "photography  photography graphics     graphics"
        }
    }

    @media (min-width:1440px) {
        section{
            margin-top: 80px;
            height: 364px;
            grid-template-columns: repeat(6, 1fr);
            grid-template-rows: repeat(2, 1fr);
            grid-template-areas: 
            "design design ui-ux        apps         photography  photography"
            "design design ilustrations ilustrations graphics     graphics"
        }
    }
</style>