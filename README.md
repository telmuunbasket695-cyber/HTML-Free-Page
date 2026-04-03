# HTML-Free-Page
HTML free glowing bg page


Here's HTML code
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <section>
        <div class="login-box">
            <form action="">
                <h2>Login</h2>
                <div class="input-box">
                    <span class="icon"><ion-icon name="mail-outline"></ion-icon></span>
                    <input type="email" required>
                    <label>Email</label>
                </div>
                <div class="input-box">
                    <span class="icon"><ion-icon name="lock-closed-outline"></ion-icon></span>
                    <input type="password" required>
                    <label>Password</label>
                </div>
                <div class="remember-forgot">
                    <label><input type="checkbox">Remember me</label>
                    <a href="https://accounts.google.com/v3/signin/confirmidentifier?authuser=0&continue=https%3A%2F%2Fmyaccount.google.com%2Fsigninoptions%2Fpassword&dsh=S-1491599478%3A1775202953791937&emr=1&followup=https%3A%2F%2Fmyaccount.google.com%2Fsigninoptions%2Fpassword&mrp=security&osid=1&passive=1209600&service=accountsettings&flowName=GlifWebSignIn&flowEntry=ServiceLogin&ifkv=AT1y2_Vkj6IyJC5-70p3-v3_wKUz6WIiQs8UveR0VVmIkodtv42Zi_tl6kHMJfFP49bnkljacaTiRA">Forgot password?</a>
                </div>
                <button type="submit">Login</button>
                <div class="register-link">
                    <p>Don't have an account?<a href="https://accounts.google.com/lifecycle/steps/signup/name?dsh=S640599394:1775203702142390&flowEntry=SignUp&flowName=GlifWebSignIn&TL=AIgtPP0LNq9amJalV5WBvTaBYTKJY71rAG23AeO2h8gagsNisOEggQIme3ckb2Dm&continue=https://accounts.google.com/ManageAccount?nc%3D1">Register</a></p>
                </div>
            </form>
        </div>
    </section>

    <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
    <script nomodule src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.js"></script>
</body>

</html>


Here's CSS
section {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100vh;
    background: url(https://static.vecteezy.com/system/resources/thumbnails/035/792/899/small/ai-generated-beautiful-swirl-of-purple-smoke-on-a-black-background-photo.jpeg) no-repeat;
    background-size: cover;
    background-position: center;
    animation: animatebg 5s linear infinite;
}

@keyframes animatebg {
    100% {
        filter: hue-rotate(360deg);
    }
}

.login-box {
    position: relative;
    width: 400px;
    height: 450px;
    background-color: transparent;
    border: 2px solid rgba(255, 255, 255, .5);
    border-radius: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    backdrop-filter: blur(15px);
}


h2 {
    font-size: 2em;
    color: white;
    text-align: center;

}

.input-box {
    position: relative;
    width: 310px;
    margin: 30px 0;
    border-bottom: 2px solid white;
}

.input-box label {
    position: absolute;
    top: 50%;
    left: 5px;
    transform: translateY(-50%);
    font-size: 1em;
    color: #fff;
    pointer-events: none;
    transition: .5s;
}

.input-box input:focus~label,
.input-box input:valid~label {
    top: -5px;
}

.input-box input {
    width: 100%;
    height: 50px;
    background: transparent;
    border: none;
    outline: none;
    font-size: 1em;
    color: #fff;
    padding: 0 35px 0 px;
}

.input-box .icon {
    position: absolute;
    right: 8px;
    color: #fff;
    font-size: 1.2em;
    line-height: 57px;

}

.remember-forgot {
    margin: -15px 0 15px;
    font-size: .9em;
    color: #fff;
    display: flex;
    justify-content: space-between;
}

.remember-forgot label input {
    margin-right: 3px;
}

.remember-forgot a {
    color: #fff;
    text-decoration: none;
}

.remember-forgot a:hover {
    text-decoration: underline;
}

button {
    width: 100%;
    height: 40px;
    background: #fff;
    border: none;
    outline: none;
    border-radius: 40px;
    cursor: pointer;
    font-size: 1em;
    color: #000;
    font-weight: 500;
}

.register-link {
    font-size: .9em;
    color: #fff;
    text-align: center;
    margin: 25px 0 10px;
}

.register-link p a {
    color: #fff;
    text-decoration: none;
    font-weight: 600;
}

.register-link p a:hover {
    text-decoration: underline;
}

@media (max-width: 418px) {
    .login-box {
        width: 100%;
        height: 100vh;
        border: none;
        border-radius: 0;
    }

    .input-box {
        width: 290px;
    }
}
