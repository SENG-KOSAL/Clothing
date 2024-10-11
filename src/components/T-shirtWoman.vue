<script setup>
  import props from "./propsM.vue";
  
  //shirt
  import shirt from "./assets/woman/hmgoepprod.webp"
  import shirt1 from "./assets/woman/1688629051371.jpg"
  import shirt2 from "./assets/woman/1688629051383.jpg"
  import shirt3 from "./assets/woman/AKB-8349-STRIPE-BUTTON-KNIT-BEIGE.webp"
  import shirt4 from "./assets/woman/AKB-8349-STRIPE-BUTTON-KNIT-NAVY-1.webp"

  import shirt5 from "./assets/woman/ao-so-mi-nu-10-10f23shsw001-blue-stripe-_2__1_1_jpg.webp"
  import shirt6 from "./assets/woman/BB11724PRINTEDBLOUSECREAM.webp"
  import shirt7 from "./assets/woman/BK11745CROCHETTOPPALEBLUE.jpg"
  import shirt8 from "./assets/woman/hmgoepprod (1).jpg"
  import shirt9 from "./assets/woman/hmgoepprod (1).webp"
  

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
    id: 5,
    img: shirt4,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 6,
    img: shirt5,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 7,
    img: shirt6,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 8,
    img: shirt7,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 9,
    img: shirt8,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 10,
    img: shirt9,
    Name: "Name_3333 views  ",
    price: "15$",
  },
 
  
];
</script>


<template>
    
    <nav class="navbar">
      <div class="logo">TradeofB</div>
      <ul class="nav-links">
        <router-link to="/"> Home </router-link>
        <router-link to="/Man"> Man </router-link>
        <router-link to="/Woman"> Woman </router-link>
        <router-link to="/Man"> Promotion </router-link>
      </ul>
      <div class="search-login">
        <div class="search-bar">
          <input type="text" placeholder="Search" />
        </div>
        <a href="#" class="login">Login / Register</a>
      </div>
    </nav>
    <!-- <h2 class="title">Woman clothing</h2> -->
    <details>
      <summary class="title" > Woman Clothing</summary>
     <ul class="son_title">
      <router-link to="/Woman"><ul>All clothing</ul></router-link>
      <router-link to="/T_Shirt_Woman"><ul>T-Shirt</ul></router-link>
      <router-link to="/Dress"><ul>Dress</ul></router-link>
      <router-link to="/Skirt"><ul>Skirt</ul></router-link>
      <router-link to="/jean"><ul>Jean</ul></router-link>
       
      
       
     </ul>
    </details>
    <div id="app">
    
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
<style scoped>
  .navbar {
    display: flex;
    font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background-color: #c0bbbb;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .logo {
    font-size: 24px;
    font-weight: bold;
  }
  
  .nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
  }
  
  .nav-links a {
    
    /* text-decoration: none;
    color: rgb(84, 84, 84);
    font-size: 18px;
    padding: 8px 15px;
    transition: background-color 0.3s; */
    text-decoration: none;
    color: rgb(60, 60, 60); /* Slightly darker, modern text color */
    font-size: 18px;
    padding: 8px 15px;
    border-radius: 4px;
    transition: color 0.2s, background-color 0.2s, box-shadow 0.2s;
    background-color: transparent; /* No background initially */
  }
  
  .nav-links a:hover {
    color: #050404;
    background-color: rgba(0, 0, 0, 0.05); /* Very light background on hover */
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1); /* Soft shadow for clean elevation effect */

    
  }
  
  .search-login {
    display: flex;
    gap: 15px;
    align-items: center;
  }
  
  .search-bar input {
    padding: 5px 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  .login {
    text-decoration: none;
    color: #000;
    font-size: 16px;
  }
  /* edit===== */
  .title {
    font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
    font-size: 24px; /* Make the font large, but not overly big */
    padding: 10px 15px;
    font-weight: bold;
    cursor: pointer;
    color:  rgb(130, 125, 125); /* Clean, dark color */
    border-bottom: 1px solid rgba(0, 0, 0, 0.1); /* Soft border for a refined look */
    transition: color 0.3s ease ;
}

.title:hover {
    color: #292626; /* Subtle hover color */
    
    
    
}

.son_title {
    font-family: 'Lucida Sans', Geneva, Verdana, sans-serif;
    font-size: 18px;
    color: #333; /* Consistent with title color */
    list-style: none; /* Remove bullets for a cleaner look */
    padding: 10px 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 10px; /* Vertical gap between items */
}

.son_title li {
    padding: 5px 10px;
    border-radius: 4px; /* Rounded corners */
    transition: background-color 0.3s, color 0.3s ease;
}

.son_title li:hover {
    background-color: rgba(0, 0, 0, 0.05); /* Subtle hover background */
    color: #005f5f; /* Hover color matches title */
}

.son_title a {
    text-decoration: none;
    color: inherit; /* Inherits the li's color for a clean look */
}

details[open] .title {
    border-bottom: none; /* Remove border when expanded */
}


/* edit  */

.son_title a:hover {
    text-decoration: none;
    background-color: #cbc8c8;
}

  </style>