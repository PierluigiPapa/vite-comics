<script>
export default {
    // STRUTTURA CLASSICA DI VUE 
    data() {
        return {
            links: [
                {
                    name: 'Facebook',
                    link: '#',
                    logo: 'img/footer-facebook.png',
                    target: '_blank'

                },
                {
                    name: 'Twitter',
                    link: '#',
                    logo: 'img/footer-twitter.png',
                    target: '_blank'

                },
                {
                    name: 'You-tube',
                    link: '#',
                    logo: 'img/footer-youtube.png',
                    target: '_blank'

                },
                {
                    name: 'Pinterest',
                    link: '#',
                    logo: 'img/footer-pinterest.png',
                    target: '_blank'

                },
                {
                    name: 'Periscope',
                    link: '#',
                    logo: 'img/footer-periscope.png',
                    target: '_blank'

                }
            ]
        }
    }
}

</script>

<template>
    <div class="container">
        <h3>FOLLOW US</h3>
        <nav>
            <ul>
                <li v-for="link in links">
                    <a :href="link.link" :target="link.target">
                        <img :src="link.logo" :alt="link.name">
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.container {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;

    h3 {
        color: $blue;
        white-space: nowrap;
    }

    ul {
        display: flex;
        justify-content: center;
        align-items: center;

        li {
            padding: 15px 10px;
        }
    }
}

</style>