<script></script>

<template>
    <nav class="navbar">
      <div class="logo">
        <img class="logo" src="..\assets\img\Logo.jpg" alt="Logo">
      </div>
      <ul class="nav-links">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Academics</a></li>
        <li><a href="#">Courses</a></li>
        <li><a href="#">News</a></li>
      </ul>
    </nav>
    
    </template>
    
    <style scoped>
    
    .navbar {
      background-color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0px;
    }
    
    .nav-links{
        margin-right: 10rem;
        font-weight: bolder;
        
    }
    
    .nav-links li {
      display: inline-block;
      margin-right: 1rem;
    }
    
    .nav-links li:first-child {
      margin-left: 0;
    }
    
    .nav-links li a {
      color: black;
      text-decoration: none;
    }
    
    .logo {
      width: 120px;
      margin-left: 8rem;
      margin-bottom: -1.5rem;
      
    }
    
    </style>