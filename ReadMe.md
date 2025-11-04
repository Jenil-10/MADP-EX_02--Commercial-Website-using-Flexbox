# Ex02 Commercial Website

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

## PROGRAM:
```
T.DANUSH REDDY
212223040029
```
# index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DR Store Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Danush store.in</h1>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#account">User Account</a></li>
      </ul>
    </nav>
  </header>
  <section id="home" class="section">
    <section id="worldmap" class="background-map">
    <div class="overlay">
    
    <h2>Welcome to Danush Store</h2>
    <p>Your trusted partner in online supplier.</p>
    <button class="btn">Learn More</button>
    </div>
  </section>
  
    </div>
  </section>
  <section id="products" class="section">
    <h2>Our Products & policies</h2>
    <p>24/7 coustomer serives and coustomer support</p>
    <div class="flex-container">
      <div class="card">
        <img src="exp-2.1.png" alt="Product 1">
        <h3>Smart Tv</h3>
        <p>$869</p>
        <p>High-quality  resolution and reliable Vr acess provided.</p>
      </div>
      <div class="card">
        <img src="tesla.jpg"alt="Product 2">
        <h3>Tesla</h3>
        <P>$54,990</P>
        <p>Designed for efficiency and performance.</p>
      </div>
      <div class="card">
        <img src="OIP.jpg" alt="Product 3">
        <h3>vr</h3>
        <p>Innovative and user-friendly.</p>
      </div>
    </div>
  </section>
  <section id="home" class="section">
    <section id="worldmap" class="background-map">
    <div class="overlay">
      <h2>Global Digital Reach</h2>
      <p>Connecting businesses around the world.</p>
    </div>
    </section>
  <section id="about" class="section">
    <h2>About Us</h2>
    <p>We are a team of passionate innovators creating impactful solutions for the digital world.</p>
  </section>
  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <p>Email: info@DRcompany.com</p>
    <p>Phone: +91 70326 86896</p>
  </section>
  <section id="account" class="section">
    <h2>User Account</h2>
    <p>Sign in to manage your profile and access services.</p>
    <button class="btn">Login</button>
  </section>
  <footer>
    <div class="social">
      <a href="#">Facebook</a> |
      <a href="#">Twitter</a> |
      <a href="#">LinkedIn</a>
    </div>
    <p>© 2025 My Company. All Rights Reserved.</p>
  </footer>
</body>
</html>
```
# style.css
```
/* Global Styles */
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background-color: #f5f5f5;
  color: #333;
}

header {
  background-color: #1a1a1a;
  color: white;
  padding: 15px 30px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

header h1 {
  font-size: 1.5rem;
}
header h2{
  font-size: 5.5rem;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
  margin: 0;
  padding: 0;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.3s;
}

nav a:hover {
  color: #03dffc;
}

/* Section Styling */
.section {
  padding: 60px 20px;
  text-align: center;
  background-color: white;
  margin: 10px 0;
}

.section h2 {
  color: #fcfefe;
}

/* Flexbox Layout for Products */
.flex-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 30px;
}

.card {
  background: #fff;
  border-radius: 12px;
  padding: 20px;
  width: 250px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  width: 100%;
  border-radius: 10px;
}

/* Digital World Map Background Section */
.background-map {
  background-image: url("photo.jpg");
  background-size: cover;
  background-position: center;
  position: relative;
  height: 1060px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.background-map .overlay {
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  padding: 60px;
  text-align: center;
  border-radius: 10px;
}

.btn {
  background-color: #0077b6;
  color: white;
  border: none;
  padding: 20px 30px;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.3s;
}

.btn:hover {
  background-color: #0096c7;
}

/* Footer */
footer {
  background-color: #1a1a1a;
  color: white;
  text-align: center;
  padding: 20px;
}

footer .social a {
  color: #00bcd4;
  margin: 0 10px;
  text-decoration: none;
}

footer .social a:hover {
  color: white;
}
```
## OUTPUT:
<img width="1919" height="975" alt="Screenshot 2025-10-09 174603" src="https://github.com/user-attachments/assets/897b9cf2-22cc-4516-8e16-2f31466f50a7" />
<img width="1915" height="620" alt="Screenshot 2025-10-10 084428" src="https://github.com/user-attachments/assets/b673bf41-7aae-417f-9351-443e1e2be9ae" />
<img width="1915" height="620" alt="Screenshot 2025-10-10 084428" src="https://github.com/user-attachments/assets/1e48dc5a-ca3b-4fcf-ae83-5a0f314d9725" />
<img width="1891" height="916" alt="Screenshot 2025-10-10 084518" src="https://github.com/user-attachments/assets/3d3658d7-cde4-4d7a-8ddd-f860a9607470" />
<img width="1891" height="755" alt="image" src="https://github.com/user-attachments/assets/e2ae4bf6-3d94-4d4f-a60c-d6281950e714" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
