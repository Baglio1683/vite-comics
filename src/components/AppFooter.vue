<script>

export default{
    name: "AppFooter"
}

</script>

<template>

    <footer>
        <div class="container">
            <div>
                <a href="">SIGN UP NOW</a>
            </div>
            <div>
                FOOLOW US
                <ul>
                </ul>
            </div>
        </div>
    </footer>

</template>


<style lang="scss" scoped>

    footer{
        background-color: rgb(95, 95, 95);
        height: 10vh;
        width: 100%;
            ul{
            list-style: none;

                li{
                    display: inline-block;
                    margin-right: 10px;
                }
        }
    }

</style>