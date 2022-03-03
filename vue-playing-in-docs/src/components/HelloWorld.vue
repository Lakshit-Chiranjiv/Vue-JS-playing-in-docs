<template>
  <HelloWorldOpt/>
  <HelloWorldComp/>
</template>

<script>
import HelloWorldOpt from './options_api_components/HelloWorldOpt.vue'
import HelloWorldComp from './composition_api_components/HelloWorldComp.vue'
export default {
    name: 'HelloWorld',
    components: {
        HelloWorldOpt,
        HelloWorldComp
    }
}
</script>

<style>

</style>