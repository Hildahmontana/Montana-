# montana-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Montana Brand</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      display: grid;
      grid-template-rows: auto 1fr auto;
      grid-template-columns: 1fr;
      min-height: 100vh;
    }

    header, footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 1em;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 2em;
      margin-top: 1em;
    }

    main {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2em;
      padding: 2em;
    }

    .product {
      border: 1px solid #ccc;
      padding: 1em;
      text-align: center;
    }

    .cart {
      position: fixed;
      top: 1em;
      right: 1em;
      background: white;
      border: 1px solid #ccc;
      padding: 1em;
      z-index: 100;
    }

    button {
      padding: 0.5em 1em;
      margin-top: 1em;
      background-color: #333;
      color: white;
      border: none;
      cursor: pointer;
    }

    button:hover {
      background-color: #555;
    }
  </style>
</head>
<body>
  <header>
    <h1>Montana Brand</h1>
    <p>Placeholder for powerful brand messaging here.</p>
    <nav>
      <a href="#" style="color:white">Home</a>
      <a href="#" style="color:white">Shop</a>
      <a href="#" style="color:white">About</a>
      <a href="#" style="color:white">Contact</a>
    </nav>
  </header>

  <div class="cart" id="cart">
    Cart: <span id="cart-count">0</span> items
  </div>

  <main>
    <div class="product">
      <h2>Product 1</h2>
      <p>$10</p>
      <button onclick="addToCart()">Add to Cart</button>
    </div>
    <div class="product">
      <h2>Product 2</h2>
      <p>$15</p>
      <button onclick="addToCart()">Add to Cart</button>
    </div>
    <div class="product">
      <h2>Product 3</h2>
      <p>$20</p>
      <button onclick="addToCart()">Add to Cart</button>
    </div>
  </main>

  <footer>
    <p>&copy; 2025 Montana Brand. All rights reserved.</p>
  </footer>

  <script>
    let cartCount = 0;

    function addToCart() {
      cartCount++;
      document.getElementById('cart-count').textContent = cartCount;
    }
  </script>
</body>
</html>
