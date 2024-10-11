<script setup>
  import props from "./propsM.vue";
  
  //shirt
  import shirt from "./assets/07200410916-e1.jpg"
  import shirt1 from "./assets/basic sliim fit 2.jpg"
  import shirt2 from "./assets/seersucker printed shirt.jpg"
  import shirt3 from "./assets/streak print shirt 1.jpg"
  //hoodie + sweater
  import shirt4 from "./assets/hoodie+sweater/jacquard 1.jpg"
  import shirt5 from "./assets/hoodie+sweater/jacquard.jpg"
  import shirt6 from "./assets/hoodie+sweater/print sweatshirt 1.jpg"
  import shirt7 from "./assets/hoodie+sweater/print sweatshirt.jpg"
  import shirt8 from "./assets/hoodie+sweater/slogan 2.jpg"
  import shirt9 from "./assets/hoodie+sweater/slogan 3.jpg"
  import shirt10 from "./assets/hoodie+sweater/slogan.jpg"
  import shirt11 from "./assets/hoodie+sweater/solgan 1.jpg"
  import shirt12 from "./assets/hoodie+sweater/techincial.jpg"
  import shirt13 from "./assets/hoodie+sweater/technical 1.jpg"
  import shirt14 from "./assets/hoodie+sweater/zip hoodie.jpg"
  //pant
  import shirt15 from "./assets/pant/comfortt trosers.jpg"
  import shirt16 from "./assets/pant/confort troiusers.jpg"
  import shirt17 from "./assets/pant/jooger 1.jpg"
  import shirt18 from "./assets/pant/jooger troussers.jpg"
  import shirt19 from "./assets/pant/striped jacquard.jpg"
  import shirt20 from "./assets/pant/striped jacuard 1.jpg"
  import shirt21 from "./assets/pant/wide fit pleated 1.jpg"
  import shirt22 from "./assets/pant/wide fit pleated.jpg"
  //short 
  import shirt23 from "./assets/short_man/bermida white 1.jpg"
  import shirt24 from "./assets/short_man/bermuca b 1.jpg"
  import shirt25 from "./assets/short_man/bermuda b.jpg"
  import shirt26 from "./assets/short_man/bermuda white.jpg"
  import shirt27 from "./assets/short_man/traning short 1.jpg"
  import shirt28 from "./assets/short_man/trasining hsort.jpg"


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
    id: 4,
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
  {
    id: 11,
    img: shirt10,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 12,
    img: shirt11,
    Name: "Name_3333 views  ",
    price: "15$",
  },
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
  {
    id: 24,
    img: shirt23,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 25,
    img: shirt24,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 26,
    img: shirt25,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 27,
    img: shirt26,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 28,
    img: shirt27,
    Name: "Name_3333 views  ",
    price: "15$",
  },
  {
    id: 29,
    img: shirt28,
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
        <router-link to="/Man" title="Man clothing"> Man </router-link>
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
    

    <details>
      <summary class="title" > Men's Clothing</summary>
     <ul class="son_title">
      <router-link to="/Man"><ul>All clothing</ul></router-link>
      <router-link to="/T_Shirt"><ul>T-Shirt</ul></router-link>
      <router-link to="/Sweater_hoodie"><ul>Sweater & Hoodie</ul></router-link>
      <router-link to="/Pant"><ul>Pant</ul></router-link>
      <router-link to="/Short"><ul>Short</ul></router-link>
       
      
       
       
       
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
      
    
    </div>
  </div>
</template>
<style scoped>
 @import url('https://fonts.googleapis.com/css2?family=Playwrite+AU+SA:wght@100..400&display=swap');
  .navbar {
    display: flex;
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
    text-decoration: none;
    color: #000;
    font-size: 18px;
    padding: 5px 10px;
    transition: background-color 0.3s;
  }
  
  .nav-links a:hover {
    background-color: #f0f0f0;
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