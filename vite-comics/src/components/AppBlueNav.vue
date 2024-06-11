<script>
export default {
    data() {
        return {
            navBarItems: [
                {
                    id: 1, 
                    text: "digital comics",
                    img: "./src/assets/img/buy-comics-digital-comics.png",
                },
                {
                    id: 2, 
                    text: "dc merchandise",
                    img: "./src/assets/img/buy-comics-merchandise.png",
                },
                {
                    id: 3, 
                    text: "subscription",
                    img: "./src/assets/img/buy-comics-subscriptions.png",
                    
                },
                {
                    id: 4, 
                    text: "comic shop locator",
                    img: "./src/assets/img/buy-comics-shop-locator.png",
                },
                {
                    id: 5, 
                    text: "dc power visa",
                    img: "./src/assets/img/buy-dc-power-visa.svg",
                },
            ]
        }
    }
}
</script>


<template>
    <nav>
        <ul>
            <li v-for="item in navBarItems" :key="item.id">
                <img :src="item.img" :alt="`${item.text} logo`">
                <span> {{ item.text.toUpperCase() }} </span>
            </li>
        </ul>
    </nav>
</template>


<style lang="scss" scoped>
@import "../styles/partials/variables.scss";

nav{
    background-color: $color-blue;

    ul{
        display: flex;
        justify-content: space-around;
        align-items: center;
        list-style-type: none;
        padding: 4em;
    }
    li{
        display: flex;
        align-items: center;
    }
    img{
        width: 60px;
        height: 80px;
        margin-right: .5em;
    }
}

</style>