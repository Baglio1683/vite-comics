<script>

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    title: "CHARACTERS",
                    href: "/characters",
                    active: true,
                },

                {
                    title: "COMICS",
                    href: "/comics",
                    active: true,
                },

                {
                    title: "MOVIES",
                    href: "/movies",
                    active: true,
                },

                {
                    title: "TV",
                    href: "/tv",
                    active: true,
                },

                {
                    title: "GAMES",
                    href: "/games",
                    active: true,
                },

                {
                    title: "COLLECTIBLES",
                    href: "/collectibles",
                    active: true,
                },

                {
                    title: "VIDEOS",
                    href: "/videos",
                    active: true,
                },

                {
                    title: "FANS",
                    href: "/fans",
                    active: true,
                },

                {
                    title: "NEWS",
                    href: "/news",
                    active: true,
                },

                {
                    title: "SHOP",
                    href: "/shop",
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

        <div class="right_header">
            <ul>
                <li v-for="(item) in links"><a href="">{{item.title}}</a></li>
            </ul>
        </div>

    </div>
</header>
</template>



<style lang="scss" scoped>

  header{
    height: 15vh;

    .right_header{

        ul{
            list-style: none;

            li{
                display: inline-block;
                margin-right: 10px;

                a{
                    text-decoration: none;
                    color: black;
                }

                & a:hover{
                    color: #0280F9;
                }
            }
        }
     }

    img{
        height: 12vh;
    }
  }



</style>