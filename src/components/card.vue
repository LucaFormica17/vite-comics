<script>
export default {
    props: {
        comic: Object,
    },
}
</script>

<template lang="">
    <div class="card">
        <img :src="comic.thumb" alt="comic">
        <p>{{comic.series}}</p>
    </div>
</template>

<style lang="scss" scoped>
    @use './styles/partials/variables.scss' as*;

    .card{
            color: white;
            margin: 5px;
            width: calc(100% / 6 - 10px);

            &:hover{
                opacity: 0.5;
                cursor: pointer;
            }

            img{
                width: 100%;
                height: 200px;
                object-fit: cover;
            }
        }
</style>