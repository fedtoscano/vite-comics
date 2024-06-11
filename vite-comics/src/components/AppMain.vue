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
        <span class="series">
            current series
        </span>
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
    position: relative;

    h1{
        color: white;
        text-align: center;
    }

    button{
        @include buttonStyle();
        align-self: center;
    }

    .series{
        padding: 1rem 4rem;
        color: white;
        text-align: center;
        text-transform: uppercase;
        font-weight: 800;
        background-color: $color-blue;
        position: absolute;
        top: -2%;
        left: 5%;
    }
}
</style>