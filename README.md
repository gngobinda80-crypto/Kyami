
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>KYAMI CLOTH | Online Fashion Store</title>

<!-- Google AdSense -->
<!-- AdSense approval ke baad apna REAL publisher ID yahan lagayen -->
<script async
src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
crossorigin="anonymous"></script>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Arial,sans-serif;
}

body{
  background:#f5f5f5;
  color:#222;
}

/* HEADER */
header{
  position:sticky;
  top:0;
  z-index:1000;
  background:#111;
  color:white;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:16px 5%;
}

.logo{
  font-size:25px;
  font-weight:bold;
  letter-spacing:2px;
}

.cart-btn{
  border:0;
  background:white;
  color:#111;
  padding:10px 17px;
  border-radius:25px;
  font-weight:bold;
  cursor:pointer;
}

/* ADS */
.ad-box{
  width:100%;
  min-height:90px;
  display:flex;
  align-items:center;
  justify-content:center;
  background:#fff;
  margin:15px 0;
  overflow:hidden;
}

.ad-label{
  color:#999;
  font-size:12px;
}

/* HERO */
.hero{
  min-height:430px;
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  color:white;

  background:
  linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
  url("https://images.unsplash.com/photo-1445205170230-053b83016050?auto=format&fit=crop&w=1600&q=80")
  center/cover;
}

.hero h1{
  font-size:55px;
  margin-bottom:12px;
}

.hero p{
  font-size:20px;
  margin-bottom:25px;
}

.shop-btn{
  display:inline-block;
  padding:14px 30px;
  background:white;
  color:#111;
  border-radius:30px;
  text-decoration:none;
  font-weight:bold;
}

/* CONTROLS */
.controls{
  padding:30px 5%;
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:10px;
}

#search{
  width:280px;
  padding:13px 18px;
  border:1px solid #ddd;
  border-radius:25px;
  outline:none;
}

.category{
  border:0;
  padding:12px 20px;
  border-radius:25px;
  cursor:pointer;
  background:#ddd;
}

.category.active{
  background:#111;
  color:white;
}

/* PRODUCTS */
.products{
  padding:10px 5% 50px;
  display:grid;
  grid-template-columns:
  repeat(auto-fit,minmax(220px,1fr));
  gap:25px;
}

.product{
  background:white;
  border-radius:15px;
  overflow:hidden;
  box-shadow:0 4px 18px rgba(0,0,0,.08);
  transition:.3s;
}

.product:hover{
  transform:translateY(-5px);
}

.product img{
  width:100%;
  height:280px;
  object-fit:cover;
}

.product-info{
  padding:18px;
}

.product-info h3{
  margin-bottom:8px;
}

.price{
  font-size:20px;
  font-weight:bold;
  margin:10px 0;
}

.old-price{
  font-size:14px;
  color:#999;
  text-decoration:line-through;
}

.add{
  width:100%;
  padding:12px;
  background:#111;
  color:white;
  border:0;
  border-radius:8px;
  cursor:pointer;
}

/* CART */
.cart{
  position:fixed;
  top:0;
  right:-420px;
  width:380px;
  max-width:90%;
  height:100vh;
  background:white;
  z-index:2000;
  padding:25px;
  box-shadow:-5px 0 20px rgba(0,0,0,.25);
  transition:.3s;
  overflow-y:auto;
}

.cart.open{
  right:0;
}

.close{
  float:right;
  border:0;
  background:#eee;
  padding:8px 12px;
  border-radius:50%;
  cursor:pointer;
}

.cart h2{
  margin:10px 0 25px;
}

.cart-item{
  border-bottom:1px solid #ddd;
  padding:14px 0;
}

.qty{
  display:flex;
  align-items:center;
  gap:10px;
  margin-top:8px;
}

.qty button{
  border:0;
  padding:5px 10px;
  cursor:pointer;
}

.remove{
  color:red;
  background:none;
  border:0;
  cursor:pointer;
}

.total{
  font-size:22px;
  font-weight:bold;
  margin:25px 0;
}

.whatsapp{
  display:block;
  text-align:center;
  background:#25D366;
  color:white;
  text-decoration:none;
  padding:14px;
  border-radius:8px;
  font-weight:bold;
}

