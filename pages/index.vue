<template>
  <!-- <Tutorial/> -->
  <!-- <Main/> -->
  <ComponentRequest/>
</template>

<script lang="ts">
    import Vue from 'vue'
    import ComponentRequest from '~/components/ComponentRequest/ComponentRequest.vue';
    
    export default Vue.extend({
    name: "IndexPage",
    components: { ComponentRequest }
})
</script>
