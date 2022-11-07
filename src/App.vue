<template>
  <Form @savePlace="insertPlace"></Form>
  <Place />

  <!-- v-if="items.length > 0" :addPlace="items" -->
</template>
<script>
import Place from './components/PlaceComponent.vue'
import Form from './components/FormComponent.vue'
import '../src/assets/styles/tailwindcss.css'
export default {
  name: 'App',
  title: 'test',
  components: {
    Place,
    Form
  },
  data() {
    return {
      items: []
    }
  },
  methods: {
    insertPlace(data) {
      this.items.push(data);
    }
  }
}
</script>

<style>

</style>
