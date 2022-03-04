<template>
  <h3>Options api</h3>
  <h4>v-html</h4>
  <p>just span tag = {{rawHtml}}</p>
  <p>span tag with v-html directive = <span v-html="rawHtml"></span></p>

  <h4>v-bind</h4>
  <p v-bind:id="paraId">This is a green paragraph using v-bind id</p>
  <p :id="paraId">This is a green paragraph using v-bind id</p>
  <p :class="paraClass">This is a orange paragraph using v-bind class</p>

  <h4>multiple v-binds</h4>
  <p v-bind="multipleBindObj">This paragraph is red and large in size</p>
</template>

<script>
export default {
    name: "DirectivesOpt",
    data(){
        return{
            rawHtml: "<span>This is a span tag in blue color</span>",
            paraId: "greenPara",
            paraClass: "orangePara",
            multipleBindObj: {
                id: "bigPara",
                class: "redPara"
            }
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
    .redPara{
        color: red;
    }
    #bigPara{
        font-size: 24px;
    }
</style>