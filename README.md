<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Retro Football Shirts</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Relive the Glory Days with Classic Football Shirts</h1>
        <a href="shop.html" class="cta-button">Shop Now</a>
    </header>
    <section class="featured-products">
        <h2>Featured Products</h2>
        <div class="product">
            <img src="images/spain_home_1990.jpg" alt="Spain Home 1990">
            <p>Spain Home 1990</p>
            <p>€45</p>
            <a href="product.html?team=spain&year=1990&type=home" class="details-button">View Details</a>
        </div>
        <div class="product">
            <img src="images/brazil_away_1994.jpg" alt="Brazil Away 1994">
            <p>Brazil Away 1994</p>
            <p>€45</p>
            <a href="product.html?team=brazil&year=1994&type=away" class="details-button">View Details</a>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 Retro Football Shirts</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shop Retro Football Shirts</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Shop Retro Football Shirts</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="shop.html">Shop</a>
            <a href="about.html">About Us</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>
    <section class="products">
        <h2>Products</h2>
        <!-- Example product listings -->
        <div class="product">
            <img src="images/spain_home_1990.jpg" alt="Spain Home 1990">
            <p>Spain Home 1990</p>
            <p>€45</p>
            <a href="product.html?team=spain&year=1990&type=home" class="details-button">View Details</a>
        </div>
        <div class="product">
            <img src="images/italy_away_1994.jpg" alt="Italy Away 1994">
            <p>Italy Away 1994</p>
            <p>€45</p>
            <a href="product.html?team=italy&year=1994&type=away" class="details-button">View Details</a>
        </div>
        <!-- Repeat for all other jerseys -->
    </section>
    <footer>
        <p>&copy; 2024 Retro Football Shirts</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Product Details</title>
    <link rel="stylesheet" href="styles.css">
    <script src="scripts.js" defer></script>
</head>
<body>
    <header>
        <h1>Product Details</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="shop.html">Shop</a>
            <a href="about.html">About Us</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>
    <section class="product-details">
        <img id="product-image" src="" alt="Product Image">
        <div class="details">
            <h2 id="product-title">Product Title</h2>
            <p id="product-description">Product Description</p>
            <p id="product-price">Price: €45</p>
            <form id="add-to-cart-form">
                <label for="size">Size:</label>
                <select name="size" id="size">
                    <option value="s">Small</option>
                    <option value="m">Medium</option>
                    <option value="l">Large</option>
                    <option value="xl">X-Large</option>
                </select>
                <button type="button" onclick="addToCart()">Add to Cart</button>
            </form>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 Retro Football Shirts</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    margin: 0;
    font-size: 2em;
}

header nav {
    margin-top: 10px;
}

header nav a {
    color: #fff;
    margin: 0 10px;
    text-decoration: none;
}

header .cta-button {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 20px;
    background-color: #ff4c4c;
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
}

section {
    padding: 20px;
}

.featured-products, .testimonials, .categories, .products, .product-details {
    margin-bottom: 20px;
}

.featured-products h2, .testimonials h2, .categories h2, .products h2 {
    margin-bottom: 10px;
}

.product, .category {
    border: 1px solid #ccc;
    padding: 10px;
    margin: 10px;
    background-color: #fff;
    text-align: center;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

.details {
    margin-left: 20px;
}

.details-button {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 20px;
    background-color: #ff4c4c;
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
}
document.addEventListener('DOMContentLoaded', () => {
    const urlParams = new URLSearchParams(window.location.search);
    const team = urlParams.get('team');
    const year = urlParams.get('year');
    const type = urlParams.get('type');

    const productTitle = document.getElementById('product-title');
    const productDescription = document.getElementById('product-description');
    const productImage = document.getElementById('product-image');
    const productPrice = document.getElementById('product-price');

    productTitle.textContent = `${capitalizeFirstLetter(team)} ${capitalizeFirstLetter(type)} ${year}`;
    productDescription.textContent = `Authentic ${capitalizeFirstLetter(team)} ${capitalizeFirstLetter(type)} shirt from ${year}. Perfect for collectors and football fans.`;
    productImage.src = `images/${team}_${type}_${year}.jpg`;
    productImage.alt = `${capitalizeFirstLetter(team)} ${capitalizeFirstLetter(type)} ${year}`;
    productPrice.textContent = 'Price: €45';

    function capitalizeFirstLetter(string) {
        return string.charAt(0).toUpperCase() + string.slice(1);
    }
});

function addToCart() {
    const size = document.getElementById('size').value;
    const productTitle = document.getElementById('product-title').textContent;

    // Add to cart logic
    alert(`${productTitle} in size ${size} added to cart.`);
}

