# Ex.07 Restaurant Website
# Date:03.10.2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
<html>
<head>
    <title>Administration - HUNGERHUB</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: lightgray;
        }
        nav {
            background-color: darkslategray;
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            text-decoration: none;
            color: white;
            margin: 0 15px;
        }
        header {
            text-align: center;
            background-color: lightsteelblue;
            padding: 20px;
        }
        .admin-section {
            padding: 30px;
            max-width: 800px;
            margin: auto;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .admin-section h2 {
            text-align: center;
            color: rgb(117, 61, 139);
            margin-bottom: 20px;
        }
        .admin-team {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        .team-member {
            background-color: lightblue;
            border-radius: 10px;
            padding: 15px;
            text-align: center;
            width: 200px;
        }
        .team-member img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }
        .admin-login {
            margin-top: 30px;
            text-align: center;
        }
        .admin-login input {
            padding: 10px;
            margin: 10px 5px;
            border: 1px solid gray;
            border-radius: 5px;
            font-size: 14px;
        }
        .admin-login button {
            padding: 10px 20px;
            background-color: darkslateblue;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .admin-login button:hover {
            background-color: slateblue;
        }
    </style>
</head>
<body>

<nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="adminstration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<header>
    <h1>HUNGERHUB Administration</h1>
</header>

<div class="admin-section">
    <h2>Team Members</h2>
    <div class="admin-team">
        <div class="team-member">
            <img src="manager.png">
            <h3>Abijith</h3>
            <p>Manager</p>
        </div>
        <div class="team-member">
            <img src="asmanager.png">
            <h3>Kishore</h3>
            <p>Assistant Manager</p>
        </div>
        <div class="team-member">
            <img src="head.png">
            <h3>Sanjay</h3>
            <p>HR Head</p>
        </div>
    </div>

    <div class="admin-login">
        <h2>Admin Login</h2>
        <form>
            <input type="text" placeholder="Username" required>
            <input type="password" placeholder="Password" required>
            <button type="submit">Login</button>
        </form>
    </div>
</div>

</body>
</html>

<html>
<head>
    <title>Book a Table - HUNGERHUB</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: lightgray;
        }
        nav {
            background-color: darkslategray;
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            text-decoration: none;
            color: white;
            margin: 0 15px;
        }
        header {
            text-align: center;
            background-color: lightsteelblue;
            padding: 20px;
        }
        .booking-section {
            padding: 30px;
            max-width: 600px;
            margin: auto;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        .booking-section h2 {
            text-align: center;
            color: darkslateblue;
            margin-bottom: 20px;
        }
        .booking-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .booking-form input, .booking-form select, .booking-form button {
            padding: 10px;
            font-size: 16px;
            border: 1px solid gray;
            border-radius: 5px;
        }
        .booking-form button {
            background-color: darkslateblue;
            color: white;
            cursor: pointer;
        }
        .booking-form button:hover {
            background-color: slateblue;
        }
    </style>
</head>
<body>

<nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="adminstration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<header>
    <h1>Book a Table</h1>
</header>

<div class="booking-section">
    <h2>Reserve Your Table Now</h2>
    <form class="booking-form">
        <input type="text" name="name" placeholder="Your Full Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <input type="tel" name="phone" placeholder="Your Phone Number" required>
        <select name="guests" required>
            <option value="" disabled selected>Number of Guests</option>
            <option value="1">1 Guest</option>
            <option value="2">2 Guests</option>
            <option value="3">3 Guests</option>
            <option value="4">4 Guests</option>
            <option value="5">5 Guests</option>
            <option value="6+">6+ Guests</option>
        </select>
        <input type="date" name="date" required>
        <input type="time" name="time" required>
        <button type="submit">Book Now</button>
    </form>
</div>

</body>
</html>

<html>
<head>
    <title>Contact Us - HUNGERHUB</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: white;
        }
        nav {
            background-color: rgb(151, 183, 220);
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            text-decoration: none;
            color: white;
            margin: 0 15px;
        }
        header {
            text-align: center;
            background-color: rgb(251, 244, 248);
            padding: 20px;
        }
        .contact-section {
            padding: 30px;
            max-width: 600px;
            margin: auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .contact-section h2 {
            text-align: center;
            margin-bottom: 20px;
        }
        .contact-section form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .contact-section input, .contact-section textarea, .contact-section button {
            padding: 10px;
            font-size: 16px;
            border: 1px solid whitesmoke;
            border-radius: 5px;
        }
        .contact-section textarea {
            resize: none;
            height: 100px;
        }
        .contact-section button {
            background-color: #4a4a4a;
            color: white;
            cursor: pointer;
        }
    </style>
</head>
<body>

<nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="adminstration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<header>
    <h1>Contact Us</h1>
</header>

<div class="contact-section">
    <h2>We're here help you,every step of the Way</h2>
    <form>
        <input type="text" name="name" placeholder="Your Full Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <input type="tel" name="phone" placeholder="Your Phone Number (optional)">
        <textarea name="message" placeholder="Your Message..." required></textarea>
        <button type="submit">Send Message</button>
    </form>
</div>

</body>
</html>

<html>
<head>=
    <title>HUNGERHUB</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: white;
        }
        header {
            background-color: wheat;
            text-align: center;
            padding: 20px;
        }
        header img {
            width: 50px;
        }
        nav {
            background-color: grey;
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            text-decoration: none;
            color: white;
            margin: 0 15px;
        }
        .banner {
            text-align: right;
            background-image: url('banner.png');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 50px;
        }
        .banner h2 {
            margin: 0;
        }
        .banner p {
            margin-top: 10px;
        }
        .sections {
            display: flex;
            justify-content: space-around;
            padding: 20px;
            gap: 10px;
        }
        .section {
            background-color: wheat;
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            width: 30%;
        }
        .section img {
            width: 100%;
            border-radius: 10px;
        }
        footer {
            text-align: center;
            background-color: white;
            padding: 10px;
            margin-top: 20px;
        }
        footer a {
            text-decoration: none;
            color: blanchedalmond;
        }
    </style>
</head>
<body>

<header>
    <img src="hungerhub.png.png" alt="HUNGERHUB Logo"> 
    <h1>HUNGERHUB</h1>
</header>

<nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="adminstration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<div class="banner">
    <h2>30% Off This Weekend</h2>
    <p>Don't miss out on our special offer! Visit us this weekend and enjoy delicious meals at discounted prices.</p>
</div>

<div class="sections">
    <div class="section">
        <img src="menu.png.png" alt="Menu"> 
        <h3>Our New Menu</h3>
        <p>Explore a variety of mouthwatering dishes crafted to satisfy every taste. From savory appetizers to hearty main courses, there's something for everyone.</p>
        <a href="menu.html">See our new menu</a>
    </div>
    <div class="section">
        <img src="table.png.png" alt="Book a Table"> 
        <h3>Reserve Your Spot</h3>
        <p>Enjoy an unforgettable dining experience at HUNGERHUB. Book your table today and treat yourself to a fantastic meal in a cozy ambiance.</p>
        <a href="booktable.html">Book your table now</a>
    </div>
    <div class="section">
        <img src="" alt="Opening Hours"> 
        <h3>Opening Hours</h3>
        <p>
            Mon - Fri: 10Am - 11Pm<br>
            Sat: 1Pm - 10Pm<br>
            Sun: 1Pm - 10Pm
        </p>
    </div>
</div>

<footer>
    <p>Designed and Developed by Pruthvisri<br> 2501368323</p>
</footer>

</body>
</html>

<html>
<head>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: lightgray;
        }
        nav {
            background-color: darkslategray;
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav a {
            text-decoration: none;
            color: white;
            margin: 0 15px;
        }
        header {
            text-align: center;
            background-color: lightsteelblue;
            padding: 20px;
        }
        .menu-section {
            padding: 30px;
            max-width: 1000px;
            margin: auto;
        }
        .menu-title {
            text-align: center;
            color: darkslateblue;
            margin-bottom: 20px;
        }
        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        .menu-item {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            text-align: center;
            padding: 15px;
            width: 250px;
        }
        .menu-item img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }
        .menu-item h3 {
            color: darkslateblue;
            margin: 10px 0;
        }
        .menu-item p {
            color: rgb(154, 142, 142);
            font-size: 14px;
        }
        .menu-item span {
            display: block;
            font-size: 18px;
            font-weight: bold;
            color: darkslategray;
            margin-top: 10px;
        }
    </style>
