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
                                <li v-for="(link, index)  in DCComicsArr"
                                :key="`dc-comics${index}`">
                                    <a href="link.href">{{link.link}}</a>
                                </li>
                                <li>
                                    <h3>SHOP</h3>
                                </li>
                                <li v-for="(link, index)  in shopArr"
                                :key="`shop${index}`">
                                    <a href="link.href">{{link.link}}</a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li>
                                    <h3>DC</h3>
                                </li>
                                <li v-for="(link, index)  in DCArr"
                                :key="`DC${index}`">
                                    <a href="link.href">{{link.link}}</a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <ul>
                                <li>
                                    <h3>SITES</h3>
                                </li>
                                <li v-for="(link, index)  in sitesArr"
                                :key="`sites-arr${index}`">
                                    <a href="link.href">{{link.link}}</a>
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
    name: "FooterComponent",
    data(){
        return{
            DCComicsArr: [
                {
                    link: "Characters",
                    href: "#"
                },
                {
                    link: "Comics",
                    href: "#"
                },
                {
                    link: "Movies",
                    href: "#"
                },
                {
                    link: "TV",
                    href: "#"
                },
                {
                    link: "Games",
                    href: "#"
                },
                {
                    link: "Videos",
                    href: "#"
                },
                {
                    link: "News",
                    href: "#"
                }
            ],

            shopArr: [
                {
                    link:"Shop DC",
                    href: "#"
                },
                {
                    link:"Shop DC Collectibles",
                    href: "#"
                }
            ],

            DCArr: [
                {
                    link:"Terms of Use",
                    href: "#"
                },
                {
                    link:"Privacy policy(New)",
                    href: "#"
                },
                {
                    link:"Ad Choices",
                    href: "#"
                },
                {
                    link:"Advertising",
                    href: "#"
                },
                {
                    link:"Jobs",
                    href: "#"
                },
                {
                    link:"Subscriptions",
                    href: "#"
                },
                {
                    link:"Talent Workshops",
                    href: "#"
                },
                {
                    link:"CPSC Certificates",
                    href: "#"
                },
                {
                    link:"Ratings",
                    href: "#"
                },
                {
                    link:"Shop Help",
                    href: "#"
                },
                {
                    link:"Contact Us",
                    href: "#"
                }
            ],

            sitesArr: [
                {
                    link: "DC",
                    href: "#"
                },
                {
                    link: "MAD Magazine",
                    href: "#"
                },
                {
                    link: "DC Kids",
                    href: "#"
                },
                {
                    link: "DC Universe",
                    href: "#"
                },
                {
                    link: "DC Power Visa",
                    href: "#"
                }
            ]
        }
    }
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