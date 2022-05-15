<template>
    <section>
        <div class="container">
            <div id="floater">
                <a v-for="(link, index) in floaterArr" 
                :key="`floater${index}`" 
                href="link.href"><img :src="require(`../assets/img/buy-${link.url}`)" alt="LOGO"><span>{{link.text}}</span></a>
            </div>
        </div>
    </section>
  
</template>

<script>
export default {
    name: "FloatingComponent",
    data(){
        return{
            floaterArr: [
                {
                    href: "#",
                    url: "comics-digital-comics.png",
                    text: "DIGITAL COMICS"
                },
                {
                    href: "#",
                    url: "comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {
                    href: "#",
                    url: "comics-shop-locator.png",
                    text: "SUBSCRIPTION"
                },
                {
                    href: "#",
                    url: "comics-subscriptions.png",
                    text: "COMIC SHOP LOCATOR"
                },
                {
                    href: "#",
                    url: "dc-power-visa.svg",
                    text: "DC POWER VISA"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/global.scss";


section{
    height: 200px;
    background-color: rgb(2, 130, 249);
}
#floater{
    height: 200px;
    width: 90%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    a{
        display: flex;
        align-items: center;
    }
    img{
        height: 40px;
        padding-right: 5px;
    }
    span{
        display: inline-block;
        font-size: 12px;
        color: white;
    }
}
</style>