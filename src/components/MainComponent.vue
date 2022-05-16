<template>

  <main>
      <div id="card-main" class="container">
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              <p>ACTION COMICS</p>
          </div>
      </div>
  </main>

</template>

<script>
export default {
    name: "MainComponent"
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/global.scss";

main{
    background-color: rgb(28, 28, 28);
    p{
        color: white;
    }
}

#card-main{
    display: flex;
    flex-wrap: wrap;
}

#card-box{
    width: calc(100% / 6);
    padding: 10px;
    img{
        width: 100%;
        height: 250px;
    }
    p{
        padding-top: 5px;
    }
}
</style>