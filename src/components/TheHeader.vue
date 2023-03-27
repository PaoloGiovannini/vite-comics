<script>
export default {
  name: "TheHeader",
  data() {
    return {
        navbarItems: [
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
        ]
    }
  }
};
</script>

<template>
    <header>
        <div class="container">
            <div class="d-flex space-between flex-center">
                <img src="../assets/dc-logo.png" alt="logo dc">
                <ul>
                    <li v-for="item in navbarItems">
                        <a :href="item.href">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>

</template>

<style scoped lang="scss">
@use"../styles/partials/variables" as *;
.container{
    max-width: 1170px;
    margin: auto;
    padding: 10px;

    img{
        width: 70px;
    }

    ul li{
    display: inline-block;
    padding: 0px 10px;
        
        a{
        color: $color-nav;

         &:hover{
         color: $color-hover;
         }
        }
    }
}



</style>