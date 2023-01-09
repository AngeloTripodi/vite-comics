<script>
export default {

}
</script>

<template>
    <header>
        <div class="headerContainer">
            <div class="logoSection">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <div class="navSection">
                <ul class="MyNav">
                    <li>CHARACTERS</li>
                    <li>COMICS</li>
                    <li>MOVIES</li>
                    <li>TV</li>
                    <li>GAMES</li>
                    <li>COLLECTIBLES</li>
                    <li>VIDEOS</li>
                    <li>FANS</li>
                    <li>NEWS</li>
                    <li>SHOP</li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss">
@use '../styles/general.scss' as *;

.headerContainer {
    display: flex;
    justify-content: space-around;

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
            padding-right: 1.5rem;
            font-weight: 700;
        }
    }

    .logoSection img {
        margin: .75rem 0;
    }

}
</style>