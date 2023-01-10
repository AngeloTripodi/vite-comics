<script>
import comicsJson from '../db/dc-comics.json';
import CardComponent from './contentComponent/CardComponent.vue';

export default {
    name: 'contentSection',
    components: {
        CardComponent,
    },

    data() {
        return {
            comicsList: comicsJson,
        }
    },
}
</script>

<template>
    <section class="contentSection">
        <div class="content wrapper">
            <div class="comicElement" v-for="comic in comicsList">
                <CardComponent :imgPath="comic.thumb" :comicsType="comic.type" :comicsSeries="comic.series"
                    :price="comic.price" />
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
.contentSection {
    background-color: #1c1c1c;

    .content {
        padding: 2rem 0;
        color: white;
        display: flex;
        flex-wrap: wrap;
        max-width: 1230px;

    }

    .comicElement {
        display: flex;
        flex-wrap: wrap;
        margin: 0 auto;
        padding: 0 5px;
    }
}
</style>