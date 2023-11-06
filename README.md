<html>
<head>
    <title>Login Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }

        .login-container {
            background-color: #fff;
            max-width: 400px;
            padding: 100px;
            border-radius: 20px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            color: #007BFF;
            text-align: center;
        }

        label {
            display: block;
            margin-top: 15px;
            font-weight: bold;
        }

        input[type="text"],
        input[type="password"] {
            width: 90%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        button {
            background-color: #007BFF;
            color: #fff;
            border: none;
            padding: 10px 20px;
            margin-top: 20px;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h1>Login</h1>
        <form id="login-form">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required><br>
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required><br>
            <button type="button" onclick="authenticateUser()">Login</button>
        </form>
    </div>

    <script>
        function authenticateUser() {
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;

            // Check if the entered username and password are correct
            if (username === "Admin" && password === "2ndApril2008") {
                // Redirect to another page when credentials are correct
                window.location.href = "https://docs.google.com/spreadsheets/u/1/d/e/2PACX-1vTQDcF7t4fzflkO5kDld5xk5qZecTpnlbfBjWHaBkQv6_9JWv2ucQ3zk2ksQ-MLQYL5oeSMv0Zslrc9/pubhtml";
            } else {
                alert("Incorrect username or password. Please try again.");
            }
        }
    </script>
</body>
</html>
