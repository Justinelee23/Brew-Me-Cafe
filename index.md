brew-me-cafe
index.md
---
layout: page
title: Brew Me Café
permalink: /
---
# Welcome to Brew Me Café

We are passionate about serving high-quality coffee in a cozy atmosphere.

## Our Menu

- ## Espresso (Espresso)
- Cappuccino
- Latte

## Visit Us Today!

[Contact Us](contact.html)
# File Name: about.md

---
layout: page
title: About Us
permalink: /about/
---

# Our Story

Brew Me Café is dedicated to providing exceptional coffee experiences.
# File Name: contact.md

---
layout: page
title: Contact Us
permalink: /contact/
---

# Get in Touch!

Email us at [info@brewmecafe.com](mailto://info@brewmecafe.com) or visit our location today!
[Visit About Page]([Visit About Page]([https://www.facebook.com/justinelee72]
_config.yml


[## 🛒 Online Ordering

Order your favorite food and drinks online! Simply select your items and submit your order.

<form action="https://formspree.io/f/xjkgerqg" method="POST">
    
### ☕ Specialty Drinks

**Espresso - ₱50**  
<label for="espresso">Quantity:</label>
<select name="Espresso" id="espresso">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

**Brewed Coffee - ₱60**  
<label for="brewed-coffee">Quantity:</label>
<select name="Brewed Coffee" id="brewed-coffee">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

**Cappuccino - ₱75**  
<label for="cappuccino">Quantity:</label>
<select name="Cappuccino" id="cappuccino">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

---

### 🍽️ Snacks & Food  

**Tuna Sandwich - ₱85**  
<label for="tuna-sandwich">Quantity:</label>
<select name="Tuna Sandwich" id="tuna-sandwich">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

**Egg Sandwich - ₱75**  
<label for="egg-sandwich">Quantity:</label>
<select name="Egg Sandwich" id="egg-sandwich">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

**Burger with Fries - ₱120**  
<label for="burger-fries">Quantity:</label>
<select name="Burger with Fries" id="burger-fries">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

---

### 🍝 Pasta  

**Creamy Tuna Pesto Pasta - ₱150**  
<label for="tuna-pesto">Quantity:</label>
<select name="Creamy Tuna Pesto Pasta" id="tuna-pesto">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

**Classic Carbonara - ₱140**  
<label for="carbonara">Quantity:</label>
<select name="Classic Carbonara" id="carbonara">
    <option value="0">0</option>
    <option value="1">1</option>
    <option value="2">2</option>
    <option value="3">3</option>
</select>  

---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brew Me Café - Online Ordering</title>
    <link rel="stylesheet" href="styles.css">
    <script>
        function updateTotal() {
            let total = 0;
            const prices = {
                espresso: 50, brewed_coffee: 60, cappuccino: 75,
                tuna_sandwich: 85, egg_sandwich: 75, burger_fries: 120,
                tuna_pesto: 150, carbonara: 140
            };
            
            for (const item in prices) {
                let qty = document.getElementById(item).value;
                total += prices[item] * qty;
            }
            document.getElementById('totalPrice').innerText = 'Total: ₱' + total;
        }
    </script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f8f8f8;
        }
        .container {
            max-width: 600px;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            text-align: center;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            font-weight: bold;
        }
        select, input, textarea {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            width: 100%;
            background-color: #ff6600;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            font-size: 16px;
        }
        .total {
            font-size: 18px;
            font-weight: bold;
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>🛒 Online Ordering</h2>
        <p>Order your favorite food and drinks online! Select your items and submit your order.</p>
        <form action="https://formspree.io/f/xjkgerqg" method="POST">
            <div class="form-group">
                <label>☕ Specialty Drinks</label>
                <select id="espresso" name="Espresso" onchange="updateTotal()">
                    <option value="0">Espresso - ₱50</option>
                    <option value="1">1</option>
                    <option value="2">2</option>
                </select>
                <select id="brewed_coffee" name="Brewed Coffee" onchange="updateTotal()">
                    <option value="0">Brewed Coffee - ₱60</option>
                    <option value="1">1</option>
                    <option value="2">2</option>
                </select>
            </div>
            <div class="form-group">
                <label>🍽 Snacks & Food</label>
                <select id="tuna_sandwich" name="Tuna Sandwich" onchange="updateTotal()">
                    <option value="0">Tuna Sandwich - ₱85</option>
                    <option value="1">1</option>
                    <option value="2">2</option>
                </select>
            </div>
            <div class="form-group">
                <label>🍝 Pasta</label>
                <select id="tuna_pesto" name="Creamy Tuna Pesto Pasta" onchange="updateTotal()">
                    <option value="0">Creamy Tuna Pesto Pasta - ₱150</option>
                    <option value="1">1</option>
                    <option value="2">2</option>
                </select>
            </div>
            <div class="total" id="totalPrice">Total: ₱0</div>
            <div class="form-group">
                <label>Name</label>
                <input type="text" name="name" required>
            </div>
            <div class="form-group">
                <label>Email</label>
                <input type="email" name="email" required>
            </div>
            <div class="form-group">
                <label>Phone Number</label>
                <input type="tel" name="phone">
            </div>
            <div class="form-group">
                <label>Additional Notes</label>
                <textarea name="message"></textarea>
            </div>
            <button type="submit">Submit Order</button>
        </form>
    </div>
</body>
</html>