/* FOOTER */
footer{
  background:#111;
  color:white;
  text-align:center;
  padding:35px 15px;
}

/* MOBILE */
@media(max-width:600px){

  .hero{
    min-height:370px;
  }

  .hero h1{
    font-size:38px;
  }

  .products{
    grid-template-columns:repeat(2,1fr);
    padding:10px 12px 40px;
    gap:12px;
  }

  .product img{
    height:210px;
  }

  .product-info{
    padding:12px;
  }

  .product-info h3{
    font-size:15px;
  }

  .price{
    font-size:17px;
  }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>

  <div class="logo">
    KYAMI CLOTH
  </div>

  <button class="cart-btn" onclick="openCart()">
    🛒 Cart (<span id="count">0</span>)
  </button>

</header>


<!-- TOP AD -->
<div class="ad-box">

  <!--
  AdSense code yahan paste karein
  AdSense approval ke baad.
  -->

  <span class="ad-label">
    Advertisement
  </span>

</div>


<!-- HERO -->
<section class="hero">

  <div>

    <h1>KYAMI CLOTH</h1>

    <p>
      Style That Speaks For You
    </p>

    <a href="#shop" class="shop-btn">
      SHOP NOW
    </a>

  </div>

</section>


<!-- SECOND AD -->
<div class="ad-box">

  <span class="ad-label">
    Advertisement
  </span>

</div>


<!-- SEARCH + CATEGORY -->
<section class="controls" id="shop">

  <input
    id="search"
    type="text"
    placeholder="🔍 Search clothes..."
    onkeyup="searchProducts()"
  >

  <button
    class="category active"
    onclick="filterProducts('all',this)">
    All
  </button>

  <button
    class="category"
    onclick="filterProducts('Men',this)">
    Men
  </button>

  <button
    class="category"
    onclick="filterProducts('Women',this)">
    Women
  </button>

  <button
    class="category"
    onclick="filterProducts('Kids',this)">
    Kids
  </button>

</section>


<!-- PRODUCTS -->
<section class="products" id="products">


<!-- PRODUCT 1 -->

<div
class="product"
data-category="Men"
data-name="Premium T Shirt">

<img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<h3>Premium T-Shirt</h3>

<div class="price">
₹499
<span class="old-price">₹799</span>
</div>

<button
class="add"
onclick="addToCart('Premium T-Shirt',499)">
Add to Cart
</button>

</div>
</div>


<!-- PRODUCT 2 -->

<div
class="product"
data-category="Women"
data-name="Fashion Dress">

<img src="https://images.unsplash.com/photo-1595777457583-95e059d581b8?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<h3>Fashion Dress</h3>

<div class="price">
₹899
<span class="old-price">₹1299</span>
</div>

<button
class="add"
onclick="addToCart('Fashion Dress',899)">
Add to Cart
</button>

</div>
</div>


<!-- PRODUCT 3 -->

<div
class="product"
data-category="Men"
data-name="Casual Shirt">

<img src="https://images.unsplash.com/photo-1602810318383-e386cc2a3ccf?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<h3>Casual Shirt</h3>

<div class="price">
₹699
<span class="old-price">₹999</span>
</div>

<button
class="add"
onclick="addToCart('Casual Shirt',699)">
Add to Cart
</button>

</div>
</div>


<!-- PRODUCT 4 -->

<div
class="product"
data-category="Women"
data-name="Women Top">

<img src="https://images.unsplash.com/photo-1551488831-00ddcb6c6bd3?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<h3>Women Top</h3>

<div class="price">
₹599
<span class="old-price">₹899</span>
</div>

<button
class="add"
onclick="addToCart('Women Top',599)">
Add to Cart
</button>

</div>
</div>


<!-- PRODUCT 5 -->

<div
class="product"
data-category="Kids"
data-name="Kids T Shirt">

<img src="https://images.unsplash.com/photo-1519238263530-99bdd11df2ea?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<h3>Kids T-Shirt</h3>

<div class="price">
₹349
<span class="old-price">₹499</span>
</div>

<button
class="add"
onclick="addToCart('Kids T-Shirt',349)">
Add to Cart
</button>

</div>
</div>


<!-- PRODUCT 6 -->

<div
class="product"
data-category="Men"
data-name="Premium Hoodie">

<img src="https://images.unsplash.com/photo-1556821840-3a63f95609a7?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<h3>Premium Hoodie</h3>

<div class="price">
₹999
<span class="old-price">₹1499</span>
</div>

<button
class="add"
onclick="addToCart('Premium Hoodie',999)">
Add to Cart
</button>

</div>
</div>

</section>


<!-- MIDDLE AD -->
<div class="ad-box">

  <span class="ad-label">
    Advertisement
  </span>

</div>


<!-- FOOTER -->
<footer>

<h3>KYAMI CLOTH</h3>

<p>
Premium Fashion • Best Prices • Easy Ordering
</p>

<br>

<p>
© 2026 KYAMI CLOTH
</p>

</footer>


<!-- CART -->
<div class="cart" id="cart">

<button
class="close"
onclick="closeCart()">
✕
</button>

<h2>🛒 Your Cart</h2>

<div id="cartItems"></div>

<div class="total">

Total: ₹<span id="total">0</span>

</div>

<a
id="whatsapp"
class="whatsapp"
target="_blank"
href="#">

📲 Order on WhatsApp

</a>

</div>


<script>

let cart = [];


/* ADD PRODUCT */

function addToCart(name,price){

  let existing =
  cart.find(item => item.name === name);

  if(existing){

    existing.quantity++;

  }else{

    cart.push({
      name:name,
      price:price,
      quantity:1
    });

  }

  updateCart();

  alert("Product added to cart!");

}


/* UPDATE CART */

function updateCart(){

  let html = "";
  let total = 0;
  let count = 0;

  cart.forEach((item,index)=>{

    total +=
      item.price * item.quantity;

    count += item.quantity;

    html += `

      <div class="cart-item">

        <b>${item.name}</b>

        <p>
          ₹${item.price}
        </p>

        <div class="qty">

          <button
          onclick="changeQty(${index},-1)">
          −
          </button>

          <span>
          ${item.quantity}
          </span>

          <button
          onclick="changeQty(${index},1)">
          +
          </button>

        </div>

        <br>

        <button
        class="remove"
        onclick="removeItem(${index})">

        Remove

        </button>

      </div>
    `;
  });


  document.getElementById("cartItems")
  .innerHTML =
  html || "<p>Your cart is empty.</p>";

  document.getElementById("total")
  .innerText = total;

  document.getElementById("count")
  .innerText = count;


  /* WHATSAPP MESSAGE */

  let message =
  "Hello KYAMI CLOTH!%0A%0AI want to order:%0A";

  cart.forEach(item=>{

    message +=
    "- " +
    item.name +
    " x" +
    item.quantity +
    " = ₹" +
    (item.price * item.quantity) +
    "%0A";

  });

  message +=
  "%0ATotal: ₹" + total;


  /*
  IMPORTANT:
  919999999999 ko apne
  WhatsApp number se replace karein.
  */

  document.getElementById("whatsapp").href =
  "https://wa.me/919999999999?text=" +
  message;

}


/* QUANTITY */

function changeQty(index,amount){

  cart[index].quantity += amount;

  if(cart[index].quantity <= 0){

    cart.splice(index,1);

  }

  updateCart();

}


/* REMOVE */

function removeItem(index){

  cart.splice(index,1);

  updateCart();

}


/* OPEN CART */

function openCart(){

  document
  .getElementById("cart")
  .classList.add("open");

}


/* CLOSE CART */

function closeCart(){

  document
  .getElementById("cart")
  .classList.remove("open");

}


/* CATEGORY FILTER */

function filterProducts(category,button){

  document
  .querySelectorAll(".category")
  .forEach(btn =>
    btn.classList.remove("active")
  );

  button.classList.add("active");


  document
  .querySelectorAll(".product")
  .forEach(product=>{

    if(
      category === "all" ||
      product.dataset.category === category
    ){

      product.style.display =
      "block";

    }else{

      product.style.display =
      "none";

    }

  });

}


/* SEARCH */

function searchProducts(){

  let search =
  document
  .getElementById("search")
  .value
  .toLowerCase();


  document
  .querySelectorAll(".product")
  .forEach(product=>{

    let name =
    product.dataset.name
    .toLowerCase();


    product.style.display =
    name.includes(search)
    ? "block"
    : "none";

  });

}

</script>

</body>
</html>
