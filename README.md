# Ex02 Commercial Website
## Date:29/07/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
index.html
```
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FlexShop | Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <header>
        <nav class="navbar">
            <h2 class="logo">FlexShop</h2>

            <ul class="nav-links">
                <li><a href="#">Home</a></li>
                <li><a href="#">Products</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Welcome to FlexShop</h1>
            <p>Your One-Stop Destination for Quality Products</p>
            <button>Shop Now</button>
        </div>
    </section>

    <!-- Products Section -->
    <section class="products">

        <h2>Featured Products</h2>

        <div class="product-container">

            <div class="card">
                <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=250&h=180&fit=crop" alt="Smartphone">
                <h3>Smartphone</h3>
                <p>$499</p>
                <button>Buy Now</button>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=250&h=180&fit=crop" alt="Laptop">
                <h3>Laptop</h3>
                <p>$899</p>
                <button>Buy Now</button>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=250&h=180&fit=crop" alt="Headphones">
                <h3>Headphones</h3>
                <p>$99</p>
                <button>Buy Now</button>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1546868871-7041f2a55e12?w=250&h=180&fit=crop" alt="Smart Watch">
                <h3>Smart Watch</h3>
                <p>$199</p>
                <button>Buy Now</button>
            </div>

        </div>

    </section>

    <!-- About Section -->

    <section class="about">

        <h2>About FlexShop</h2>

        <p>
            FlexShop is a modern online shopping platform built using HTML and CSS Flexbox.
            It provides customers with a clean, responsive, and user-friendly shopping
            experience across desktop, tablet, and mobile devices.
        </p>

    </section>

    <!-- Footer -->

    <footer>

        <p>&copy; 2026 FlexShop. All Rights Reserved.</p>

        <div class="student-details">

            <p><strong>Name :</strong> Thameez Ahamed A</p>

            <p><strong>Reg No :</strong> 212224220116</p>

        </div>

    </footer>

</body>
</html>
```
```
style.css
```
```
/* Reset */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

body{
    background:#f4f4f4;
}

/* Navigation */

.navbar{
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:#1f2937;
    color:white;
    padding:20px 60px;
}

.logo{
    font-size:30px;
    font-weight:bold;
}

.nav-links{
    display:flex;
    list-style:none;
    gap:30px;
}

.nav-links a{
    text-decoration:none;
    color:white;
    font-size:18px;
    transition:0.3s;
}

.nav-links a:hover{
    color:#ffd700;
}

/* Hero */

.hero{
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    height:450px;
    background:linear-gradient(135deg,#2563eb,#3b82f6);
    color:white;
}

.hero-content h1{
    font-size:50px;
    margin-bottom:20px;
}

.hero-content p{
    font-size:22px;
    margin-bottom:25px;
}

.hero button{
    padding:12px 30px;
    font-size:18px;
    border:none;
    border-radius:5px;
    background:#ffd700;
    cursor:pointer;
    transition:0.3s;
}

.hero button:hover{
    background:white;
}

/* Products */

.products{
    padding:60px;
    text-align:center;
}

.products h2{
    margin-bottom:40px;
    font-size:36px;
}

.product-container{

    display:flex;
    justify-content:center;
    gap:25px;
    flex-wrap:wrap;

}

.card{

    width:260px;
    background:white;
    border-radius:10px;
    overflow:hidden;
    box-shadow:0 5px 15px rgba(0,0,0,0.2);
    transition:0.3s;

}

.card:hover{

    transform:translateY(-8px);

}

.card img{

    width:100%;

}

.card h3{

    margin:15px;

}

.card p{

    color:#2563eb;
    font-size:20px;
    margin-bottom:15px;

}

.card button{

    margin-bottom:20px;
    padding:10px 25px;
    border:none;
    background:#2563eb;
    color:white;
    border-radius:5px;
    cursor:pointer;
    transition:0.3s;

}

.card button:hover{

    background:#1d4ed8;

}

/* About */

.about{

    background:white;
    text-align:center;
    padding:60px;

}

.about h2{

    margin-bottom:20px;
    font-size:35px;

}

.about p{

    max-width:800px;
    margin:auto;
    line-height:1.8;
    font-size:18px;

}

/* Footer */

footer{

    background:#1f2937;
    color:white;
    text-align:center;
    padding:25px;

}

footer p{

    margin:8px 0;

}

.student-details{

    margin-top:15px;
    border-top:1px solid rgba(255,255,255,0.3);
    padding-top:15px;

}

/* Responsive */

@media(max-width:768px){

.navbar{

    flex-direction:column;
    gap:20px;

}

.nav-links{

    flex-direction:column;
    align-items:center;

}

.hero{

    height:350px;

}

.hero-content h1{

    font-size:36px;

}

.hero-content p{

    font-size:18px;

}

.products{

    padding:30px;

}

.about{

    padding:40px 20px;

}

}
```

## OUTPUT
<img width="1917" height="1142" alt="image" src="https://github.com/user-attachments/assets/44bbac73-723a-4cbc-9285-a88cb2409c88" />
<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/2fd9ce5a-b30c-4e61-b8e7-10248cd44e8a" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