</head>
<body>

<nav>
    <a href="index.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="adminstration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<header>
    <h1>Our Menu</h1>
</header>

<div class="menu-section">
    <h2 class="menu-title">Super Delicious Dishes</h2>
    <div class="menu-items">
        <div class="menu-item">
            <img src="burgar.png.png" alt="Dish 1">
            <h3>Classic burger</h3>
            <p>A juicy chicken patty with fresh lettuce, tomatoes, and cheese in a sesame seed bun.</p>
            <span>Rs. 120</span>
        </div>
        <div class="menu-item">
            <img src="pizza.png.png" alt="Dish 2">
            <h3>Margherita Pizza</h3>
            <p>Freshly baked pizza topped with mozzarella, tomatoes, and basil.</p>
            <span>Rs. 220</span>
        </div>
        <div class="menu-item">
            <img src="grill.png.png" alt="Dish 3">
            <h3>Grill</h3>
            <p> Chicken pieces, an acidic base like lemon juice or vinegar, oil, and a blend of spices and herbs such as garlic, salt, pepper, oregano, and paprika.</p>
            <span>Rs. 440</span>
        </div>
        <div class="menu-item">
            <img src="shawarma.png.png" alt="Dish 4">
            <h3>Shawarma</h3>
            <p>Marinated meat, various spices for the marinade, and accompaniments such as tahini sauce, yogurt sauce, pita bread, and fresh vegetables like tomatoes, cucumbers, and onions.</p>
            <span>Rs. 100</span>
        </div>
        <div class="menu-item">
            <img src="tikka.png.png" alt="Dish 5">
            <h3>Chiken Tikka</h3>
            <p>Boneless chicken marinated in a blend of yogurt and spices like ginger-garlic paste, cumin, coriander, turmeric, chili powder, and garam masala.</p>
            <span>Rs. 300</span>
        </div>
        <div class="menu-item">
            <img src="dosa.png.png" alt="Dish 6">
            <h3>Dosa</h3>
            <p>Soaked and fermented rice, urad dal, and fenugreek seeds, along with water and salt for fermentation and taste.</p>
            <span>Rs. 50</span>
        </div>
        <div class="menu-item">
            <img src="naan.png.png" alt="Dish 7">
            <h3>Naan</h3>
            <p>Yogurt, ghee or butter for richness, and sometimes milk or egg. A leavening agent, like yeast or baking powder, creates air pockets for a soft, fluffy texture.</p>
            <span>Rs. 90</span>
        </div>
        <div class="menu-item">
            <img src="fish.png.png" alt="Dish 8">
            <h3>Fish fry</h3>
            <p> Fish a blend of spices such as salt, turmeric, chili powder, and ginger-garlic paste, a coating made from flour, and oil for frying.</p>
            <span>Rs. 140</span>
        </div>
        <div class="menu-item">
            <img src="soup.png.png" alt="Dish 9">
            <h3>Chicken and sweetcorn soup</h3>
            <p>Chicken, sweetcorn, chicken stock, a thickener like cornstarch or flour, aromatics, eggs for a traditional creamy texture, seasonings, and sometimes fresh cream.</p>
            <span>Rs. 100</span>
        </div>
        <div class="menu-item">
            <img src="puttu.png.png" alt="Dish 10">
            <h3>Puttu</h3>
            <p>Coarsely ground rice flour, grated coconut, and salt, mixed with a small amount of water to achieve a crumbly consistency.</p>
            <span>Rs. 60</span>
        </div>
        <div class="menu-item">
            <img src="mojito.png.png" alt="Dish 11">
            <h3>Mojito</h3>
            <p>White rum, fresh mint leaves, fresh lime juice, simple syrup, ice, and club soda. </p>
            <span>Rs. 130</span>
        </div>
        <div class="menu-item">
            <img src="prawm.png.png" alt="Dish 12">
            <h3>Prawn Biryani</h3>
            <p>Basmati rice, prawns, ghee, oil, onions, tomatoes, and a blend of whole spices like cinnamon, cloves, and cardamom.</p>
            <span>Rs. 250</span>
        </div>
    </div>
</div>

</body>
</html>

```

# OUTPUT:
![alt text](<Screenshot (76).png>)
![alt text](<Screenshot (77).png>)
![alt text](<Screenshot (78)-1.png>)
![alt text](<Screenshot (79).png>)
![alt text](<Screenshot (80).png>)
![alt text](<Screenshot (81).png>)
![alt text](<Screenshot (82).png>)
# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
