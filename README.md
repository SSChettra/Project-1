<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Login Page" />
    <title>Login Page with a Twist</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f4f8;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .login-container {
            background-color: #fff;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 400px;
            width: 100%;
            text-align: center;
        }

        h1 {
            color: #333;
        }

        .form-control {
            margin-bottom: 20px;
            text-align: left;
        }

        .form-control label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #333;
        }

        .form-control input {
            width: 100%;
            padding: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        .form-control input:focus {
            outline: none;
            border-color: #007bff;
        }

        .login-button {
            background-color: #007bff;
            color: white;
            padding: 10px;
            width: 100%;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }

        .login-button:hover {
            background-color: #0056b3;
        }

        .forgot-password {
            margin-top: 10px;
            color: #007bff;
            cursor: pointer;
            display: block;
        }

        .forgot-password:hover {
            text-decoration: underline;
        }

        .signup {
            margin-top: 20px;
            color: #666;
        }

        .signup a {
            color: #007bff;
            text-decoration: none;
        }

        .signup a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <div class="login-container">
        <h1>Login</h1>
        <form id="loginForm">
            <div class="form-control">
                <label for="username">Username:</label>
                <input type="text" id="username" name="username" placeholder="Enter your username" required />
            </div>

            <div class="form-control">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" placeholder="Enter your password" required />
            </div>

            <button type="submit" class="login-button">Login</button>
        </form>

        <span class="forgot-password" onclick="showAlert()">Forgot password?</span>

        <div class="signup">
            Don't have an account? <a href="#">Sign up</a>
        </div>
    </div>

    <script>
        const loginForm = document.getElementById('loginForm');
        loginForm.addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Logging in...');
        });

        function showAlert() {
            alert('Password recovery process...');
        }
    </script>

</body>
</html>
