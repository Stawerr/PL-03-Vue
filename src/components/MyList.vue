<template>
  <ul>
    <TasksComponent v-for="(item, i) of items" :description="item.description" :status="item.status" :key="i"></TasksComponent>
  </ul>
</template>

<script>
import TasksComponent from "./TasksComponent.vue";
export default {
  data() {
    return {
      items: [
        {
          description: "Limpar o jardim",
          status: true,
        },
        {
          description: "Arrumar a garagem",
          status: true,
        },
        {
          description: "Limpar o pó",
          status: false,
        },
      ]
    }
  },
  components: { TasksComponent }
}
</script>

<style scoped>

</style>
