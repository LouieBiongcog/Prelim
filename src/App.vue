<template>
  <Item :Items="Items"/>
</template>


<script>
import Item from './components/icons/Item.vue'
export default {
  name: 'App',
  components: {
    Item,
    },
    data() {
      return {
        Items: [
          { id: 1, name: 'Product 1', price: 10.99},
          { id: 2, name: 'Product 2', price: 9.99},
          { id: 3, name: 'Product 3', price: 7.99},
        ]
      }
    }
}
</script>
<style scoped>
.list-container{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}
</style>