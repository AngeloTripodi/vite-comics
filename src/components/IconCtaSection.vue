<script>
export default {
    data() {
        return {
            ctaLinks: [
                {
                    text: 'DIGITAL COMICS',
                    url: '#',
                    img: 'buy-comics-digital-comics.png'

                },
                {
                    text: 'DC MERCHANDISE',
                    url: '#',
                    img: 'buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    url: '#',
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: '#',
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    url: '#',
                    img: 'buy-dc-power-visa.svg'
                }

            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(`../assets/img/${imgPath}`, import.meta.url).href;
        }
    },

}
</script>

<template>
    <section class="ctaSection">
        <div class="ctas wrapper">
            <ul>
                <li v-for="cta in ctaLinks"> <img :src="'src/assets/img/' + cta.img" :alt="cta.text"> {{ cta.text }}
                </li>
            </ul>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.ctaSection {
    background-color: #0282f9;
}

.ctas {
    padding: 2rem 0;
    color: white;


    ul {
        list-style-type: none;
        display: flex;
        justify-content: space-around;
        width: 100%;

    }

    li {
        display: flex;
        flex-direction: row;
        align-items: center;
        margin-left: 1rem;
        margin-right: 1rem;

        img {
            height: 55px;
            padding-right: 1rem;
        }




    }
}
</style>