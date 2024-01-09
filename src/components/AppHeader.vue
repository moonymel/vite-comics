<script>
export default {
    data() {
        return {
            links: [
                {
                    label: 'Characters',
                    link: '...',
                    current: false
                },
                {
                    label: 'Comics',
                    link: '...',
                    current: true
                },
                {
                    label: 'Movies',
                    link: '...',
                    current: false
                },
                {
                    label: 'Tv',
                    link: '...',
                    current: false
                },
                {
                    label: 'Games',
                    link: '...',
                    current: false
                },
                {
                    label: 'Collectibles',
                    link: '...',
                    current: false
                },
                {
                    label: 'Videos',
                    link: '...',
                    current: false
                },
                {
                    label: 'Fans',
                    link: '...',
                    current: false
                },
                {
                    label: 'News',
                    link: '...',
                    current: false
                },
                {
                    label: 'Shop',
                    link: '...',
                    current: false
                },
            ]
        }
    }
}

</script>

<template lang="">
    <div class="container">
        <div class="row">
            <div class="left">
                <img src="../img/dc-logo.png">
            </div>
            <div class="right">
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :href="link.link" :alt="link.label" :class="link.current == true ? 'active' : ''">
                            {{ link.label }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/generals.scss' as *;
@use '../styles/partials/variables' as *;

.container {
    height: 80px;
    font-size: $min_text;
    width: 1200px;
    margin: 20px auto;
    font-family: Oswald;
    text-transform: uppercase;
    letter-spacing: 0.5px;

    img {
        height: 80px;
    }

    a {
        text-decoration: none;
        color: black;

        &.active {
            color: $light_blue;
            border-bottom: 4px solid $light_blue;
            padding-bottom: 44px;
        }
    }

    .row {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .right {
            text-align: right;
        }

        ul {
            list-style: none;
            display: flex;
        }

        li {
            padding: 0 20px;
        }
    }
}
</style>