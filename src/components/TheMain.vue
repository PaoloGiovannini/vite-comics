<script>
    export default {
      name: "TheMain"
    }

</script>
    
<template>
  <main>
    <div class="wrap-up">
      <div class="container">aggiungere contenuto</div>
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
  padding: 60px 0px;
}

.wrap-down{
  background-color: $color-hover;

  .container{
    padding: 40px 0px;

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