<template>

  <main>
      <div id="card-main" class="container">
              <CardComponent v-for="(card, index) in cardArr"
                            :key="`card-${index}`"
                            :cardImage="card.thumb"
                            :cardTitle="card.series"/>
      </div>
      
      <div id="load-more">
          <button>LOAD MORE</button>
      </div>
  </main>

</template>

<script>
import CardComponent from "./CardComponent.vue";
import cardArr from "../assets/img/data/data.js";


export default {
    name: "MainComponent",
    components: { CardComponent },
    data(){
        return{
            cardArr
        }
    }
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