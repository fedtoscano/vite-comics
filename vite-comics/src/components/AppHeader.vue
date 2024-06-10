<script>
export default {
    data() {
        return {
            navBarElements: [
                {
                    id: 1,
                    text: "characters",
                    active: false,
                },
                {
                    id: 2,
                    text: "comics",
                    active: false,
                },
                {
                    id: 3,
                    text: "movies",
                    active: false,
                },
                {
                    id: 4,
                    text: "tv",
                    active: false,
                },
                {
                    id: 5,
                    text: "games",
                    active: false,
                },
                {
                    id: 6,
                    text: "collectibles",
                    active: false,
                },
                {
                    id: 7,
                    text: "videos",
                    active: false,
                },
                {
                    id: 8,
                    text: "fans",
                    active: false,
                },
                {
                    id: 9,
                    text: "news",
                    active: false,
                },
                {
                    id: 10,
                    text: "shop",
                    active: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="logo-container">
            <img src="../assets/img/dc-logo.png" alt="DC Logo">
        </div>
        <div class="navbar-container">
            <ul>
                <li v-for="el in navBarElements" :key="el.id">
                    <a href="#">
                        {{ el.text.toUpperCase() }}
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem 4rem;
}

.logo-container{
    width: 80px;
    img{
        width: 100%;
    }
}
ul{
    list-style-type: none;
    display: flex;
    gap: 2em;

    & li a{
        text-decoration: none;
        color: black;
    }
}
</style>