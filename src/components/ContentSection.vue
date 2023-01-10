<script>
import comicsJson from '../db/dc-comics.json';

export default {
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
            <h1> --> Content Goes Here &lt;-- {{ comicsList[0] }} </h1>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.contentSection {
    background-color: #1c1c1c;
}

.content {
    padding: 2rem 0;
    color: white;
}
</style>