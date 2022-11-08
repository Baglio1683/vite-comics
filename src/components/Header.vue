<script>

export default {
    name: "AppHeader",
    data() {
        return {
           message : "ciao"
        }
    }
}

</script>



<template>
   <h1>{{message}}</h1>
</template>

<style scope>

   h1{
    color : red
   }

</style>