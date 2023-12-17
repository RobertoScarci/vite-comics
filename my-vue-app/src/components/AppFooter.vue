<template>
    <footer>
        <div class="upperFooter">
            <div class="wrapper">
                <div class="column">
                    <h2>DC Comics</h2>
                    <ul class="firstUl">
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h2>Shop</h2>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="column">
                    <h2>DC</h2>
                    <ul>
                        <li>Terms of Use</li>
                        <li>Privacy policy(New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="column">
                    <h2>Sites</h2>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>Ad Choices</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="bottomFooter">
            <div class="wrapper">
                <button>
                    sign-up now!
                </button>
                <div class="socials">
                    <div class="text">Follow us</div>
                    <span class="iconWrapper">
                        <i class="fa-brands fa-facebook-f"></i>
                    </span>
                    <span class="iconWrapper">
                        <i class="fa-brands fa-twitter"></i>
                    </span>
                    <span class="iconWrapper">
                        <i class="fa-brands fa-youtube"></i>
                    </span>
                    <span class="iconWrapper">
                        <i class="fa-brands fa-pinterest-p"></i>
                    </span>
                    <span class="iconWrapper">
                        <i class="fa-solid fa-location-dot"></i>
                    </span>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
</script>

<style lang="scss">
    @use "../styles/partials/variables" as *;
    @use "../styles/partials/mixins" as *;
    footer .upperFooter {
        background-image: url(../assets/footer-bg.jpg);
        background-position: left;
        background-size: cover;
        div.wrapper {
            height: 100%;
            width: 90%;
            margin-left: 6rem;
            @include flex();
            div.column {

                ul {
                    list-style: none;
                    color: $text-color;
                    li {
                        margin-bottom: 0.5rem;
                        font-size: 0.8rem;
                    }
                    li:hover{
                        color: white;
                    }
                }
                .firstUl {
                    margin-bottom: 1.5rem;
                }
            }
            h2 {
                color: white;
                text-transform: uppercase;
                margin-bottom: 1rem;
                margin-left: 2.4rem;
            }
        }
    }
    footer .bottomFooter {
        padding: 2rem 0;
        background-color: $secondary-color;
        .wrapper {
            width: 80%;
            height: 100%;
            margin: 0 auto;
            @include flex(row, space-between, center);
            button {
                padding: 1rem .5rem;
                background-color: transparent;
                border: 2px solid $main-color;
                text-transform: uppercase;
                color: white;
                font-weight: 600;
                font-size: 1.3rem;
                &:hover {
                    color: $main-color;
                    opacity: 0.8;
                }
            }
            div.socials {
                @include flex();
                .text {
                    text-transform: uppercase;
                    color: $main-color;
                    font-size: 1.3rem;
                    font-weight: 600;
                    margin-right: 2rem;
                    @include flex(row, center, center);
                }
                .iconWrapper {
                    width: 30px;
                    height: 30px;
                    margin-right: .8rem;
                    border-radius: 50%;
                    background-color: $text-color;
                    @include flex(row, center, center);
                    color: $secondary-color;
                }
                .iconWrapper:hover{
                    background-color: rgb(228, 228, 228);
                }
            }
        }
    }
</style>