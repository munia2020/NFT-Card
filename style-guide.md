# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

## Colors

### Primary

- Soft blue: hsl(215, 51%, 70%)
- Cyan: hsl(178, 100%, 50%)

### Neutral

- Very dark blue (main BG): hsl(217, 54%, 11%)
- Very dark blue (card BG): hsl(216, 50%, 16%)
- Very dark blue (line): hsl(215, 32%, 27%)
- White: hsl(0, 0%, 100%)

## Typography

### Body Copy

- Font size (paragraph): 18px

### Font

- Family: [Outfit](https://fonts.google.com/specimen/Outfit)
- Weights: 300, 400, 600



<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  <link rel="stylesheet" href="./styles/style.css">
  <title>Frontend Mentor | NFT preview card component</title>

  <style>

  </style>
</head>
<body>
  <main class="card_container">
    <div class="img_container">
      <img src="./images/image-equilibrium.jpg" alt="Ethereum">
    </div>
    <div class="title_card_container">
      <h3>Equilibrium #3429</h3>
    </div>
    <div class="text_container">
      <span>
        Our Equilibrium collection promotes balance and calm.
      </span>
    </div>
    <div class="info_card_container">
      <div class="eth_container">
        <img src="./images/icon-ethereum.svg" alt="Ethereum logo">
        <span class="eth">0.041 ETH</span> 
      </div>
      <div class="clock_container">
        <img src="./images/icon-clock.svg" alt="Clock logo">
        <span class="days_left">3 days left</span>
      </div>
       
    </div>
    <div class="autor_container">
      <div class="img_avatar_container">
        <img src="./images/image-avatar.png" alt="Avatar of Jules Wyvern">
      </div>
      <p>Creation of <span> Jules Wyvern</span></p>
    </div>
    
    
  </main>


  <div class="attribution">
    <span>Challenge by</span> <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    <span>Coded by</span> <a href="#">Cristian Mariño</a>.
  </div>
</body>
</html>








  
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');

:root{
    --softBlue: hsl(215, 51%, 70%);
    --Cyan: hsl(178, 100%, 50%);
    --veryDarkBlueMain: hsl(217, 54%, 11%);
    --veryDarkBlueCard: hsl(216, 50%, 16%);
    --veryDarkBlueLine: hsl(215, 32%, 27%);
    --white: hsl(0, 0%, 100%);
    font-family: 'Outfit', sans-serif;;
}

*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body{
    background-color: var(--veryDarkBlueMain);
}

main{
    background-color: var(--veryDarkBlueCard);
    margin-bottom: 10px;
}

.title_card_container h3{
    color: var(--white);
    margin-left: 24px;
    font-weight: 600;
}

.text_container span{
    color: var(--softBlue);
    text-align: center;
    font-weight: 300;
    line-height: 25px;
}

.text_container{
    margin-left: 24px;
    margin-top: 10px;
    margin-bottom: 20px;
}

.eth_container span{
    color: var(--Cyan);
    font-weight: 400;
}

.clock_container span{
    color: var(--softBlue);
    font-weight: 300;
}

.info_card_container{
    display: flex;
    border-bottom: solid 0.1px var(--veryDarkBlueLine);
    justify-content: space-between;
    width: 85%;
    margin-left: 24px;
    padding-bottom: 15px;
}

.img_avatar_container{
    width: 11%;
    margin-left: 25px;
}

.autor_container{
    display: flex;
    margin-top: 10px;
    width: 85%;
    padding-top: 4px;
    padding-bottom: 20px;
}

.autor_container p{
    margin-left:13px;
    margin-top: 5px;
    color: var(--softBlue);
}

.autor_container span{
    color: var(--white);
    font-weight: 300;
}

.img_avatar_container img{
    max-width: 100%;
    border-radius: 50%;
    border: solid 1px var(--white);
}

@media only screen and (max-width:1440px) {
    body{
        display: flex;
        flex-direction: column;
        align-items: center;
        
    }
    main{
        width: 22%;
        margin-top: 40px;
        border-radius: 15px;
    }
    .img_container{
        width: 85%;
        margin-top: 20px;
        margin-left: 24px;
    }
    .img_container img{
        max-width: 100%;
        border-radius: 10px;
    }
    .title_card_container{
        margin-top: 20px;
    }   
    .text_container span{
        padding-right: 35px;
    }
}

@media only screen and (max-width:375px) {
    body{
        display: flex;
        flex-direction: column;
        align-items: center;
        
    }
    main{
        width: 85%;
        margin-top: 50px;
        border-radius: 15px;
    }
    .img_container{
        width: 85%;
        margin-top: 20px;
        margin-left: 24px;
    }
    .img_container img{
        max-width: 100%;
        border-radius: 10px;
    }
    .title_card_container{
        margin-top: 20px;
    }   
}


.attribution { font-size: 11px; text-align: center; }
.attribution a { color: var(--softBlue); }
.attribution span { color: var(--white); }