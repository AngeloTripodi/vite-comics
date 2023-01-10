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
        <div class="currentCategories wrapper">
            <div class="currentElement">CURRENT SERIES</div>
        </div>
        <div class="content wrapper">
            <div class="comicElement" v-for="comic in comicsList">
                <CardComponent :imgPath="comic.thumb" :comicsType="comic.type" :comicsSeries="comic.series"
                    :price="comic.price" />
            </div>
        </div>
        <div class="buttonSection wrapper">
            <button id="loadMore">LOAD MORE</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.contentSection {
    background-color: #1c1c1c;

    .content {
        padding: 4rem 0 2rem 0;
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


    .buttonSection {
        display: flex;
        justify-content: center;

        & #loadMore {
            font-weight: bold;
            color: white;
            background-color: #1374ed;
            border: none;
            padding: .75rem 3rem;
            margin: .5rem 0 1.5rem 0;
        }

    }

    .currentCategories {
        max-width: 1230px;
    }

    .currentElement {
        position: absolute;
        top: 512px;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 225px;
        height: 50px;
        text-align: center;
        font-size: 2rem;
        font-weight: bold;
        color: white;
        background-color: #1374ed;
    }


}
</style>