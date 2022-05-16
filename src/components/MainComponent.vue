<template>

  <main>
      <div id="card-main" class="container">
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
          <div id="card-box">
              <div id="single-card">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
              </div>
              <p>ACTION COMICS</p>
          </div>
      </div>
      <div id="load-more">
          <button>LOAD MORE</button>
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
@import "../assets/img/style/vars";

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
    width: calc(100% / 6 );
    padding-right: 10px;
    #single-card{
        margin-top: 50px;
        width: 100%;
        height: 200px;
        overflow: hidden;
    }
    p{
        padding-top: 10px;
    }
}

#load-more{
    width: 100%;
    text-align: center;
    button{
        margin: 30px;
        padding: 8px 30px;
        background-color: $brand-color;
        color: white;
        cursor: pointer;
    }
}
</style>