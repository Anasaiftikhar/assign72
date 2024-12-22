<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Animation</title>
        <style>
            body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #db2828;
  }
  
  
  .text-slider {
    position: relative;
    width: 200px;  /* Set the width for your text container */
    height: 40px;  /* Set the height to fit your text */
    overflow: hidden;
    text-align: center;
  }
  
  
  .text {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    font-size: 24px;
    font-weight: bold;
    color: #333;
    opacity: 0; /* Initially hidden */
    animation: changeText 8s infinite;
  }
  
  
  @keyframes changeText {
    0% {
      opacity: 0;
      transform: translateY(100%);  
    }
    20% {
      opacity: 1;
      transform: translateY(0);  
    }
    25% {
      opacity: 1;
      transform: translateY(0);  
    }
    45% {
      opacity: 0;
      transform: translateY(-100%);  
    }
    100% {
      opacity: 0;
      transform: translateY(100%); 
    }
  }
  
  
  .text:nth-child(1) {
    animation-delay: 0s;
  }
  
  .text:nth-child(2) {
    animation-delay: 2s;
  }
  
  .text:nth-child(3) {
    animation-delay: 4s;
  }
  
  .text:nth-child(4) {
    animation-delay: 6s;
  }
        </style>
    </head>
    <body>
        <h2>
            Hello
        </h2>
            <div class="text-slider">
                <span class="text">Bob!</span>
                <span class="text">Everybody!</span>
                <span class="text">User!</span>
                <span class="text">World!</span>
            </div>
    </body>
</html>
