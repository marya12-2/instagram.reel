<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram Login</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #fafafa;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background-color: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            width: 300px;
            text-align: center;
        }
        .logo {
            font-size: 30px;
            font-weight: bold;
            color: #3897f0;
            margin-bottom: 30px;
        }
        input[type="text"], input[type="password"] {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input[type="submit"] {
            width: 100%;
            padding: 10px;
            background-color: #3897f0;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #2980b9;
        }
        .footer {
            font-size: 12px;
            margin-top: 20px;
        }
        .footer a {
            color: #8e8e8e;
            text-decoration: none;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="logo">Instagram</div>
        <form id="loginForm">
            <input type="text" id="username" placeholder="Username or email" required><br>
            <input type="password" id="password" placeholder="Password" required><br>
            <input type="submit" value="Log In">
        </form>
        <div class="footer">
            <a href="#">Forgot password?</a>
        </div>
    </div>

    <script>
        // Handle the form submission
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Prevent the default form submission

            // Get the username and password values
            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;

            // Log the username (you can add password in a more secure method)
            console.log(`Username: ${username}`);

            // Simulate sending an email (for demo purposes, we can't actually send emails without a server)
            alert('Login attempt captured. (This is a simulation, no email sent!)');

            // Simulate login logic (for demonstration)
            if (username === "admin" && password === "password") {
                alert(`Welcome, ${username}!`);
            } else {
                alert("Invalid username or password.");
            }
        });
    </script>

</body>
</html>
