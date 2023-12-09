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
                    <a :href="li.link" :target="li.target" class="flecs">
                        <div class="logo">
                            <img :src="li.img" :alt="li.name">
                        </div>
                        <div class="near-logo">
                            {{ li.name.toUpperCase() }}
                        </div>
                    </a>

                </li>

            </ul>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../../styles/partials/variables.scss' as *;

.jumbo {
    background-color: $onhover;
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

.point a.flecs {
    display: flex;
    align-items: center;
    gap: 15px;
}

a {
    text-decoration: none;
    color: $primary;
    transition: transform 0.3s ease-in-out;

    &:hover {
        color: gainsboro;
        transform: scale(1.2);
    }
}

.logo {
    width: 40px;
    height: 40px;

    img {
        width: 100%;
        height: 100%;
        object-fit: contain;
        display: block;
        transition: transform 0.3s ease-in-out;
    }
}
</style>