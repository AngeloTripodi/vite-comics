<script>
export default {
    name: 'CardComponent',
    props: {
        imgPath: String,
        comicsType: String,
        comicsSeries: String,
        price: String
    },
}
</script>

<template>
    <div class="card">
        <img :src="imgPath" alt="">
        <h2 class="comicsTitle">{{ comicsSeries }}</h2>
    </div>
</template>

<style lang="scss" scoped>
div.card {
    width: min-content;
    margin: 0 auto;
    padding-top: 1.5rem;
}

div.card img {
    width: 180px;
    height: 180px;
    object-fit: cover;
    object-position: top;
}

h2 {

    padding-top: .5rem;
    text-transform: uppercase;
    font-size: 1.3rem;
}
</style>