<script>
export default {

}
</script>

<template lang="">
    <div class="main">
        <div class="m-container">
             Content here
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/generals.scss' as *;
@use '../styles/partials/variables' as *;

.main {
    background-color: black;

    .m-container {
        width: 1200px;
        height: 200px;
        margin: 0 auto;
        color: white;
    }
}
</style>