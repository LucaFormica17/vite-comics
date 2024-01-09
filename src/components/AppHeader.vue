<script>
export default {
    data() {
        return {
            links: ['character','comics','movies','tv','games','collectibles','videos','fans','news','shop']
        }
    }
    
}
</script>

<template lang="">
    <div>
        <header>
            <div class="container">
                <div class="navbar">
                    <div class="logo">
                        <img src="../assets/img/dc-logo.png" alt="header-logo">
                    </div>
                    <ul>
                        <li v-for="(link, index) in links">
                            <a href="#" :class="index == 1 ? 'active' : ''">{{link}}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </header>
    </div>
</template>

<style lang="scss" scoped>
    @use './styles/partials/variables.scss' as *;

    .navbar{
        display: flex;
        justify-content: space-between;
        padding: 20px 0;

        ul{
            display: flex;

            li{
                margin: 0 5px;
                line-height: 100px;

                a{
                    font-size: 13px;
                    font-weight: 600;
                    text-transform: uppercase;
                    color: black;
                    position: relative;
                    display: block;

                    &.active,
                    &:hover{
                        color: $main_color;

                        &::after{
                            content: '';
                            position: absolute;
                            bottom: 0;
                            left: 0;
                            height: 5px;
                            width: 100%;
                            background-color: $main_color;
                        }
                    }
                }
            }
        }
    }
</style>