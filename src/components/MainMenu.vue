<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light fixed-top">
      <div class="container">
        <!-- Logo centered -->
        <div class="row justify-content-center">
          <div class="col text-center">
            <a class="navbar-brand" href="#">
              <img src="@/assets/logo.png" alt="Logo" class="logo">
            </a>
          </div>
        </div>
        
        <!-- Navigation links centered -->
        <div class="row justify-content-center">
          <div class="col">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
              <ul class="navbar-nav">
                <li class="nav-item">
                  <router-link :to="{ name: 'Models' }" class="nav-link" exact active-class="active">Models</router-link>
                </li>
                <li class="nav-item">
                  <router-link :to="{ name: 'Colors' }" class="nav-link" active-class="active">Colors</router-link>
                </li>
                <li class="nav-item">
                  <router-link :to="{ name: 'Accessories' }" class="nav-link" active-class="active">Accessories</router-link>
                </li>
                <li class="nav-item">
                  <router-link :to="{ name: 'Summary' }" class="nav-link" active-class="active">Summary</router-link>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: "MainMenu",
  };
  </script>
  
  <style scoped>
  .navbar {
    padding: 1rem;
  }
  
  .navbar-brand .logo {
    width: 50px;
    height: auto;
  }
  
  .navbar-nav .nav-link {
    font-weight: bold;
    color: grey; /* Default text color */
  }
  
  .navbar-nav .nav-link.active {
    color: black; /* Active page text color */
  }
  
  .navbar-nav .nav-link:hover {
    color: #6c757d; /* Hover text color */
  }
  </style>
  