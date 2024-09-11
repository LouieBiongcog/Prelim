<script>
export default {
    
    name: 'ItemList',
    props: ['Items'],
    components: ['Items'],
    methods: {
        addToCart(Items){
            console.log(Items)
        }
    }
}
</script>

<template>
  <div class="Items">
    <h4>{{ Items.name }}</h4>
    <p>Price: {{ Items.price }}</p>
    <button @click="addToCart(Items)">Add to Cart</button>
  </div>
</template>
<style scoped>
.item{
    border: 1px solid black;
    padding: 10px;
    margin: 10px;
    width: 200px;
    height: 200px;
    text-align: center;
    border-radius: 10px;
    box-shadow: 0px 4px 8px 2px rgba(0, 0, 0, 0.5);
    
}
button{
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
button:hover{
    background-color: #3e8e41;
}

</style>