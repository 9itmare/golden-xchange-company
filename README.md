<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Golden Exchange  company</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #c921c9;
        }
        header {
            background-color: #eee7e7f1;
            color: #460a2e;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #179b17;
            color: #960b96;
            padding: 10px;
            text-align: center;
        }
        nav a {
            text-decoration: none;
            color: #660404;
            margin: 0 10px;
        }
        section {
            padding: 20px;
        }
        footer {
            background-color: #030303;
            color: #fff;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome To Golden Exchange Company</h1>
        <img src="bitcoin image.jpeg.html.jfif" alt="Header Image">
    </header>
    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>
    <section>
        <h2>About</h2>
        <p>
            Golden Exchange Company is a global investment company that allows 
            our customers to buy, sell  and earn profits in Bitcoins,USDT or in 
            USD from the comfort of their homes or anywhere in the world we have 
            been in existence from 2012 till date and have about five million 
            customers world wide.
        </p>
    </section>
    <footer>
        <p>&copy; 2024 Golden Exchange Company. All rights reserved.</p>
        <p>Contact us at: goldenxcom@gmail.com</p>
    </footer>

    <section id="registration-form">
        <h2>Register Here</h2>
        <form id="registerForm">
            <input type="text" id="fullName" placeholder="Full Name"><br>
            <input type="email" id="email" placeholder="Email Address"><br>
            <input type="password" id="password" placeholder="password"><br>
            <input type="nationality" placeholder="nationality"><br>
            <input type="phone number" placeholder="phone number"><br>
            <input type="date of birth" placeholder="date of birth"><br>
            <input type="radio" name="gender"> male <br>
            <input type="radio" name="gender"> female<br>
            <input type="submit" value="Register">
        </form>
    </section>
        <script>
            document.getElementById('registerForm').addEventListener('submit', function(event) {
                event.preventDefault(); // Prevent form submission

                // Get user input
                var fullName = document.getElementById('fullName').value;
                var email = document.getElementById('email').value;
                var password = document.getElementByid('password').value;

                // Example: Send data to server (replace with your own implementation)
                console.log("User registered: ", fullName, email, password);
                alert("Registration Successful!"); 
        </script>
<h2>User Dashboard</h2>
<style>
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background-color: #eaee06;
    }
    header {
        background-color: #ecde0e;
        color: #122486;
        padding: 20px;
        text-align: center;
    }
    section {
        padding: 20px;
        text-align: center;
    }
    .dashboard {
        background-color: #1ba70fa6;
        padding: 20px;
        border-radius: 5px;
        margin: 20px auto;
        width: 300px;
    }
    input[type="text"], input[type="email"], input[type="submit"] {
        display: block;
        margin: 10px auto;
        padding: 8px;
        width: 90%;
        border-radius: 5px;
        border: 1px solid #ccc;
    }
    p {
        margin: 10px 0;
    }
</style>


    <div>
     <h1>Welcome to Your Dashboard</h1>
        <img src="bitcoin image.jpeg.html.jfif" alt="Header Image">
    </div>
    <section>
        <div class="dashboard" id="dashboard">
            <h2>User Dashboard</h2>
            <p>Your GEC Balance: <span id="GECBalance">$1</span> USD</p>
            <button onclick="deposit()">Deposit</button>
            <button onclick="withdraw()">Withdraw</button>
        </div>
    <div class="dashboard" id="registration-form">
        <h2>Register Here</h2>
        <form id="registerForm">
            <input type="text" id="fullName" placeholder="Full Name">
            <input type="email" id="email" placeholder="Email Address">
            <input type="submit" value="Register">
        </form>
    </div>
        <div class="dashboard" id="referral-link" style="display:none;">
            <h2>Referral Link</h2>
            <p>Your referral link: <span id="referralLink"></span></p>
        </div>
    </section>

    <script>
        function deposit() {
            var amount = prompt("Enter deposit amount in USD:");
            var name = prompt("Michael Chiemeziem Ikechukwu");
            var accountnumber = prompt("2292747665"); 
            var bank = prompt("United Bank OF Africa");
            if (amount && parseFloat(amount) >= 5) {
                alert("Deposit successful!");
                // Update Bitcoin balance (for simulation)
                document.getElementById('GECBalance').innerText = parseFloat(document.getElementById('bitcoinBalance').innerText) + parseFloat(amount);
            } else {
                alert("Minimum deposit amount is $5 USD");
            }
        }

        function withdraw() {
            var name = prompt("Enter your Name:");
            var email = prompt("Enter your Email:");
            var password = prompt("Enter your Password:");
            var bank = prompt("Enter your Bank:");
            var accountDetails = prompt("Enter your Account Details:");
            var accountName = prompt("Enter your Name on Account:");
            var amount = prompt("Enter withdrawal amount in USD:");
            if (amount && parseFloat(amount) >= 50) {
                alert("Withdrawal request submitted!");
                // Here, you would typically handle the withdrawal request on the server
            } else {
                alert("Minimun withdrawal is $50 USD!");
                }
            }
            // Simulate dashboard update after registration
            document.getElementById('registration-form').style.display = 'none'; // Hide registration form
            document.getElementById('dashboard').style.display = 'block'; // Show dashboard
            // Generate referral link
            var referralLink = "http://yourwebsite.com/referral?code=" + email;
            document.getElementById('referralLink').innerText = referralLink;
            document.getElementById('referral-link').style.display = 'block'; // Show referral link section
        });
    </script>
</body>
</html>
