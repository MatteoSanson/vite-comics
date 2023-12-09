<script>
export default {
    name: 'MainLeftFooter',
    data() {
        return {
            dcComics: [
                {
                    name: 'Characters',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Comics',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Movies',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'TV',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Games',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Videos',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'News',
                    link: '#',
                    target: '_self',
                },
            ],
            shop: [
                {
                    name: 'Shop DC',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Shop DC Collectibles',
                    link: '#',
                    target: '_self',
                },
            ],
            dc: [
                {
                    name: 'Terms Of Use',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Privacy policy (New)',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Ad Choices',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Advertising',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Jobs',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Subscriptions',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Talent Workshops',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'CPSC Certificates',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Ratings',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Shop Help',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Contact Us',
                    link: '#',
                    target: '_self',
                },
            ],
            sites: [
                {
                    name: 'DC',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'MAD Magazine',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'DC Kids',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'DC Universe',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'DC Power Visa',
                    link: '#',
                    target: '_self',
                },
            ],
        }
    }
};
</script>

<template>
    <div class="menu-footer">
        <div class="nav-left">
            <h3>dc comics</h3>
            <ul>
                <li v-for="li in dcComics">
                    <a :href="li.link" :target="li.target">
                        {{ li.name }}
                    </a>
                </li>
            </ul>

            <h3>shop</h3>
            <ul>
                <li v-for="li in shop">
                    <a :href="li.link" :target="li.target">
                        {{ li.name }}
                    </a>
                </li>
            </ul>
        </div>

        <div class="nav-center">
            <h3>dc</h3>
            <ul>
                <li v-for="li in dc">
                    <a :href="li.link" :target="li.target">
                        {{ li.name }}
                    </a>
                </li>
            </ul>
        </div>

        <div class="nav-rightr">
            <h3>sites</h3>
            <ul>
                <li v-for="li in sites">
                    <a :href="li.link" :target="li.target">
                        {{ li.name }}
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>


<style scoped lang="scss">
@use '../../../styles/partials/variables.scss' as *;

.menu-footer {
    padding-top: 40px;
    width: 35%;
    display: flex;
    gap: 30px;

    h3 {
        text-transform: uppercase;
    }

    ul {
        list-style: none;

        li {
            font-size: 12px;
            line-height: 20px;
            color: gray;
        }

        li:first-child {
            padding-top: 10px;
        }

        a {
            text-decoration: none;
            color: gray;

            &:hover {
                color: $onhover;

                a {
                    color: $onhover;
                }
            }
        }


    }

}

.nav-left h3 {
    &:nth-of-type(2) {
        padding-top: 20px;
    }
}
</style>