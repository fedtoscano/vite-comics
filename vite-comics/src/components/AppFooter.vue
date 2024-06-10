<script>
export default {
    data() {
        return {
            dcComicsUlEls: [
                {
                    id: 1, 
                    text: "Characters"
                },
                {
                    id: 2, 
                    text: "Comics"
                },
                {
                    id: 3, 
                    text: "Movies"
                },
                {
                    id: 4, 
                    text: "Tv"
                },
                {
                    id: 5, 
                    text: "Games"
                },
                {
                    id: 6, 
                    text: "Videos"
                },
                {
                    id: 7, 
                    text: "News"
                },
            ],
            shopUlEls: [
                {
                    id: 1, 
                    text: "Shop DC"
                },{
                    id: 2, 
                    text: "Shop DC Collectibles"
                },
            ],
            dcUlEls: [
            {
                    id: 1, 
                    text: "Terms of use"
                },
                {
                    id: 2, 
                    text: "Privacy Polici (new)"
                },
                {
                    id: 3, 
                    text: "Ad Choices"
                },
                {
                    id: 4, 
                    text: "Advertising"
                },
                {
                    id: 5, 
                    text: "Jobs"
                },
                {
                    id: 6, 
                    text: "Subscriptions"
                },
                {
                    id: 7, 
                    text: "Talent Workshops"
                },
                {
                    id: 8, 
                    text: "CPSC Certificates"
                },
                {
                    id: 9, 
                    text: "Ratings"
                },
                {
                    id: 10, 
                    text: "Shop Help"
                },
                {
                    id: 11, 
                    text: "Contact Us"
                },
            ],
            sitesUlEls: [
                {
                    id: 1, 
                    text: "DC"
                },
                {
                    id: 2, 
                    text: "MAD Magazine"
                },
                {
                    id: 3, 
                    text: "DC Kids"
                },
                {
                    id: 4, 
                    text: "DC Universe"
                },
                {
                    id: 5, 
                    text: "DC Power Visa"
                },
            ]
        }
    } 
}
</script>

<template>
    <footer>
                <div class="navbar-container">

            <ul id="dc-comics-ul">
                <li v-for="el in dcComicsUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

            <ul id="shop-ul">
                <li v-for="el in shopUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

            <ul id="dc-ul">
                <li v-for="el in dcUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

            <ul id="sites-ul">
                <li v-for="el in sitesUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>
        </div>
    <div class="footer-bottom"></div>
    </footer>


</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
ul{
    $ulStyle
}
</style>