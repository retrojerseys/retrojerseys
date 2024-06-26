- 👋 Hi, I’m @retrojerseys
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
retrojerseys/retrojerseys is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
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
        <!-- Example product listings -->
        <div class="product">
            <img src="images/shirt1.jpg" alt="Retro Shirt 1">
            <p>1986 Argentina Home Shirt</p>
            <p>$79.99</p>
        </div>
        <div class="product">
            <img src="images/shirt2.jpg" alt="Retro Shirt 2">
            <p>1994 Brazil Away Shirt</p>
            <p>$89.99</p>
        </div>
    </section>
    <section class="testimonials">
        <h2>What Our Customers Say</h2>
        <blockquote>"The best place to find authentic retro shirts!" - John D.</blockquote>
        <blockquote>"High-quality and fast shipping. Love my new shirt!" - Sarah P.</blockquote>
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
    <section class="categories">
        <h2>Categories</h2>
        <ul>
            <li><a href="#">1970s</a></li>
            <li><a href="#">1980s</a></li>
            <li><a href="#">1990s</a></li>
            <li><a href="#">Teams</a></li>
            <li><a href="#">Countries</a></li>
        </ul>
    </section>
    <section class="products">
        <h2>Products</h2>
        <!-- Example product listings -->
        <div class="product">
            <img src="images/shirt1.jpg" alt="Retro Shirt 1">
            <p>1986 Argentina Home Shirt</p>
            <p>$79.99</p>
            <a href="product.html" class="details-button">View Details</a>
        </div>
        <div class="product">
            <img src="images/shirt2.jpg" alt="Retro Shirt 2">
            <p>1994 Brazil Away Shirt</p>
            <p>$89.99</p>
            <a href="product.html" class="details-button">View Details</a>
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

.featured-products, .testimonials, .categories, .products {
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
