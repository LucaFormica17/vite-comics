<script>
import blueBanner from './blueBanner.vue';
import footerBanner from './footerBanner.vue';
export default {
    
    components: {
        blueBanner,
        footerBanner
    }
}
</script>

<template lang="">
    <div>
        <blueBanner />
        <div class="bg-img">
            <div class="container">
                <div class="lists">
                    <div class="col">
                        <h3>dc comics</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h3>shop</h3>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>dc</h3>
                        <ul>
                            <li>Terms Of Us</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choice</li>
                            <li>Advertsing</li>
                            <li>Jobs</li>
                            <li>Subscrtions</li>
                            <li>Talnet Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>sites</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <footerBanner />
    </div>
</template>

<style lang="scss" scoped>
    @use './styles/partials/variables.scss' as*;

    .bg-img{
        background-image: url('../assets/img/footer-bg.jpg');
        
        .container{
            display: flex;
            justify-content: space-between;
            align-items: center;

            .lists{
                display: flex;
                
                .col{
                    margin: 0 5px;
                    h3{
                        color: white;
                        text-transform: uppercase;
                        margin: 10px 0;
                    }

                    li{
                        color: lightgrey;
                    }
                }
            }
        }
    }    
</style>