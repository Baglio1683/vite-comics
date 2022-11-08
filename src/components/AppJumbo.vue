<script>

export default{
    name : "AppJumbo"
}

</script>

<template>

    <section>
        <div class="container">
         
            <div class="lists">
                <ul>
                    <h2>DC COMICS</h2>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                </ul>
            </div>

            <div class="logo">
            </div>



        </div>
    </section>

</template>


<style lang="scss" scoped>

    section{
        height: 45vh;
        width: 100%;
        background-image: url("../assets/img/footer-bg.jpg");
    }

    .logo{
        height: 100%;
        width: 50%;
        background-image: url("../assets/img/dc-logo-bg.png");
        background-size: cover; 
       
    }
        img{
            height: 50vh;
            object-fit: fill;
        }

</style>