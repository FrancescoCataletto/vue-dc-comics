<template>
  
    <footer>
            <!-- sezione con logo e i vari link -->
            <div class="container">
                <div id="footer-top">
                <!-- div con i link -->
                    <div id="footer-links">
                        <ul>
                            <li style="color:aqua"><h3>DC COMICS</h3></li>
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
                        </ul>
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
                        <p>ICONE</p>
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

#footer-bottom{
    height: 100px;
    background-color: rgb(48, 48, 48);
    @include center;
    div:first-child{
        @include space-between;
        #socials{
            @include center;
        }
    }
    button{
        color: white;
        background-color: rgb(48, 48, 48);
        padding: 10px;
        font-size: 16px;
        border: 2px solid $brand-color;
        cursor: pointer;
    }
}
</style>