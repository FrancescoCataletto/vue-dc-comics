<template>
  
    <footer>
            <!-- sezione con logo e i vari link -->
            <div class="container">
                <div id="footer-top">
                <!-- div con i link -->
                    <div id="footer-links">
                        <div>
                            <ul>
                                <li>
                                    <h3>DC COMICS</h3>
                                </li>
                                <li>
                                    <a href="#">Characters</a>
                                </li>
                                <li>
                                    <a href="#">Comics</a>
                                </li>
                                <li>
                                    <a href="#">Movies</a>
                                </li>
                                <li>
                                    <a href="#">TV</a>
                                </li>
                                <li>
                                    <a href="#">Games</a>
                                </li>
                                <li>
                                    <a href="#">Videos</a>
                                </li>
                                <li>
                                    <a href="#">News</a>
                                </li>
                                <li>
                                    <h3>SHOP</h3>
                                </li>
                                <li>
                                    <a href="#">Shop DC</a>
                                </li>
                                <li>
                                    <a href="#">Shop DC Collectibles</a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li>
                                    <h3>DC</h3>
                                </li>
                                <li>
                                    <a href="#">Terms of Use</a>
                                </li>
                                <li>
                                    <a href="#">Privacy policy(New)</a>
                                </li>
                                <li>
                                    <a href="#">Ad Choices</a>
                                </li>
                                <li>
                                    <a href="#">Advertising</a>
                                </li>
                                <li>
                                    <a href="#">Jobs</a>
                                </li>
                                <li>
                                    <a href="#">Subscriptions</a>
                                </li>
                                <li>
                                    <a href="#">Talent Workshops</a>
                                </li>
                                <li>
                                    <a href="#">CPSC Certificates</a>
                                </li>
                                <li>
                                    <a href="#">Ratings</a>
                                </li>
                                <li>
                                    <a href="#">Shop Help</a>
                                </li>
                                <li>
                                    <a href="#">Contact Us</a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li>
                                    <h3>SITES</h3>
                                </li>
                                <li>
                                    <a href="#">DC</a>
                                </li>
                                <li>
                                    <a href="#">MAD Magazine</a>
                                </li>
                                <li>
                                    <a href="#">DC Kids</a>
                                </li>
                                <li>
                                    <a href="#">DC Universe</a>
                                </li>
                                <li>
                                    <a href="#">DC Power Visa</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                <!-- div con il logo grande -->
                    <div id="big-logo">
                        <img src="../assets/img/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
            <!-- sezione con i social -->
            <div id="footer-bottom">
                <div class="container">
                    <button>SIGN-UP NOW!</button>
                    <div id="socials">
                        <p>FOLLOW US</p>
                        <div id="social-icons">
                            <a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook Logo"></a>
                            <a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter Logo"></a>
                            <a href="#"><img src="../assets/img/footer-youtube.png" alt="YouTube Logo"></a>
                            <a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest Logo"></a>
                            <a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope Logo"></a>
                        </div>
                    </div>
                </div>
            </div>
        
    </footer>

</template>

<script>
export default {
    name: "FooterComponent"
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/global.scss";
@import "../assets/img/style/utilities.scss";
@import "../assets/img/style/vars.scss";

footer{
    height: 500px;
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    background-position: center;
    li{
        @include menu-style;
        padding: 1px 0;
        &:hover{
            text-decoration: underline
        }
        a{
            @include link-underline;
            color: white;
        }
    }
}

#footer-top{
    @include space-between;
    height: 400px;
    overflow: hidden;
}

#footer-links{
    display: flex;
    ul{
        padding-right: 25px;
        li a{
            font-size: 10px;
            color: rgb(129, 133, 135);
        }
    }
    h3{
        color: white;
        padding-bottom: 5px;
    }
}

#big-logo{
    display: flex;
    justify-content: flex-end;
}

#big-logo img{
    width: 90%;
}

#footer-bottom{
    height: 100px;
    background-color: rgb(48, 48, 48);
    @include center;
    div:first-child{
        @include space-between;
        #socials{
            @include center;
            p{
                margin-right: 20px;
                color: $brand-color;
                font-weight: bold;
            }
        }
    }
    button{
        color: white;
        background-color: rgb(48, 48, 48);
        padding: 10px;
        font-size: 16px;
        border: 2px solid $brand-color;
        cursor: pointer;
        &:hover{
            background-color: $brand-color;
        }
    }
}

#social-icons img{
    padding: 0 5px;
}
</style>