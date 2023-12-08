<script>
export default {
    name: 'NavHeader',
    data() {
        return {
            menu: [
                {
                    nome: 'Characters',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Comics',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Movis',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Tv',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Games',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Collectibles',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Videos',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Fans',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'News',
                    link: '#',
                    target: '_self',
                },
                {
                    nome: 'Shop',
                    link: '#',
                    target: '_self',
                },
            ]
        }
    },
};
</script>

<template>
    <ul class="navHeader">
        <li v-for="li in menu">
            <a :href="li.link" :target="li.target">
                {{ li.nome.toUpperCase() }}
            </a>
        </li>
    </ul>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.navHeader {
    list-style: none;
    display: flex;
    justify-content: end;
}


li {
    position: relative;

    padding: 5px 10px;

    a {
        text-decoration: none;
        color: $header;
    }

    &:hover {
        color: $onhover;

        a {
            color: $onhover;
        }

        &::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -57px;
            width: 100%;
            height: 3px;
            background-color: $onhover;
        }
    }
}
</style>