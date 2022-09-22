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

    .banner{
        height: 320px;
        margin: 88px 0px 56px;
        background-color: $black;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    .content{   
        width: 540px; 
        h2{
            color: $light-cream;
            @include font-heading-m;
            margin-bottom: 25px;
        }
        p{
            color: $light-cream;
            @include font-body-m;
        }
    }
}

@media (max-width: 768px) {
    section{
        .banner{
            height: 352px;
            flex-direction: column;
            justify-content: start;
            align-items: center;
            margin: 56px 0px 64px;
            .content{
                text-align: center;
                h2{
                    margin-top: 56px;
                    @include font-heading-s;
                }
            }
            button{
                margin-top: 25px;
            }
        }
    }  
}



</style>