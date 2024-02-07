<script>
export default {
    data() {
        return {
            menu: [
                {
                    sectionName: 'DC COMICS',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    sectionName: 'SHOP',
                    content: [
                        {
                            text: 'Shop DC',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Shop DC collectibles',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                },
                {
                    sectionName: 'DC',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Videos',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'News',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                }, {
                    sectionName: 'SITES',
                    content: [
                        {
                            text: 'Characters',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Comics',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Movies',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'TV',
                            link: '#',
                            target: '_blank'
                        },
                        {
                            text: 'Games',
                            link: '#',
                            target: '_blank'
                        }
                    ]
                }
            ]
        }
    }
}

</script>

<template>
    <div class="container">
        <nav>
            <ul v-for="element in menu">
                <li class="liHeader">{{ element.sectionName }}</li>
                <li class="lilinks" v-for="listItem in element.content"><a :href="listItem.link"
                    :target="listItem.target">{{ listItem.text }}</a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
nav {
    color: white;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    max-height: 500px;
    font-size: 23px;
    padding-top: 20px;
    padding-bottom: 40px;

    ul {
        padding-left: 70px;

        .liHeader {
            font-size: 23px;
            font-weight: bold;
            padding-bottom: 8px;
        }

        .lilinks a {
            font-size: 19px;
            color: $greyfooter;

            &:hover {
                text-decoration: underline;
            }
        }
    }
}
</style>