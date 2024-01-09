<script>
export default {
    data() {
        return {
            sections: [
                {
                    title: 'Digital Comics',
                    image: '../src/img/buy-comics-digital-comics.png'
                },
                {
                    title: 'DC Merchandise',
                    image: '../src/img/buy-comics-merchandise.png'
                },
                {
                    title: 'Subscription',
                    image: '../src/img/buy-comics-subscriptions.png'
                },
                {
                    title: 'Comic Shop Locator',
                    image: '../src/img/buy-comics-shop-locator.png'
                },
                {
                    title: 'DC Power Visa',
                    image: '../src/img/buy-dc-power-visa.svg'
                },
            ]
        }
    }

}
</script>

<template lang="">
    <div class="blue-line">
        <div class="b-container">
            <div class="section" v-for="(section, index) in sections">
                <img :src="section.image" :class="section.title == 'DC Power Visa' ? 'visa' : ''">
                {{ section.title }}
            </div>
        </div>
        
    </div>
</template>

<style lang="scss">
@use '../styles/generals.scss' as *;
@use '../styles/partials/variables' as *;

.blue-line {
    background-color: $light_blue;

    .b-container {
        width: 1200px;
        margin: 0 auto;
        color: white;
        display: flex;
        justify-content: space-between;

        .section {
            font-family: Montserrat;
            text-transform: uppercase;
            font-size: 14px;
            margin: 40px 0px;

            img {
                height: 50px;
                vertical-align: middle;
                margin-right: 10px;

                &.visa {
                    height: 35px;
                    margin-top: 10px;
                }
            }
        }

    }
}
</style>