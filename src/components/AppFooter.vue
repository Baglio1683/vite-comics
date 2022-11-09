<script>

export default{
    name: "AppFooter", 

    data(){
        return{

            images : [
                {src: "../assets/img/footer-facebook.png"},
                {src: "../assets/img/footer-periscope.png"},
                {src: "../assets/img/footer-pinterest.png"},
                {src: "../assets/img/footer-twitter"},
                {src: "../assets/img/footer-youtube.png"}
            ]


        }
    }, 
    methods : {

        getImagePath: function(imgPath){

            return new URL(imgPath, import.meta.url).href

        }

     }

}

</script>

<template>

    <footer>
        <div class="container">
            <div>
                <a href="">SIGN UP NOW</a>
            </div>
            <div class="right_foot">
                FOOLOW US
                <ul>
                    <li v-for="(item) in images">
                        <img :src="getImagePath(item.src)" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </footer>

</template>


<style lang="scss" scoped>

    footer{
        background-color: rgb(95, 95, 95);
        width: 100%;
        padding: 1rem;
            ul{
            list-style: none;

                li{
                    display: inline-block;
                    margin-right: 10px;
                }
        }

        .right_foot{
            display: flex;
            justify-content: flex-start;
            align-items: center;

            ul{
                margin-left: 10px;
            }
        }
    }

</style>