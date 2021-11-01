# Phones Online Store

Buying phones from the store

## Description
This website was created to help people to buy phone online 
phones store contain three brand's Apple, Samsung, and Huawei user choose the brand then all products of those brands will be displayed with the price
he can choose any one of them to add to the cart then buy it

## Executing program

* main.js 

```
 fetch("https://api-mobilespecs.azharimm.site/v2/brands/apple-phones-48?page=2")
    .then(function(response) {
        return response.json()
        
    })
    .then(function(json) {
        document.getElementById("formCart").style.display = "none";
        document.getElementById('apple').addEventListener('click', function() {
            document.getElementById("grid-container2").style.display = "none";
            document.getElementById("grid-container3").style.display = "none";
            document.getElementById("grid-container1").style.display = "block";
            document.getElementById("formCart").style.display = "none";

            let searchButton = document.getElementById('search-button');
            let searchInput = document.getElementById('input1');

            let pro1 = document.getElementById('grid-container1')
            let index
            let pic = document.createElement('img')
            let name2 = document.createElement('h5')
            let total = 0
       
         

            for (i = 0; i < json.data.phones.length; i++) {


                let p1 = document.createElement('img')
                let g1 = document.createElement('div')
                g1.className = 'grid-item'
                pro1.appendChild(g1)
                p1.className = 'img1'
                p1.src = json.data.phones[i].image
                    // p1.style = 'width: 100px'

                let h = document.createElement('h4')
                h.className = 'name1'
                h.innerText = json.data.phones[i].phone_name
                let pr = document.createElement('h5')
                pr.className = 'price1'

                price = Math.floor(Math.random() * (3000 - 2000 + 1) + 2000)
                pr.innerText = price + ' SAR'
                let cart = document.createElement('button')
                cart.id = 'shop'
                cart.className = 'cart1 '
                cart.innerText = 'Add to cart'

                g1.appendChild(p1)
                g1.appendChild(h)
                g1.appendChild(pr)
                g1.appendChild(cart)


                pic = p1


                let arr = document.querySelectorAll(".grid-item")

```

## The used API

Phone Specifications API
it's contain many brands with detials 
like Apple ,Samsung ,Huawei,Acer and more brands 
API link: https://github.com/azharimm/phone-specs-api
