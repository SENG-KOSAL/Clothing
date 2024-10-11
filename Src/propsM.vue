<script setup lang="js">
   const props = defineProps({
    img:String,
    Name:String,
    price:String,
   
   });
   
</script>

<template>
    <div class="Card">
      <div class="img">
        <img :src="img" >
        <h3>{{ props.price }} </h3>
            {{ props.Name }} 
          
        </div>
        <button @click="addToCart">Add To Card</button>
    </div>
   
</template>
<style>
  .Card {
  
  border-radius: 5px;
  padding: 10px;
  text-align: center;
}
.img {
  width: 100%;
  height: auto;
  margin: 9px;
}

</style>
