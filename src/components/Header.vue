<script>

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    title: "CHARACTERS",
                    href: "/home",
                    active: true,
                },

                {
                    title: "COMICS",
                    href: "/products",
                    active: true,
                },

                {
                    title: "MOVIES",
                    href: "/about",
                    active: true,
                },

                {
                    title: "TV",
                    href: "/contacts",
                    active: true,
                },

                {
                    title: "GAMES",
                    href: "/contacts",
                    active: true,
                },

                {
                    title: "COLLECTIBLES",
                    href: "/contacts",
                    active: true,
                },

                {
                    title: "VIDEOS",
                    href: "/contacts",
                    active: true,
                },

                {
                    title: "FANS",
                    href: "/contacts",
                    active: true,
                },

                {
                    title: "NEWS",
                    href: "/contacts",
                    active: true,
                },

                {
                    title: "SHOP",
                    href: "/contacts",
                    active: true,
                },
            ]
        }
    }
}

</script>



<template>

   <header>

    <div class="container">

        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>

        <div>
            <ul>
                <li v-for="(item) in links">{{item.title}}</li>
            </ul>
        </div>

    </div>
</header>
</template>



<style lang="scss" scope>

  header{
    height: 20vh;
    background-color: lightblue;

    ul{
        list-style: none;

        li{
            display: inline-block;
            margin-right: 10px;

            &:hover{
                color: blue;
            }
        }
    }
  }



</style>