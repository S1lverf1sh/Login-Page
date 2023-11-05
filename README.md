<!DOCTYPE html>
<html>
<head>
    <title>Login Page</title>
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
