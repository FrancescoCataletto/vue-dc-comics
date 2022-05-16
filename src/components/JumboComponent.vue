<template>
  <div id="jumbo">
    <div id="current-series">
      <p>CURRENT SERIES</p>
    </div>
  </div>
</template>

<script>
export default {
    name: "JumboComponent"
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/vars";

#jumbo{
    height: 400px;
    background-image: url("../assets//img/jumbotron.jpg");
    background-size: cover;
    position: relative;
}

#current-series{
  position: absolute;
  color: white;
  padding: 10px 20px;
  background-color: $brand-color;
  bottom: -20px;
  left: 210px;
}
</style>