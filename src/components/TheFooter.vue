<script>
    export default {
      name: "TheFooter",
      data() {
        return {
            DcComics: [
            {
              text: "Characters",
              href: "#Characters",
            },
            {
              text: "Comics",
              href: "#Comics",
            },
            {
              text: "Movies",
              href: "#Movies",
            },
            {
              text: "TV",
              href: "#TV",
            },
            {
              text: "Games",
              href: "#Games",
            },
            {
              text: "Collectibles",
              href: "#Collectibles",
            },
            {
              text: "Videos",
              href: "#Videos",
            },
            {
              text: "Fans",
              href: "#Fans",
            },
            {
              text: "News",
              href: "#News",
            },
            {
              text: "Shop",
              href: "#Shop",
            },
            ],

            ShopDc:[
            {
              text: "Shop Dc",
              href: "#Shop-Dc",
            },
            {
              text: "Shop Dc Collectibles",
              href: "# Shop-Dc-Collectibles",
            }  
            ],

            DC:[
            {
              text: "Term Of Use",
              href: "#Term-Of-Use",
            },
            {
              text: "Privacy policy(new)",
              href: "#Privacy-policy(new)",
            },
            {
              text: "Ad Choices",
              href: "#Ad-Choices",
            },
            {
              text: "Advertising",
              href: "#Advertising",
            },
            {
              text: "Jobs",
              href: "#Jobs",
            },
            {
              text: "Subscriptions",
              href: "#Subscriptions",
            },
            {
              text: "Talent Workshops",
              href: "#Talent-Workshops",
            },
            {
              text: "CPSC Certificates",
              href: "#CPSC-Certificates",
            },
            {
              text: "Ratings",
              href: "#Ratings",
            },
            {
              text: "Shop Helps",
              href: "#Shop-Helps",
            },
            {
              text: "Contact Us",
              href: "#Contact-Us",
            }, 
            ],
            Sites:[
            {
              text: "DC",
              href: "#DC",
            },
            {
              text: "MAD Magazine",
              href: "#MAD-Magazine",
            },
            {
              text: "DC Kids",
              href: "#DC-Kids",
            },
            {
              text: "DC Universe",
              href: "#DC-Universe",
            },
            {
              text: "DC Power Visa",
              href: "#DC-Power Visa",
            },
            ]

        }
    }
      
    }

</script>
    
<template>
  <footer>

  
    <div class="wrap">
        <div class="container d-flex">
            <div>
                <h3>Dc Comics</h3>
                <ul>
                    <li v-for="item in DcComics">
                        <a :href="item.href">{{ item.text }}</a>
                    </li>
                    <h3>Shop</h3>
                    <ul>
                        <li v-for="item in ShopDc">
                            <a :href="item.href">{{ item.text }}</a>
                        </li>
                    </ul>
                 </ul>
            </div>
            <div>
                <h3>DC</h3>
                <ul>
                    <li v-for="item in DC">
                        <a :href="item.href">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
            <div class="sites">
                <h3>Sites</h3>
                <ul>
                    <li v-for="item in Sites">
                        <a :href="item.href">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
    <div class="wrapper">
      <div class="container-footer d-flex space-between flex-center">
        <div class="button-sign-up">
          <span>SIGN-UP NOW</span>
        </div>
      <div>
        <span class="follow">FOLLOW US</span>
        <img src="../assets/footer-facebook.png" alt="">
        <img src="../assets/footer-twitter.png" alt="">
        <img src="../assets/footer-youtube.png" alt="">
        <img src="../assets/footer-pinterest.png" alt="">
        <img src="../assets/footer-periscope.png" alt="">
      </div>
      </div>
    </div>
  </footer>
</template>
    
<style scoped lang="scss">
@use"../styles/partials/variables" as *;

.wrap{
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
      .container{
        background-image: url(../assets/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
        padding: 35px 0px;

        ul li{
          padding: 3px 0px;

          a{
            color:#959595;
          }   
        }

        .sites{
          margin-left: 10px;
        } 

        h3{
          color: $text-main;
          padding: 15px 0px;
        }
      }
}

.wrapper{
  background-color: $footer-bg;
  padding: 30px 0px;
  .container-footer{
  max-width: 1170px;
  margin: auto;

    .button-sign-up{
      color: $text-main;
      border: 3px solid $color-hover;
      padding: 15px 10px;
    }
    img{
      display: inline;
      vertical-align: middle;
      padding: 0px 7px;
    }

    .follow{
      color: $color-hover;
      font-weight: bold;
      font-size: 20px;
      vertical-align: middle;
      margin-right: 7px;
    }
}

}


</style>