<script>
export default {
    props: {
        comic: Object,
    }

}
</script>

<template lang="">
    <div class="comic-card" :key="index">
        <img :src="comic.thumb">
        <h3>{{ comic.series }}</h3>
    </div>
</template>

<style lang="scss">
@use '../styles/generals.scss' as *;
@use '../styles/partials/variables' as *;

.main {
    background-color: black;

    .m-container {
        width: 1200px;
        margin: 0 auto;
        color: white;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;

        .comic-card {
            width: calc(100% / 6 - 40px);
            margin: 20px 20px;

            img {
                max-width: 100%;
                aspect-ratio: 1 / 1;
                object-fit: cover;
                object-position: 50% 0%;
                margin-bottom: 10px;
            }

            h3 {
                @include white_title
            }
        }
    }
}
</style>