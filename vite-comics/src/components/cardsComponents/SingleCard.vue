<script>
export default {
data() {
return {  
}
}, 
props: {
    cardThumb: String, 
    cardPrice: String, 
    cardSeries: String, 
    cardType: String,
}}
</script>

<template>
    <div class="single-card">
        <img :src="cardThumb" alt="">
        <span> {{ cardSeries }}</span>
    </div>
</template>

<style scoped lagn="scss">
    .single-card{
        display: flex;
        flex-direction: column;
        align-items: center;
        width: calc((100% / 6) - .25rem);
        margin-right: .25rem;

        span{
            text-align: center;
        }
        
        img{
            width: 100%;
            height: 80%;
        }
    }
</style>    