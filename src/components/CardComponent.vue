<template>

  <div id="single-card">
    <div>
      <img :src="cardImage" alt="IMMAGINE">
    </div>
    <p>{{cardTitle}}</p>
  </div>

</template>

<script>

export default {
    name: "CardComponent",
    props: {
        cardTitle: String,
        cardImage: String
    }
}
</script>

<style lang="scss" scoped>

#single-card{
  width: calc(100% / 6);
  padding-right: 10px;
  margin-top: 30px;
  cursor: pointer;
  div{
    height: 150px;
    overflow: hidden;
    img{
      width: 100%;
    }
  }
}

p{
    padding-top: 10px;
    color: white;
}
</style>