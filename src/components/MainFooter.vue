<script>
export default {

}
</script>

<template>
    <footer>
        <section class="wrapper">
            <div class="links">
                <div class="link1">
                    <ul>
                        <li>DC COMICS</li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Collectibles</li>
                        <li>Videos</li>
                        <li>Fans</li>
                        <li>News</li>
                    </ul>
                    <ul>
                        <li>SHOP</li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="link2">
                    <ul>
                        <li>DC</li>
                        <li>Terms Of Use</li>
                        <li>Privacy Policy (New)</li>
                        <li>All Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="link3">
                    <ul>
                        <li>SITES</li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <div class="imgBackground">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </section>
    </footer>
    <section class="socialFooter">
        <div class="wrapper socialFooterWrapper">
            <div class="singUp">
                <button id="singUp">SING-UP NOW!</button>
            </div>
            <div class="socialIcon">
                <ul>
                    <li>
                        <h1>FOLLOW US</h1>
                    </li>
                    <li><img src="../assets/img/footer-facebook.png" alt="facebook"></li>
                    <li><img src="../assets/img/footer-twitter.png" alt="twitter"></li>
                    <li><img src="../assets/img/footer-youtube.png" alt="youtube"></li>
                    <li><img src="../assets/img/footer-pinterest.png" alt="pinterest"></li>
                    <li><img src="../assets/img/footer-periscope.png" alt="periscope"></li>

                </ul>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    padding: 2rem 0;
    overflow: hidden;
    color: white;

}

.links {
    display: flex;

    ul {
        list-style-type: none;

        li {
            color: grey;
            padding-right: 1.5rem;
            font-weight: 700;
            cursor: pointer;
            padding-bottom: .2rem;

            &:first-child {
                color: white;
                font-size: 1.5rem;
                padding-bottom: .75rem;
            }
        }

    }
}

.wrapper {
    display: flex;
    justify-content: space-between;
}

.imgBackground img {
    margin-top: -130px;
    margin-bottom: -130px;
}

.socialFooter {
    background-color: #303030;
    padding: 2rem 0;

    h1 {
        color: #1374ed;
        padding-right: 1rem;
    }

    #singUp {
        color: white;
        background-color: #303030;
        border: 3px solid #1374ed;
        padding: .5rem 1rem;
    }

    .socialIcon {
        display: flex;
        align-content: center;
    }

    & ul {
        list-style-type: none;
        display: flex;
        align-items: center;
    }

    & li {
        padding-left: 1rem;
    }
}
</style>