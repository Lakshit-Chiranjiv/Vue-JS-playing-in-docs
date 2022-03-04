<template>
  <h3>{{message}}</h3>
  <p>message length = {{message.length}}</p>
</template>

<script>
export default {
    name: "TemplatesOpt",
    data(){
        return{
            message: "message from options api template syntax"
        }
    }
}
</script>

<style>

</style>