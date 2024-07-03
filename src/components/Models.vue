<template>
    <div class="car-details-container">
      <!-- Car Card -->
      <div class="car-card">
        <div class="car-background">
          <h2 class="car-title">IBIZA</h2>
        </div>
        <img src="..\assets\car.png" alt="Car Image" class="car-image">
        <div class="car-details">
          <p class="car-price">193.500 TL'den başlayan fiyatlarla</p>
          <button class="btn btn-select">Select</button>
        </div>
        <!-- Next Page Box -->
        <div class="next-page-box">
          <!-- Left Side: Small Photo of Car -->
          <div class="left-content">
            <img src="..\assets\car.png" alt="Small Car Photo" class="small-car-photo">
          </div>
          
          <!-- Middle: Total and Price -->
          <div class="middle-content">
            <p>Total</p>
            <p>193.500 TL</p>
          </div>
          
          <!-- Right: Button -->
          <div class="right-content">
            <button class="btn btn-primary">
              <span class="btn-text">Next Page</span>
              <span class="arrow-icon">&rarr;</span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "CarDetails",
  };
  </script>
  
  <style scoped>
  .car-details-container {
    display: flex;
    justify-content: center; /* Center horizontally */
    align-items: center; /* Center vertically */
    height: 100vh; /* Full viewport height */
  }
  
  .car-card {
    width: 600px; /* Adjust width as needed */
    background-color: #f8f9fa;
    padding: 20px;
    border: 1px solid #dee2e6;
    border-radius: 8px;
    margin-bottom: 20px;
    position: relative;
    overflow: hidden; /* Ensure overflow doesn't affect layout */
    transition: box-shadow 0.3s ease; /* Smooth transition for box-shadow */
  }
  
  .car-card:hover {
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.1); /* Shadow effect on hover */
  }
  
  .car-background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent background */
  }
  
  .car-title {
    font-size: 5rem; /* Adjust font size as needed */
    color: #fff; /* Text color */
    margin: 0;
    padding: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  
  .car-image {
    max-width: 100%;
    height: auto;
    transition: transform 0.3s ease; /* Smooth transition for transform */
  }
  
  .car-image:hover {
    transform: scale(1.05); /* Scale up on hover */
  }
  
  .car-details {
    text-align: center;
  }
  
  .car-price {
    font-size: 1.5rem; /* Adjust font size as needed */
    margin-bottom: 10px;
  }
  
  .btn-select, .btn-primary {
    background-color: #000;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease; /* Smooth transition for background-color */
  }
  
  .btn-select:hover, .btn-primary:hover {
    background-color: #333; /* Darker background on hover */
  }
  
  .next-page-box {
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    background-color: #f8f9fa;
    border: 1px solid #dee2e6;
    border-radius: 8px;
  }
  
  .left-content {
    display: flex;
    align-items: center;
  }
  
  .small-car-photo {
    width: 60px; /* Adjust size as needed */
    height: auto;
    margin-right: 10px;
  }
  
  .middle-content {
    flex-grow: 1;
    text-align: center;
  }
  
  .right-content {
    text-align: right;
  }
  
  .btn-text {
    color: #fff;
    margin-right: 10px;
  }
  
  .arrow-icon {
    font-size: 1.2rem;
    transform: scaleX(-1); /* Flips the arrow horizontally */
  }
  </style>
  