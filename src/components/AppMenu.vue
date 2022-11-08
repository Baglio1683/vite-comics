<script>

export default {
        name: "AppMenu",
        data(){
            return{
                links: [
                    {
                      srcIm : "../assets/img/buy-comics-digital-comics.png",
                      description: "DiGITAL COMICS"

                    },

                    {
                        srcIm : "../assets/img/buy-comics-digital-comics.png",
                      description: "DiGITAL COMICS"

                    },

                    {
                        srcIm : "../assets/img/buy-comics-digital-comics.png",
                      description: "DiGITAL COMICS"

                    },

                    {
                        srcIm : "../assets/img/buy-comics-digital-comics.png",
                      description: "DiGITAL COMICS"

                    },

                    {
                        srcIm : "../assets/img/buy-comics-digital-comics.png",
                      description: "DiGITAL COMICS"

                    },


                ]
            }
        }, 
        methods : {

            getImagePath: function(imgPath){

                return URL(imgPath, import.meta.url).href

            }

        }
    }

</script>

<template>

    <section>
        <div class="container">

            <div class="card" v-for="(item) in links">

                <img src={{item.srcIm}} alt="">
                <p>{{item.description}}</p>
                
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>

section{
    height: 20vh;
    background-color: rgb(73, 73, 255);
}



</style>