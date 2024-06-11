<script>
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

        <button>Load More</button>
    </main>
</template>

<style scoped lang="scss">
@use '../styles/partials/mixins' as *;
@import "../styles/partials/variables.scss";


main{
    padding: 6rem;
    background-color: black;
    display: flex;
    flex-direction: column;
    gap: 2rem;

    h1{
        color: white;
        text-align: center;
    }

    button{
        @include buttonStyle();
        align-self: center;
    }
}
</style>