<script>
    import ProductCard from './ProductCard.vue';

    export default {
      name: "TheMain",
      components: {
        ProductCard
      },
      data() {
    return {
        fumetti: [
  {
      "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
      "price": "$19.99",
      "series": "Action Comics",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
      "price": "$3.99",
      "series": "American Vampire 1976",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/ST_GH_Cv3_00311_DIGITAL.jpg?w=640",
      "price": "$16.99",
      "series": "Aquaman",
      "type": "graphic novel"
  },
  {
      "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640",
      "price": "$2.99",
      "series": "Batgirl",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/MS30A_Cv1_00111_DIGITAL.jpg?w=640", 
      "price": "$3.99",
      "series": "Batman",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
      "price": "$2.99",
      "series": "Batman Beyond",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
      "price": "$3.99",
      "series": "Batman/Superman",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
      "price": "$4.99",
      "series": "Batman/Superman Annual",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/DCConnect_35-CVR.jpg?w=640",
      "price": "$5.99",
      "series": "Batman: The Joker War Zone",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
      "price": "$6.99",
      "series": "Batman: Three Jokers",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/LP-ROTG_Cv1_00111_DIGITAL.jpg?w=640",
      "price": "$4.99",
      "series": "Batman: White Knight Presents: Harley Quinn",
      "type": "comic book"
  },
  {
      "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
      "price": "$16.99",
      "series": "Catwoman",
      "type": "graphic novel"
  }
]
    }
  }
    }
    

</script>
    
<template>
  <main>

    <div class="wrap-up">
      <div id="container-fumetti" class="container d-flex">
        <div v-for="(fumetto, index) in fumetti" class="card" :key="index">
            <ProductCard :image="fumetto.thumb" :title="fumetto.series"/>  
        </div>
      </div>
      <div class="loading">
        <span>LOAD MORE</span>
      </div>
    </div>

    <div>
      <div class="wrap-down">
        <div class="container d-flex space-around">
          <div class="d-flex flex-center">
            <img src="../assets/buy-comics-digital-comics.png" alt="digital comics">
            <span>DIGITAL COMICS</span>
          </div>
          <div class="d-flex flex-center">
            <img src="../assets/buy-comics-merchandise.png" alt="Merchandise">
            <span>DC MERCHANDISE</span>
          </div>
          <div class="d-flex flex-center">
            <img src="../assets/buy-comics-subscriptions.png" alt="subscription">
            <span>SUBSCRIPTION</span>
          </div>
          <div class="d-flex flex-center">
            <img src="../assets/buy-comics-shop-locator.png" alt="Comic shop locator">
            <span>COMIC SHOP LOCATOR</span>
          </div>
          <div class="d-flex flex-center">
            <img src="../assets/buy-dc-power-visa.svg" alt="DC power visa">
            <span>DC POWER VISA</span>
          </div>
        </div>
      </div>
      
    </div>
  </main> 
    
</template>
    
<style scoped lang="scss">
@use"../styles/partials/variables" as *;
.wrap-up{
  background-color: $bg-main;
  color: $text-main;
  padding: 30px 0px;

  & .loading{
      text-align: center;
      & span{
        font-weight: bold;
        background-color: $color-hover;
        padding: 10px 50px;
      }
    }
}

#container-fumetti{
  flex-wrap: wrap;
    & .card{
      width: calc(100% / 6);
      margin: 20px 0px;
      
    }
    
}

.wrap-down{
  background-color: $color-hover;

  .container{
    padding: 30px 0px;
    

    img{
      display: inline-block;
      width: 50px;
      vertical-align: middle;
    }
    span{
      vertical-align: middle ;
      color: $text-main;
      margin-left: 10px;
    }
  }

  
}

   
</style>