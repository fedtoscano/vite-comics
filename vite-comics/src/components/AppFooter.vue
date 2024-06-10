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
            
            <h2>DC COMICS</h2>
            <ul id="dc-comics-ul">
                <li v-for="el in dcComicsUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

            <h2>SHOP</h2>
            <ul id="shop-ul">
                <li v-for="el in shopUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

            <h2>DC</h2>
            <ul id="dc-ul">
                <li v-for="el in dcUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

                <h2>SITES</h2>
            <ul id="sites-ul">
                <li v-for="el in sitesUlEls":key="el.id">
                    <a href="#">{{ el.text }}</a>
                </li>
            </ul>

        </div>

        <div class="dc-logo-container">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>

    </footer>


</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;

footer{
    padding: 4em;
    font-size: .8em;
    display: flex;
    justify-content: space-between;
    color: white;
    height: 600px;
    background-image: url(../assets/img/footer-bg.jpg);
}

ul{
    @include footerUlStyle()
}

.navbar-container{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 100%;
}

.dc-logo-container{
    width: 400px;

    img{
        width: 100%;
    }
}

h2{
    font-weight: 800;
}
</style>