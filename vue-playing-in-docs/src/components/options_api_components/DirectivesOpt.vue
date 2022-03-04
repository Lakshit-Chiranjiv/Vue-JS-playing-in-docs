<template>
  <h3>Options api</h3>
  <h4>v-html</h4>
  <p>just span tag = {{rawHtml}}</p>
  <p>span tag with v-html directive = <span v-html="rawHtml"></span></p>

  <h4>v-bind</h4>
  <p v-bind:id="paraId">This is a green paragraph using v-bind id</p>
  <p :id="paraId">This is a green paragraph using v-bind id</p>
  <p :class="paraClass">This is a orange paragraph using v-bind class</p>
</template>

<script>
export default {
    name: "DirectivesOpt",
    data(){
        return{
            rawHtml: "<span>This is a span tag in blue color</span>",
            paraId: "greenPara",
            paraClass: "orangePara"
        }
    }
}
</script>

<style>
    span{
        color: blue;
    }
    h4{
        text-decoration: underline;
    }
    .orangePara{
        color: orange;
    }
    #greenPara{
        color: green;
    }
</style>