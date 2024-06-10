<script>
export default {
    data() {
        return {
            navBarItems: [
                {
                    id: 1, 
                    text: "digital comics",
                    img: "../assets/img/buy-comics-digital-comics.png",
                },
                {
                    id: 2, 
                    text: "dc merchandise",
                    img: "../assets/img/buy-comics-merchandise.png",
                },
                {
                    id: 3, 
                    text: "subscription",
                    img: "../assets/img/buy-comics-subscription.png",
                },
                {
                    id: 4, 
                    text: "comic shop locator",
                    img: "../assets/img/buy-comics-comic-shop-locator.png",
                },
                {
                    id: 5, 
                    text: "dc power visa",
                    img: "../assets/img/buy-comics-dc-power-visa.png",
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
@import "../styles/variables.scss"


</style>