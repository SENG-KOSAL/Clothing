

<script setup>
  import Banner from "./Navbar.vue";
  import Navbar from "./Banner.vue";
  import props from "./propsH.vue";
  

  //img
  import shirt from "./assets/07200410916-e1.jpg"
  import shirt1 from "./assets/basic sliim fit 2.jpg"
  import shirt2 from "./assets/seersucker printed shirt.jpg"
  import shirt3 from "./assets/streak print shirt 1.jpg"

  
  
   const posts = [
  {
    id: 1,
    img: shirt,
    Name: "Name_1",
    price: "15$",
  },
  {
    id: 2,
    img: shirt1,
    Name: "basic sliim fit 2",
    price: "20$",
  },
  {
    id: 3,
    img: shirt2,
    Name: "Name_3333 views  ",
    price: "10$",
  },
  {
    id: 3,
    img: shirt3,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 4,
    img: shirt3,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  
];
</script>



<template>
 
  <div id="app">
    <Banner />
    <Navbar />
    <div class="container">
      <props
       v-for="post in posts"
       :key="post.id"
       :Name="post.Name"
       :img="post.img"
       :price="post.price"
       class="component-item"
      />
      <nav>
      
       
    </nav>
    
    </div>
  </div>
</template>
<style>
.container {
  background-color: #ffffff;
  display: flex;
  flex-wrap: wrap;
  gap: 18px;
  width: 100%;
  margin: 0 auto;
  justify-content: center;
  padding: 20px;
  border-radius: 1px;
  box-shadow: 0 4px 8px rgba(255, 255, 255, 0.928)}
.component-item {
  margin: 12px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 305px;
  padding: 10px;
  background-color: #ffffff;
  border-radius: 1px;
  box-shadow: 0 4px 8px rgba(255, 255, 255, 0.912);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.component-item img {
  width: 100%;
  border-radius: 33px;
}

.component-item h3 {
  margin: 1px 0 5px;
  font-size: 1.2em;
  color: #000000;
}

.component-item p {
  font-size: 0.9em;
  color: #ffffff;
}

.component-item:hover {
  transform: translateY(-10px);
  box-shadow: 0 8px 16px rgba(255, 255, 255, 0.2);
}
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: white;
}

#app {
  text-align: center;
  background-color: white; 
}
</style>
