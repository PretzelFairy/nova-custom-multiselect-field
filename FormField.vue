<template>
  <multiselect v-model="value" :options="options"></multiselect>
</template>

<script>
import Multiselect from 'vue-multiselect'
export default {
props: ['index', 'resource', 'resourceName', 'resourceId', 'field'],
components: { Multiselect },
data () {
  return {
    options: [
    { id: 1, label: "A" },
    { id: 2, label: "B" },
    { id: 3, label: "C" }
  ],
  selected: []
  }
}
}
</script>

<style src="vue-multiselect/dist/vue-multiselect.min.css"></style>
