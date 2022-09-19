<template>
  <div>
   <MyList></MyList>
   <UserComponent></UserComponent>
  </div>
</template>

<script>
  import MyList from "./components/MyList.vue";
  import UserComponent from "./components/userComponent.vue";

 export default {
  components: {
    MyList,
    UserComponent
}
 }
  
  </script>
  
<style scoped>

</style>
