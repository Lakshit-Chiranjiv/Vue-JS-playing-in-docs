<template>
  <h3>Compositions api </h3>
  <h4>v-html</h4>
  <p>just span tag = {{htmlData}}</p>
  <p>span tag with v-html directive = <span v-html="htmlData"></span></p>

  <h4>v-bind</h4>
  <p v-bind:id="paraId">This is a green paragraph using v-bind id</p>
  <p :id="paraId">This is a green paragraph using v-bind id</p>
  <p :class="paraClass">This is a orange paragraph using v-bind class</p>
</template>

<script>
import { ref } from 'vue'
export default {
    name: "DirectivesComp",
    setup(){
        const htmlData = ref("<span>This is a span tag in blue color</span>")
        const paraId = ref("greenPara")
        const paraClass = ref("orangePara")
        return{
            htmlData,
            paraId,
            paraClass
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