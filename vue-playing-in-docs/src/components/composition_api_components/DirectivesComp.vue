<template>
  <h3>Compositions api </h3>
  <h4>v-html</h4>
  <p>just span tag = {{htmlData}}</p>
  <p>span tag with v-html directive = <span v-html="htmlData"></span></p>

  <h4>v-bind</h4>
  <p v-bind:id="paraId">This is a green paragraph using v-bind id</p>
  <p :id="paraId">This is a green paragraph using v-bind id</p>
  <p :class="paraClass">This is a orange paragraph using v-bind class</p>

  <h4>multiple v-binds</h4>
  <p v-bind="multipleBindObj">This paragraph is red and large in size</p>
</template>

<script>
import { ref,reactive } from 'vue'
export default {
    name: "DirectivesComp",
    setup(){
        const htmlData = ref("<span>This is a span tag in blue color</span>")
        const paraId = ref("greenPara")
        const paraClass = ref("orangePara")
        const multipleBindObj = reactive({
            id: "bigPara",
            class: "redPara"
        })
        return{
            htmlData,
            paraId,
            paraClass,
            multipleBindObj
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