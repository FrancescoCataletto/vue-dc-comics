<template>

  <header>
      <!-- container principale header -->
      <div id="header-box" class="container">
          <!-- div del logo -->
          <div>
              <img src="../assets/img/dc-logo.png" alt="Logo piccolo">
          </div>
          <!-- div del menu -->
          <div>
              <ul>
                <li v-for="(link, index)  in nameArr" 
                :key="`menu-${index}`">
                    <a href="link.href">{{link.link}}</a>
                </li>
              </ul>
          </div>
      </div>
  </header>

</template>

<script>
export default {
    name: "HeaderComponent",
    data(){
        return{
            nameArr: [
                {
                    link: "CHARACTERS",
                    href: "#"
                },
                {
                    link: "COMICS",
                    href: "#"
                },
                {
                    link: "MOVIES",
                    href: "#"
                },
                {
                    link: "TV",
                    href: "#"
                },
                {
                    link: "GAMES",
                    href: "#"
                },
                {
                    link: "COLLECTIBLES",
                    href: "#"
                },
                {
                    link: "VIDEOS",
                    href: "#"
                },
                {
                    link: "FANS",
                    href: "#"
                },
                {
                    link: "NEWS",
                    href: "#"
                },
                {
                    link: "SHOP",
                    href: "#"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/utilities.scss";
@import "../assets/img/style/global.scss";
@import "../assets/img/style/vars";

header{
    height: 150px;
    display: flex;
    align-items: center
}

#header-box{
    @include space-between;
    height: 150px;
}

ul{
    display: flex;
    li{
        @include menu-style;
        padding: 0 10px;
        font-size: 12px;
        font-weight: bold;
            a{
                @include link-underline;
                color: black;
                padding-bottom: 66px;
                &:hover{
                    color: $brand-color;
                    border-bottom: 3px solid $brand-color;
                }
            }
    }
}

</style>