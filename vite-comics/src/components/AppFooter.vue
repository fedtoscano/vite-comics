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

        <div class="footer-top">
            <div class="navbar-container">
                
                <ul id="dc-comics-ul">
                    <li>DC COMICS</li>
                    <li v-for="el in dcComicsUlEls":key="el.id">
                        <a href="#">{{ el.text }}</a>
                    </li>
                </ul>
    
                <ul id="shop-ul">
                    <li>SHOP</li>
                    <li v-for="el in shopUlEls":key="el.id">
                        <a href="#">{{ el.text }}</a>
                    </li>
                </ul>
    
                <ul id="dc-ul">
                    <li>DC</li>
                    <li v-for="el in dcUlEls":key="el.id">
                        <a href="#">{{ el.text }}</a>
                    </li>
                </ul>
    
                <ul id="sites-ul">
                    <li>SITES</li>
                    <li v-for="el in sitesUlEls":key="el.id">
                        <a href="#">{{ el.text }}</a>
                    </li>
                </ul>
    
            </div>
    
            <div class="dc-logo-container">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
        
        <div class="footer-bottom">
            <div class="sign-up">
                <button>SIGN UP NOW!</button>
            </div>
            <div class="follow-us">
                <span>FOLLOW US</span>
                <div class="socials-container">
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                </div>
            </div>
        </div>

    </footer>


</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;

footer{
    display: flex;
    flex-direction: column;

    color: white;
    height: 600px;
    background-size: cover;
    background-image: url(../assets/img/footer-bg.jpg);
}

ul{
    @include footerUlStyle();
        & li:first-of-type{
        text-transform: uppercase;
        font-weight: 600;
        }
}

.footer-top{
    padding: 3em;
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.footer-bottom{
    padding: 3em;
    background-color: rgb(48, 48, 48);
    display: flex;
    justify-content: space-between;
    button{
        text-transform: uppercase;
        font-weight: bold;
        color: white;
        padding: 1em;
        border: 1px solid $color-blue;
        background-color: rgb(48, 48, 48);
    }
        .follow-us{
            display: flex;
            justify-content: space-around;
            gap: 2em;
            color: blue;
            font-size: 1.5em;

                span{
                    color: $color-blue;
                }
        }

        .socials-container img{
            margin-left: 1em;
        }
}

.navbar-container{
    display: flex;
    flex-direction: column;
    align-items: start;
    flex-wrap: wrap;
    height: 400px;
    font-size: .8em;
}

.dc-logo-container{
    width: 400px;

    img{
        width: 100%;
    }
}

h2{
    margin-bottom: .8em;
    font-weight: 800;
}
</style>