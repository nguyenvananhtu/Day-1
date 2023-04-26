<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Product card</title>
    <link rel="stylesheet" href="card.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@700&display=swap" rel="stylesheet">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
</head>
<style>
    *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
:root{
    --prinary-color:#a5ebb5;
    --prinary-color1:#528f89;
}
body{
    height: 100vh;
    background: linear-gradient(to right,#e7461e,#374272);
    font-family: 'Poppins', sans-serif;
}
.card{
    margin: 120px auto;
    width: 320px;
    height: 370px;
    background: linear-gradient(to top, #7c1d05,#374272);
    border-radius: 20px;
    padding: 20px;
    color: white;
    position: relative;
}
.card_cart,
.card_heart{
    font-weight: bold;
    font-size: 25px;
    position: absolute;
    left: 20px;
    top: 15px;
}
.card_cart i{
    cursor: pointer;
}
.card_heart i{
    cursor: pointer;
}
.card_cart{
    left: unset;
    right: 20px;
}
.card_img{
    width: 77%;
    transition: 0.5s;
    margin: 0px auto;
    transition: transform .2s;
}
.card_img img{
    width: 100%;
    height: 100%;
}
.card_title, .card_price{
    font-size: 20px;
    text-align: center;
    font-weight: bold;
}
.card_title{
    color:white;
}
.card_size,.card_color{
   display: flex;
   align-items: center;
   margin-bottom: 10px;
}

.card_color{
    margin-left: 75px;
}
.card_action{
    margin-left: 30px;
}

.card_color span{
    width: 35px;
    height: 35px;
    border-radius: 20%;
    margin: 0px 3px;
    cursor: pointer;
    border: 0.5px solid black;
}
.card_color_blue{
    background-color: blue;
}
.card_color_red{
    background-color: red;
}
.card_color_green{
    background-color: orange;
}
.card_action button{
    background: linear-gradient(to right,#e7461e,#374272);
    color: white;
    font-weight: bold;
    border-radius: 5px;
    border: none;
    padding: 10px 20px;
    margin: 0px 5px;
    outline: none;
    cursor: pointer;
}
.card:hover .card_img{
    transform: scale(1.5);
}
.card:hover .card_title{
   transform: translate(50px, -45px);
   margin-left: -100px;
}
.card:hover .card_price{
    transform: translate(0px, -45px);
}
.card_title,.card_price,.card_color,.card_size,.card_action button{
    transition: 0.5s;
}
.card_size{
    margin-top: 200px;
}
.card_color,.card_action{
   visibility: hidden;
   opacity: 0;
   transition-delay: 0.2s;
   
}

.card:hover .card_color,
.card:hover .card_action
{
    visibility: visible;
    opacity: 100;

}
.card:hover .card_color{
    margin-top: -30px;
    
}
.card_action button{
    font-family: 'Poppins', sans-serif;
    font-weight: bold;
    transition: 0.3s;
}
.card_action button:hover{
    transform: scale(1.2);
    background-color: var(--prinary-color1);
}
</style>
<body>
    <div class="card">
        <div class="card_heart">
            <i class='bx bx-heart'></i>
        </div>
        <div class="card_cart">
            <i class='bx bx-cart'></i>
        </div>
        <div class="card_img">
            <img src="https://o.remove.bg/downloads/22e73c7a-2c9f-44c8-b803-413ab44c952d/1455765015_ban_phim_gae_thu_marvo_k828-removebg-preview.png" alt="">
        </div>
        <div class="card_title">
            GAMING KEYBOARD
        </div>
        <div class="card_price">
            $100
        </div>
        
        <div class="card_color">
            <span class="card_color_blue"></span>
            <span class="card_color_red"></span>
            <span class="card_color_green"></span>
        </div>
        <div class="card_action">
            <button>Buy Now</button>
            <button>Add Cart</button>
        </div>
    </div>
</body>
</html>
