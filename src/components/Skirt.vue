<script setup>
  import props from "./propsM.vue";
  
  import shirt10 from "./assets/Skirt/51gVqA510PL._AC_SY879_.jpg"
  // import shirt11 from "./assets/Skirt/51XvwhvN0wL._AC_SY879_.jpg"
  import shirt12 from "./assets/Skirt/BS-11741-DOUBLE-PLEATS-A-LINE-FLARE-SKIRT-LIGHT-DENIM.webp"
  import shirt13 from "./assets/Skirt/BSK-9529-PLEATED-SKIRT-BEIGE.webp"
  import shirt14 from "./assets/Skirt/D001_1_ae212fd7-bfe0-4610-a769-6716e43d8166_1001x1360.webp"
  import shirt15 from "./assets/Skirt/d001_1a29c863-0b9b-492d-a3bb-d4d6b7f6724c_1001x1360.webp"
  import shirt16 from "./assets/Skirt/D002_Beige_8299c874-be9c-4031-b621-d3aaf61a1269_1001x1360 (1).webp"
  import shirt17 from "./assets/Skirt/d002_Black_b291fb46-ce4c-4412-95a0-c91bc24e1fa7_1001x1360.webp"
  import shirt18 from "./assets/Skirt/d002_Dark_20gray_ab11a5f6-54a7-406c-95ab-81dec5d07e7a_1001x1360.webp"
  import shirt19 from "./assets/Skirt/d004_Black_a389d850-6676-4493-adc3-19e265e1cde0_1001x1360.webp"
  import shirt20 from "./assets/Skirt/D006_Black_55432f02-8e89-4805-8271-3d582759e522_1001x1360.webp"
  import shirt21 from "./assets/Skirt/Screenshot 2024-06-05 210623.png"
  import shirt22 from "./assets/Skirt/Screenshot 2024-06-05 210712.png"

  

 const posts = [
 {
    id: 12,
    img: shirt10,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  // {
  //   id: 12,
  //   img: shirt11,
  //   Name: "Name_3333 views  ",
  //   price: "15$",
  // },
  {
    id: 13,
    img: shirt12,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 14,
    img: shirt13,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 15,
    img: shirt14,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 16,
    img: shirt15,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 17,
    img: shirt16,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 18,
    img: shirt17,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 19,
    img: shirt18,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 20,
    img: shirt19,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 21,
    img: shirt20,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 22,
    img: shirt21,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 23,
    img: shirt22,
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