<script>
    export default {
        
    }
</script>
<template lang="">
    <div class="bg-blue">
        <div class="container">
            <div class="banner-card">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="image">
                <p>dc comics</p>
            </div>
            <div class="banner-card">
                <img src="../assets/img/buy-comics-merchandise.png" alt="image">
                <p>dc merchandaise</p>
            </div>
            <div class="banner-card">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="image">
                <p>subscription</p>
            </div>
            <div class="banner-card">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="image">
                <p>comic shop locator</p>
            </div>
            <div class="banner-card">
                <img class="svg" src="../assets/img/buy-dc-power-visa.svg" alt="image">
                <p>dc power visa</p>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    @use './styles/generals.scss';
    @use './styles/partials/variables.scss' as*;

    .bg-blue{
        background-color: $main_color;

        .container{
            display: flex;
            justify-content: space-between;

            .banner-card{
                display: flex;
                align-items: center;
                margin: 30px 0;

                img{
                    width: 25%;
                    
                    &.svg{
                        width: 100%;
                    }
                }

                p{
                    color: white;
                    text-transform: uppercase;
                    margin-left: 10px;
                }
            }
        }
    }
</style>