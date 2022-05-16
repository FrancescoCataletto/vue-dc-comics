<template>
    <div>
        <div id="single-card">
          <img :src="cardImage" alt="IMMAGINE">
        </div>
        <p>{{cardTitle}}</p>
    </div>
</template>

<script>
export default {
    props: {
        cardTitle: String,
        cardImage: String
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/img/style/global.scss";


</style>