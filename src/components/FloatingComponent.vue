<template>
    <section>
        <div class="container">
            <div id="floater">
                <a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""></a><span>DIGITAL COMICS</span>
                <a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt=""></a><span>DC MERCHANDISE</span>
                <a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt=""></a><span>SUBSCRIPTION</span>
                <a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt=""></a><span>COMIC SHOP LOCATOR</span>
                <a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt=""></a><span>DC POWER VISA</span>
            </div>
        </div>
    </section>
  
</template>

<script>
export default {
    name: "FloatingComponent"
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
    img{
        height: 40px;
    }
    span{
        font-size: 12px;
        color: white;
    }
}
</style>