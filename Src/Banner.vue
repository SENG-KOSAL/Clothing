<template>
    <div class="banner">
      <div class="banner-content">
        <h1>Shop the latest fashion designed by Top Brands</h1>
        <button>Shop Now</button>
      </div>
    </div>
    <div class="img">
       <img src="@/components/assets/rectangle_12.png" alt="">
       
       <div class="text_of_img">
        <h3>The Holiday Outfit</h3>
       </div>
    </div>
  </template>
  
  <style scoped>
  .banner {
    background-image: url('@/components/assets/rectangle_2.png') ; 
    background-size: cover;
    background-position: center;
    color: rgb(255, 255, 255);
    text-align: left;
    padding: 320px 20px;
    position: relative;
  }
  
  .banner-content {
    position: absolute;
    bottom: 30px;
    left: 30px;
    max-width: 600px;
  }
  
  .banner h1 {
    font-size: 36px;
    margin-bottom: 20px;
  }
  
  .banner button {
    padding: 10px 20px;
    background-color: #c60000;
    color: #fff;
    border: none;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
  }
  
  .banner button:hover {
    background-color: #333;
  }
  .img {
    display: flex;
    align-items: center;
    
    gap: 20px;
    margin: 20px 0;
    
  }
  .img img {
    height: 300px;
    width: 800px;
    object-fit: cover;
    border-radius: 30px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border: 2px solid #fff;
    transition: transform 0.3s ease;
    
  }
  .img img:hover {
   transform: scale(1.05); /* Slightly zoom in on hover */
   box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); /* Increase box shadow on hover */
  }
  .text_of_img {
    
   max-width: 50%; /* Ensure the text doesn’t overflow */
   left: 40px;
   position: relative;
}

.text_of_img h3 {
  font-family: 'Arial', sans-serif;
  color: #757575;
  font-size: 39px;
  margin: 0;
  font-family: "Lilita One", sans-serif;
  font-weight: 400;
  font-style: normal;
}
  
  </style>
  