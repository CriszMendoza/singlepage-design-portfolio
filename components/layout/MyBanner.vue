<template>
    <section class="container">
        <div class="banner">
            <div class="content">
                <h2>Book a call with me</h2>

                <p>I'd love to have a chat to see how I can help you. The best first step is for us to discuss your project during a 
                free consultation. Then we can move forward from there.</p>
            </div>
            <base-button type='secondary' title='Free Consultation'/>
        </div>
    </section>
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
@import '~/assets/scss/main';

section{
    margin: 100px 0 40px;
    .banner{
        background-color: $black;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 48px 0;
        
        .content{
            width: 295px;
            text-align: center;
            h2{
                @include mobile-font-heading-m;
                color: $light-cream;
            }
            p{
                margin-top: 24px;
            }
        }

        button{
            margin-top: 24px;
        }
    }
}

@media (min-width: 768px){
    section{
        margin: 120px 0 56px;
        .banner{
            padding: 60px 0;
            flex-direction: row;
            justify-content: space-around;
            .content{
                width: 540px;
                h2{
                    @include tablet-font-heading-m;
                    color: $light-cream;
                }
                p{
                    margin-top: 26px;
                }
            }
            
            button{
                    margin-top: 26px;
            }
        }
    }
}

@media (min-width: 1440px){
    section{
        margin-top: 88px;
        .banner{
            padding: 80px 0;
            .content{
                width: 540px;
                text-align: initial;
                h2{
                    @include desktop-font-heading-m;
                    color: $light-cream;
                }
                p, button{
                    margin-top: 26px;
                }
            }
        }
    }
}
</style>