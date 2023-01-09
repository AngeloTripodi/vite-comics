<script>
export default {

}
</script>

<template>
    <footer>
        <section class="wrapper">
            <div class="links">
                <div class="link1">
                    a
                </div>
                <div class="link2">
                    a
                </div>
                <div class="link3">
                    a
                </div>
            </div>
            <div class="imgBackground">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </section>
    </footer>
</template>

<style lang="scss">
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    padding: 2rem 0;
    overflow: hidden;
}

.wrapper {
    display: flex;
    justify-content: space-between;
}

.imgBackground img {
    margin: -130px;
}
</style>