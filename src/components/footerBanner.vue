<script>
export default {
    
}
</script>

<template lang="">
    <div class="bg-grey">
        <div class="container">
            <div>
                <button>
                    <p>SIGN-UP NOW</p>
                </button>
            </div>
            <div class="social-links">
                <h3>FOLLOW US</h3>
                <img src="../assets/img/footer-facebook.png" alt="fb">
                <img src="../assets/img/footer-twitter.png" alt="twitter">
                <img src="../assets/img/footer-youtube.png" alt="yt">
                <img src="../assets/img/footer-pinterest.png" alt="pint">
                <img src="../assets/img/footer-periscope.png" alt="peri">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables.scss' as*;

.bg-grey{
    background-color: rgb(48, 48, 48);

    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px 0;

        button{
            background-color: transparent;
            border: $main_color 1px solid;

            p{
                color: white;
                padding: 10px;
                font-weight: 600;
            }
        }

        .social-links{
            display: flex;
            align-items: center;

            h3{
                color: $main_color;
                font-weight: 600;
                margin: 10px;
            }

            img{
                margin: 0 5px;
            }
        }
    }
}
    
</style>