<script>
export default {
    name: 'Jumbotron',
    data() {
        return {
            dcList: [
                {
                    name: 'digital comics',
                    img: '/img/buy-comics-digital-comics.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'dc merchandise',
                    img: '/img/buy-comics-merchandise.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'subscription',
                    img: '/img/buy-comics-subscriptions.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'comic shop locator',
                    img: '/img/buy-comics-shop-locator.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'dc power visa',
                    img: '/img/buy-dc-power-visa.svg',
                    link: '#',
                    target: '_self',
                },
            ]
        }
    }
};
</script>

<template>
    <div class="jumbo">
        <div class="container">
            <ul>
                <li v-for="li in dcList" class="point">
                    <div class="logo">
                        <a :href="li.link" :target="li.target">
                            <img :src="li.img" :alt="li.name">
                        </a>
                    </div>
                    <div class="near-logo">
                        <a :href="li.link" :target="li.target">
                            {{ li.name.toUpperCase() }}
                        </a>
                    </div>
                </li>

            </ul>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../../styles/partials/variables.scss' as *;

.jumbo {
    background-color: $onhover;

    a {
        text-decoration: none;
        color: $primary;

        &:hover {
            color: gainsboro;
        }
    }
}

.container {
    width: 80%;
    height: 150px;
    margin: 0 auto;
    display: flex;
    align-items: center;

    ul {
        width: 100%;
        list-style: none;
        display: flex;
        justify-content: space-around;
    }
}

.point {
    display: flex;
    align-items: center;
    gap: 15px;
}

.logo {
    width: 40px;
    height: 40px;

    a img {
        width: 100%;
        height: 100%;
        object-fit: contain;
        display: block;
    }
}
</style>