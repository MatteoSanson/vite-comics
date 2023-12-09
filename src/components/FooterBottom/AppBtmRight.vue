<script>
export default {
    name: 'BtmFooterRight',
    data() {
        return {
            links: [
                {
                    name: 'Facebook',
                    img: '/img/footer-facebook.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Twitter',
                    img: '/img/footer-twitter.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'YouTube',
                    img: '/img/footer-youtube.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Pinterest',
                    img: '/img/footer-pinterest.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Periscope',
                    img: '/img/footer-periscope.png',
                    link: '#',
                    target: '_self',
                },
            ]
        }
    }
};
</script>

<template>
    <div class="container">
        <div class="left">
            <a href="#" target="_self">
                follow us
            </a>
        </div>

        <div class="right">
            <ul>
                <li v-for="li in links">
                    <div class="icon">
                        <a :href="li.link" :target="li.target">
                            <img :src="li.img" :alt="li.link">
                        </a>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../../styles/partials/variables.scss' as *;

.container {
    display: flex;
    gap: 15px;
    align-items: center;

    a {
        text-decoration: none;
        color: inherit;
        display: inline-block;
    }
}

.left {
    text-transform: uppercase;
    color: $onhover;

    a:hover {
        color: $primary;
    }
}

.right {
    ul {
        display: flex;
        list-style: none;
        gap: 15px;

        .icon {
            width: 30px;
            height: 30px;
            border-radius: 50%;

            img {
                display: block;
                object-fit: contain;
                width: 100%;
            }

            &:hover {
                background-color: $onhover;
            }
        }
    }
}
</style>