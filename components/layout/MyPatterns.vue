<template>
    <section class="container"> 
        <div v-for="pattern in patterns" :key="pattern.class[0]"   :class="pattern.class">
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
                    name: 'Design',
                    class: ['design', 'img-l']
                },
                { 
                    img: '/pattern-ui-ux.svg',
                    name: 'UI/UX',
                    class: ['ui-ux', 'img-s']
                },
                { 
                    img: '/pattern-apps.svg',
                    name: 'Apps',
                    class: ['apps', 'img-s']
                },
                { 
                    img: '/pattern-photography.svg',
                    name: 'Photography',
                    class: ['photography', 'img-m']
                },
                { 
                    img: '/pattern-illustrations.svg',
                    name: 'Ilustrations',
                    class: ['ilustrations', 'img-m']
                },
                { 
                    img: '/pattern-motion-graphics.svg',
                    name: 'Motion Graphics',
                    class: ['graphics', 'img-m']
                }

            ] 
        }
    }

}
</script>

<style lang="scss" scoped>
    @import '~/assets/scss/main';

    section{
        height: 364px;
        display: grid;
        margin-bottom: 136px;
        grid-template-columns: repeat(6, 1fr);
        grid-template-rows: repeat(2, 1fr);
        grid-template-areas: 
        "design design ui-ux apps photography photography"
        "design design ilustrations ilustrations graphics graphics";
        gap: 24px;

        div{
            padding: 24px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;

            img{   
                align-self: end;

                &.img-s{
                    width: 64px;
                    height: 64px;
                }
                &.img-m{
                    width: 128px;
                    height: 64px;
                }
                &.img-l{
                    width: 128px;
                    height: 192px;
                }
            }

            p{
                color: #ffffff;
                font-weight: 700;
                font-size: 24px;
                line-height: 30px;
                font-style: normal;
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

</style>