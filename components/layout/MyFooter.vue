<template>
    <footer class="container">
        <div>
            <h2>Book a call with me</h2>

            <p>I'd love to have a chat to see how I can help you. The best first step is for us to discuss your project during a 
            free consultation. Then we can move forward from there.</p>
        </div>

        <base-button type='secondary' title='Free Consultation'/>
    </footer>
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

footer{
    height: 320px;
    margin: 88px 0px 56px;
    background-color: $black;
    display: flex;
    justify-content: space-between;
    align-items: center;

    div{   
        width: 640px; 
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

</style>