# Ex.07 Restaurant Website
## Date:14-12-2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CASSENDRA - Home</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #444;
            box-sizing: border-box;
            background-color: #f0f8f5;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(90deg, #2a9d8f, #264653);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        header img {
            height: 50px;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 600;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1rem;
        }

        header nav a:hover {
            color: #e9c46a;
        }

        .banner {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 50px 20px;
            background: url('banner-placeholder.jpg') no-repeat center center/cover;
            color: #ffffff;
            height: 350px;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.7);
            position: relative;
            overflow: hidden;
        }

        .banner:after {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
        }

        .banner-content {
            max-width: 60%;
            z-index: 1;
            position: relative;
        }

        .banner-content h1 {
            font-size: 3rem;
            margin-bottom: 15px;
            font-family: 'Playfair Display', serif;
            color: #e9c46a;
        }

        .banner-content p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .banner-content a {
            background: #e76f51;
            color: white;
            padding: 12px 20px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .banner-content a:hover {
            background: #d65a3d;
        }

        .features {
            display: flex;
            justify-content: space-between;
            padding: 30px 10%;
            gap: 20px;
            background: #ffffff;
        }

        .feature {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            flex: 1;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .feature img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .feature h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: #264653;
        }

        .feature p {
            font-size: 1rem;
            color: #555;
        }

        footer {
            background: #264653;
            color: white;
            text-align: center;
            padding: 15px 0;
            margin-top: 20px;
        }

        footer a {
            color: #e9c46a;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4a261;
        }

        @media (max-width: 768px) {
            .banner {
                flex-direction: column;
                text-align: center;
                height: auto;
            }

            .banner-content {
                max-width: 100%;
            }

            .features {
                flex-direction: column;
                gap: 20px;
                padding: 20px;
            }

            header nav a {
                margin: 0 10px;
                font-size: 0.9rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="banner">
        <div class="banner-content">
            <h1>Welcome to CASSENDRA</h1>
            <p>Experience the finest flavors and a cozy ambiance at Olive Garden. We serve happiness on a plate!</p>
            <a href="#features">Explore Now</a>
        </div>
    </div>

    <section id="features" class="features">
        <div class="feature">
            <img src="veg.jpg" alt="Fresh Ingredients">
            <h3>Fresh Ingredients</h3>
            <p>We source only the freshest and most organic ingredients to create our dishes.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 CASSENDRA. All rights reserved. | <a href="#">Privacy Policy</a></p>
    </footer>
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CASSENDRA - Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background: #f8f9fa;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(90deg, #264653, #2a9d8f);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
        }

        header h1 {
            font-size: 1.8rem;
            font-weight: 700;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 600;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1rem;
        }

        header nav a:hover {
            color: #e9c46a;
        }

        .menu-container {
            padding: 40px 10%;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 2.5rem;
            color: #2a9d8f;
            margin-bottom: 20px;
            font-family: 'Playfair Display', serif;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .menu-item {
            background: #ffffff;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .menu-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 3px solid #2a9d8f;
        }

        .menu-details {
            padding: 15px;
            text-align: left;
        }

        .menu-details h3 {
            font-size: 1.5rem;
            color: #264653;
            margin-bottom: 10px;
        }

        .menu-details p {
            font-size: 0.95rem;
            color: #555;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-size: 1.2rem;
            font-weight: bold;
            color: #e76f51;
        }

        footer {
            background: #264653;
            color: white;
            text-align: center;
            padding: 15px 0;
            margin-top: 40px;
        }

        footer a {
            color: #e9c46a;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4a261;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                margin: 0 10px;
                font-size: 0.9rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <h1>CASSENDRA</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="menu-container">
        <h1>Our Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="cake.jpg" alt="Spaghetti">
                <div class="menu-details">
                    <h3>Black Forest Cake</h3>
                    <p class="price">₹120/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="juice.jpg" alt="Pizza">
                <div class="menu-details">
                    <h3>Juice</h3>
                    <p class="price">₹100/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="samoosa.jpg" alt="Lasagna">
                <div class="menu-details">
                    <h3>Samoosa</h3>
                    <p class="price">₹80/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="noodles.jpg" alt="Salad">
                <div class="menu-details">
                    <h3>Noodles</h3>
                    <p class="price">₹150/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="coffee.jpg" alt="Risotto">
                <div class="menu-details">
                    <h3>Coffee</h3>
                    <p class="price">₹50/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="sandwich.jpg" alt="Tiramisu">
                <div class="menu-details">
                    <h3>Sandwich</h3>
                    <p class="price">₹200/-</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 CASSENDRA. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CASSENDRA - Contact Us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background: #f4f4f9;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(90deg, #264653, #2a9d8f);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
        }

        header img {
            height: 50px;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 600;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1rem;
        }

        header nav a:hover {
            color: #e9c46a;
        }

        .contact-banner {
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(to bottom, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('contact.jpeg') no-repeat center center/cover;
            color: white;
            height: 300px;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.8);
        }

        .contact-banner h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            color: #f4f4f9;
        }

        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 40px 20px;
            gap: 30px;
            background: #f4f4f9;
        }

        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: white;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .contact-details:hover, .contact-form:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .contact-details h2, .contact-form h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #264653;
            text-align: center;
        }

        .contact-details p {
            margin: 15px 0;
            font-size: 1rem;
            color: #555;
        }

        .contact-details img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .contact-form label {
            font-size: 1rem;
            color: #555;
            margin-bottom: 5px;
            display: block;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
            transition: border 0.3s ease;
        }

        .contact-form input:focus, .contact-form textarea:focus {
            border-color: #2a9d8f;
            outline: none;
        }

        .contact-form textarea {
            height: 120px;
            resize: none;
        }

        .contact-form button {
            width: 100%;
            padding: 12px;
            background: #e76f51;
            color: white;
            font-size: 1.2rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .contact-form button:hover {
            background: #d1495b;
        }

        footer {
            background: #264653;
            color: white;
            text-align: center;
            padding: 15px 0;
            margin-top: 40px;
        }

        footer a {
            color: #e9c46a;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4a261;
        }

        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }

            .contact-banner h1 {
                font-size: 2rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="contact-banner">
        <h1>Contact Us</h1>
    </div>

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            <p><strong>Address:</strong> CASSENDRA, Chennai, Tamil Nadu, India</p>
            <p><strong>Phone:</strong> +91 9344210898</p>
            <p><strong>Email:</strong> cassendra@gmail.com</p>
            <p><strong>Hours:</strong> Mon-Sun: 10 AM - 10 PM</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 OLIVE CASSENDRA. All rights reserved. | <a href="#">Privacy Policy</a></p>
    </footer>

</body>
</html>

admin.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CASSENDRA - Administration</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            color: #333;
            background: #f4f4f9;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(90deg, #264653, #2a9d8f);
            color: white;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
        }

        header h1 {
            font-size: 1.8rem;
            font-weight: bold;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 600;
            margin: 0 15px;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #e9c46a;
        }

        .admin-container {
            padding: 40px 20px;
            background: #f4f4f9;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 2.5rem;
            color: #2a9d8f;
            margin-bottom: 30px;
            font-family: 'Playfair Display', serif;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 25px;
            justify-content: center;
        }

        .admin-item {
            background: white;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .admin-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .admin-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .admin-details {
            padding: 20px;
            text-align: center;
        }

        .admin-details h3 {
            font-size: 1.5rem;
            color: #264653;
            margin-bottom: 10px;
        }

        .admin-details p {
            font-size: 1rem;
            color: #555;
            line-height: 1.5;
        }

        footer {
            background: #264653;
            color: white;
            text-align: center;
            padding: 15px 0;
            margin-top: 30px;
        }

        footer a {
            color: #e9c46a;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4a261;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
</head>
<body>

    <header>
        <h1>CASSENDRA</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="admin-container">
        <h1>Our Leadership Team</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="me.jpg" alt="CEO">
                <div class="admin-details">
                    <h3>Hemanath</h3>
                    <p>CEO</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="msd.png" alt="Manager">
                <div class="admin-details">
                    <h3>Dhoni</h3>
                    <p>Manager</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="chef.jpg" alt="Master Chef">
                <div class="admin-details">
                    <h3>Venkatesh Bhat</h3>
                    <p>Master Chef</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="rona.jpg" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Ronaldo</h3>
                    <p>Assistant Managing Director</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 CASSENDRA. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>
</html>
```


## OUTPUT:
![alt text](<Screenshot (27).png>)
![alt text](<Screenshot (28).png>)
![alt text](<Screenshot (29).png>)
![alt text](<Screenshot (30).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
