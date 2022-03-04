<template>
  <TemplatesOpt/>
  <TemplatesComp/>
</template>

<script>
import TemplatesOpt from './options_api_components/TemplatesOpt.vue'
import TemplatesComp from './composition_api_components/TemplatesComp.vue'
export default {
    name: "Templates",
    components: {
        TemplatesOpt,
        TemplatesComp
    }
}
</script>

<style>

</style>