<template>
    <div class="fumetto-card">
        <img :src="image" :alt="title">
        <p>{{ title }}</p>
    </div>
</template>

<script>
  export default {
        name: "ProductCard",
        props: {
            image: String,
            title: String
        }
    }
</script>

<style lang="scss" scoped>
    .fumetto-card {
        & img {
            width: 180px;
            height: 180px;
        }
        
        & p{
        margin: 10px 0px;
    }
    }
    
</style>