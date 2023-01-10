<script>
export default {
    data() {
        return {
            navMenuLinks: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    isActive: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'TV',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    isActive: false
                }

            ]
        }
    },

}
</script>

<template>
    <header>
        <div class="headerContainer wrapper">
            <div class="logoSection">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <div class="navSection">
                <ul class="MyNav">
                    <li v-for="navElement in navMenuLinks" :class="(navElement.isActive === true) ? 'active' : ''">{{
                        navElement.text
                    }}</li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.headerContainer {
    display: flex;
    justify-content: space-between;

    .navSection {
        display: flex;
        align-items: center;
    }

    ul {
        list-style-type: none;
        display: flex;
        align-content: center;
        padding: 0;

        li {
            margin-right: 1.5rem;
            font-weight: 700;
            cursor: pointer;
            line-height: 132px;

            &.active {
                border-bottom: 5px solid #53b0f0;
                color: #53b0f0;
            }

            &:hover {
                color: #53b0f0;
            }
        }

    }

    .logoSection img {
        margin: .75rem 0;
    }

}
</style>