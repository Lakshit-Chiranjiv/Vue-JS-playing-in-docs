<template>
  <h3>{{objVal.name}} - {{objVal.power}}</h3>
  <h3>{{normalVal}} - {{num}}</h3>
  <p>sums up to {{objVal.power + num}}</p>
  <p>whole string is {{objVal.name + normalVal}}</p>
</template>

<script>
import { ref,reactive } from 'vue'

export default{
    name: "TemplatesComp",
    setup(){
      const objVal = reactive({
          name: "reactive component",
          power: 78
      })

      const normalVal = ref("Ref component")
      const num = ref(81)

      console.log(objVal,objVal.name,objVal.power);
      console.log(normalVal,normalVal.value)
      console.log(num,num.value)

      return{
        objVal,
        normalVal,num
      }
    }
}


</script>

<style>

</style>