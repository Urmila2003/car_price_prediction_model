<!DOCTYPE html> 
<html lang="en"> 
  
<head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" 
          content="width=device-width,initial-scale=1.0"> 
    <title>Car Price Prediction</title>
    </head> 
  
<body>
  <style>
    body { 
    margin: 0; 
    display: flex; 
    align-items: center; 
    justify-content: space-around; 
    flex-direction: column; 
    height: 100vh; 
    background-color:#F7EFED; 
    font-family: 'Poppins', sans-serif;
    }
    .radio-group { 
    display: flex; 
    margin-bottom: 16px; 
    }
input[type="radio"] { 
    margin-right: 8px; 
} 
  select{
          display:block;
          background-color: rgba(0,0,80,0.3);
          border-radius: 0;
          font-size: 16px;
          margin:auto;
          padding: 4px;
          border: 0;
          box-shadow: 0 0 12px rgba(0,0,255,0.4); 
		}
label { 
    display: block; 
    margin-bottom: 8px; 
    font-size: 17px; 
    color: green; 
    font-weight: 600; 
} 
i { 
    margin-right: 3px;
    color:green;
}
h1 { 
color: green; 
}
h3
{ color:green;
}

.slider {
  -webkit-appearance: none;
  width: 100%;
  height: 15px;
  border-radius: 5px;  
  background: #d3d3d3;
  outline: none;
  opacity: 0.7;
  -webkit-transition: .2s;
  transition: opacity .2s;
}
.slider:hover {
  opacity: 1; /* Fully shown on mouse-over */
}
var slider = document.getElementById("myRange");
var output = document.getElementById("demo");
output.innerHTML = slider.value; // Display the default slider value

// Update the current slider value (each time you drag the slider handle)
slider.oninput = function() {
  output.innerHTML = this.value;
}
  </style>
    <h1>Car Price Prediction</h1> 
    <div class="form-box"> 
        <div class="textup"> 
            <i class="fa fa-solid fa-clock"></i> 
            <h3>Let's start!!</h3>
            <br></br>
            <label> 
                <i class="fa-solid fa-face-smile"></i> 
                Fuel Type 
            </label> 
            <div class="radio-group"> 
                <input type="radio" id="Diesel" 
                       name="satisfy" value="Diesel" checked> 
                <label for="Diesel">Diesel</label> 
  
                <input type="radio" id="Petrol" 
                       name="satisfy" value="Petrol"> 
                <label for="Petrol">Petrol</label>
               
                <input type="radio" id="CNG" 
                       name="satisfy" value="CNG"> 
                <label for="CNG">CNG</label>
            </div> 
            <h3></h3>
  
             <label> 
                <i class="fa-solid fa-face-smile"></i> 
                Transmission Type 
            </label>
            <div class="radio-group"> 
                <input type="radio" id="Manual" 
                       name="satisfy" value="Manual" checked> 
                <label for="Manual">Manual</label> 
  
                <input type="radio" id="Automatic" 
                       name="satisfy" value="Automatic"> 
                <label for="Automatic">Automatic</label>
                </div>
                <h3></h3>
                
                <label> 
                <i class="fa-solid fa-face-smile"></i> 
                Are you a Dealer or Individul? 
            </label>
            <div class="radio-group"> 
                <input type="radio" id="Dealer" 
                       name="satisfy" value="Dealer" checked> 
                <label for="Dealer">Dealer</label> 
  
                <input type="radio" id="Individual" 
                       name="satisfy" value="Individual"> 
                        <label for="Individual">Individual</label>
                </div>
                <h3></h3>
        <label for="Cars">Number of owners the car previously had</label>
    <select name="Cars" id="Cars">
      <option value="0">0</option>
      <option value="1">1</option>
      <option value="2">2</option>
      <option value="3">3</option>
    </select>  
    <div class="slidecontainer">
      <label>Current Ex-showroom price of the car</label>
  <input type="range" min="2" max="25" value="23" class="slider" id="myRange">
</div>

<div class="slidecontainer">
      <label>In which year the car was purchased</label>
  <input type="range" min="1990" max="2024" value="34" class="slider" id="myRange">
</div>
                
        </div> 
        </body>
        </html>
