<script>
    export default {
      name: "TheFooterUp",
      data() {
        return {
            DcComics: [
            {
              text: "Characters",
              href: "#",
            },
            {
              text: "Comics",
              href: "#",
            },
            {
              text: "Movies",
              href: "#",
            },
            {
              text: "TV",
              href: "#",
            },
            {
              text: "Games",
              href: "#",
            },
            {
              text: "Collectibles",
              href: "#",
            },
            {
              text: "Videos",
              href: "#",
            },
            {
              text: "Fans",
              href: "#",
            },
            {
              text: "News",
              href: "#",
            },
            {
              text: "Shop",
              href: "#",
            },
            ],

            ShopDc:[
            {
              text: "Shop Dc",
              href: "#",
            },
            {
              text: "Shop Dc Collectibles",
              href: "#",
            }  
            ],

            DC:[
            {
              text: "Term Of Use",
              href: "#",
            },
            {
              text: "Privacy policy(new)",
              href: "#",
            },
            {
              text: "Ad Choices",
              href: "#",
            },
            {
              text: "Advertising",
              href: "#",
            },
            {
              text: "Jobs",
              href: "#",
            },
            {
              text: "Subscriptions",
              href: "#",
            },
            {
              text: "Talent Workshops",
              href: "#",
            },
            {
              text: "CPSC Certificates",
              href: "#",
            },
            {
              text: "Ratings",
              href: "#",
            },
            {
              text: "Shop Helps",
              href: "#",
            },
            {
              text: "Contact Us",
              href: "#",
            }, 
            ],
            Sites:[
            {
              text: "DC",
              href: "#",
            },
            {
              text: "MAD Magazine",
              href: "#",
            },
            {
              text: "DC Kids",
              href: "#",
            },
            {
              text: "DC Universe",
              href: "#",
            },
            {
              text: "DC Power Visa",
              href: "#",
            },
            ]

        }
    }
      
    }

</script>
    
<template>
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

</template>
    
<style scoped lang="scss">
@use"../styles/partials/variables" as *;

.wrap{
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}
.container{
    background-image: url(../assets/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
}
h3{
    margin: 20px 0px;
    color: $text-main;
}

ul li{
    padding: 3px 0px;
    
}
a{
    color:#959595;;
}

.sites{
    margin-left: 10px;
}

</style>