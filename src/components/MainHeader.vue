<script>
export default {

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
                    <li>CHARACTERS</li>
                    <li class="active">COMICS</li>
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
            padding-right: 1.5rem;
            font-weight: 700;
            cursor: pointer;

            &.active,
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