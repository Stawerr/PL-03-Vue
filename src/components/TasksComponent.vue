<template>
    <li>
      <p>{{description}}</p>
      <input type="checkbox" v-model="status" />
    </li>
</template>

<script>
export default {
  props:{
    description: String,
    status: Boolean,
  },

}
</script>

<style scoped>

</style>