<template>
    <div class="header-wrapper">
        <div class="header-logo">
            <a href="#">
                <img src="../assets/10.png" alt="">
            </a>
        </div>
        <div class="header-options">
            <ul>
                <li>Home</li>
                <li>about us</li>
                <li>service</li>
                <li>portfolio</li>
                <li>Blog</li>
            </ul>
        </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Header',
  
  }
  </script>
  <style scoped>
  .header-wrapper{
    float: left;
    width: 100%;
    background-color: rgb(252, 248, 248);
    display: flex;
    justify-content: space-between;
  }
  .header-logo,.header-options{
    margin: 16px 30px;
  }
  .header-options ul{
    padding: 0;
    margin: 0%;
    display: flex;
  }
  .header-options ul li{
    list-style: none;
    font-size: 17px;
    font-weight: 600;
    padding: 0 10px;
  }
  </style>