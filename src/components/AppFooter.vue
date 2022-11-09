<script>

export default{
    name: "AppFooter", 

    data(){
        return{

            images : [
                {src: "../assets/img/footer-facebook.png"},
                {src: "../assets/img/footer-periscope.png"},
                {src: "../assets/img/footer-pinterest.png"},
                {src: "../assets/img/footer-twitter.png"},
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
            <div class="left_foot">
                <a href="">SIGN UP NOW</a>
            </div>
            <div class="right_foot">
                <p>FOOLOW US</p> 
                <ul>
                    <li v-for="(item) in images">
                        <a href=""><img :src="getImagePath(item.src)" alt=""></a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>

</template>


<style lang="scss" scoped>

    footer{
    
        background-color: #303030;
        width: 100%;
        padding: 1em;

    .left_foot{
     
        a{
           display: inline-block;
           text-decoration: none;
           color: white;
           border: 3px solid #0282F9;
           padding: 10px;
        }
    }

    .right_foot{
            display: flex;
            justify-content: flex-start;
            align-items: center;
        
        p{
            color: #0282F9;
            font-weight: bold;
            margin-right: 10px;

        }
        ul{
            list-style: none;
            margin-left: 10px;

                li{
                    display: inline-block;
                    margin-right: 10px;
                }
            }

          }
       }

</style>