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
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">COMICS</a>
                </li>
                <li>
                    <a href="#">MOVIES</a>
                </li>
                <li>
                    <a href="#">TV</a>
                </li>
                <li>
                    <a href="#">GAMES</a>
                </li>
                <li>
                    <a href="#">COLLECTIBLES</a>
                </li>
                <li>
                    <a href="#">VIDEOS</a>
                </li>
                <li>
                    <a href="#">FANS</a>
                </li>
                <li>
                    <a href="#">NEWS</a>
                </li>
                <li>
                    <a href="#">SHOP</a>
                </li>
              </ul>
          </div>
      </div>
  </header>

</template>

<script>
export default {
    name: "HeaderComponent"
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/utilities.scss";
@import "../assets/img/style/global.scss";

#header-box{
    @include space-between;
}

ul{
    display: flex;
    li{
        @include menu-style;
        padding: 10px 15px;
        font-size: 12px;
        font-weight: bold;
            a{
                @include link-underline;
                color: black;
            }
    }
}

</style>