<template>
  <DirectivesOpt/>
  <DirectivesComp/>
</template>

<script>
import DirectivesOpt from './options_api_components/DirectivesOpt.vue'
import DirectivesComp from './composition_api_components/DirectivesComp.vue'
export default {
    name: "Directives",
    components: {
        DirectivesOpt,
        DirectivesComp
    }
}
</script>

<style>

</style>