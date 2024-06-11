<script>
//importo cardList
import CardList from "./cardsComponents/CardList.vue";

export default {
    components: {
        CardList,
    },
    data() {
    return {
        
    }
    }

}
</script>

<template>
    <main>
        <CardList/>
    </main>
</template>

<style scoped lang="scss">
main{
    padding: 2rem 6rem;
    background-color: black;

    h1{
        color: white;
        text-align: center;
    }
}
</style>