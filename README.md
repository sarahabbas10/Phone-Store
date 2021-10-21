# Phones Online Store

Buying phones from the store

## Description
This website was created to help people to buy phone online 
phones store contain three brand's Apple, Samsung, and Huawei user choose the brand then all products of those brands will be displayed with the price
he can choose any one of them to add to the cart then buy it

## Executing program

* index.html

```
  <!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-uWxY/CJNBR+1zjPWmfnSnVxwRheevXITnMqoEIeG1LJrdI0GlVs/9cVSyPYXdcSF" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link rel="stylesheet" href="style.css">

</head>

<body>
    <script src="main.js"></script>
    <nav class="navbar navbar-expand-lg navbar-light bg-light ">
        <div class="cart"> <button id="mycart" style="font-size:24px">my cart <i class="fa fa-shopping-cart"></i></button></div>
        <ul class="nav justify-content-end">
            <li class="nav-item">
                <a class="nav-link" href="sign up in.html">Create Account/Login</a>
            </li>
        </ul>
    </nav>

    <div class="row">
        <div class="logo-content">
            <img class="logoimg " src="products.jpg">
            <h1 id=h1>Welecome to Apple Store</h1>
        </div>
    </div>

    <br><br>
    <!-- <form class="example" style="margin:auto;max-width:300px">
        <input class="input1" type="text" placeholder="Search.." name="search2">
        <button id='search-button' class="search-button" type="submit"><i class="fa fa-search"></i></button>
    </form> -->
    <br><br>
    <div class='containar'>
        <div class="productsF">
            <img class='phone' src="applep.jpg" alt=""> <br>
            <button id='apple' class=btn>Apple Products</button>
        </div>
        <div id='grid-container1'></div>
        <br><br>
        <div class="productsS">
            <img class='phone' src="huawei.jpg" alt=""><br>
            <button id='huawei' class=btn>Huawei Products</button>
        </div>
        <div id='grid-container2'></div>
        <br><br>
        <div class="productsT">
            <img class='phone' src="samsung.webp" alt=""><br>
            <button id='samsung' class=btn>Samsung Products</button>
        </div>
        <div id='grid-container3'></div>

        <br><br>
        <br><br>
    </div>
    <div id='formCart' class="formCart">
        <label class='cartColumn'>Shopping Cart</label>
        <div id='carts' class='cart-items'>
            <label class='itemColumn'>Items</label>
            <label class='model'>Model</label>
            <label class='pricelColumn'>Price</label>
            <br><br>
        </div>
        <div class="cart-items">
            <label id="total" class='itemColumn'>Total Price: </label>
        </div>
        <button class="pur">PURCHASE</button>

    </div>



</body>

</html>
```

## The used API

Phone Specifications API
it's contain many brands with detials 
like Apple ,Samsung ,Huawei,Acer and more brands 
API link: https://github.com/azharimm/phone-specs-api
