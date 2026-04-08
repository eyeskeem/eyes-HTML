# 🎨 web-core-5.9
https://eyeskeem.github.io/web-core-5.9./

### HTML (Основная структура)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="/web-core-4.7/style.css">
    <title>Homework Landing Page</title>
</head>
<body>
    <main>
        <div class="two-columns"> 
            
            <div class="left-column">
                <img class="main-pic" src="/web-core-4.7/image/bg.jpg" alt="pc graphics, graphics, notebook">
                <img class="logo" src="/web-core-4.7/image/logo (2).svg" alt="logo">
            </div>

            <div class="right-column">
                <h1>Get into it today</h1>
                <p>There is no charge or obligation upon registration.</p>

                <div class="registration">
                    <button class="facebook-button">Register with Facebook</button>
                    <button class="linkedin-button">Register with Linkedin</button>
                    <p class="OR">OR</p>
                    <span class="box-left"></span>
                    <span class="box-right"></span>
                </div>

                <div class="input-pic">
                    <img class="facebook-img" src="/web-core-4.7/image/facebook (1).svg" alt="facebook">
                    <img class="linkedin-img" src="/web-core-4.7/image/linkedin (1).svg" alt="linkedin">
                </div>

                <form action="https://chat.deepseek.com/" method="get">
                    <div class="enter-form">
                        <label class="email" for="email">Email</label>
                        <input class="email-input" type="email" id="email" name="email" placeholder="gus.goodwin@gmail.com" required>
                        <label class="phone" for="phone">Phone</label>
                        <input class="phone-input" type="tel" name="phone" id="tel" required>
                    </div>   

                    <div class="Main-text">
                        <h2>What type of investor are you?</h2>
                        <p>Select the type of investor you are below</p>
                    </div>

                    <div class="radio-button">
                        <label>
                            <input type="radio" id="Individual" name="options" value="Individual" required>Individual
                            <span class="info-icon">ⓘ</span>
                        </label>
                        <label>
                            <input type="radio" id="Business" name="options" value="Business" required> Business
                            <span class="info-icon">ⓘ</span>
                        </label>
                        <label>
                            <input type="radio" id="IRA" name="options" value="IRA" required> IRA
                            <span class="info-icon">ⓘ</span>
                        </label>
                        <label>
                            <input type="radio" id="Trust" name="options" value="Trust" required>Trust
                            <span class="info-icon">ⓘ</span>
                        </label>
                    </div>

                    <div>
                        <p class="radio-info">I am a natural person investing on my own behalf as a sole owner, joint tenant, or tenant on common.</p>
                    </div>

                    <label class="checkbox">
                        <input type="checkbox" id="checkbox" name="terms-agreed" value="trust" required> 
                        I agree to the terms and receiving notifications from iintoo 
                        <a href="https://medium.com/@TermsFeed/12-ways-to-show-your-terms-to-users-156ad6c8416e">View full terms</a>
                    </label>
                    
                    <div class="form">
                        <button class="Create-Account" type="submit">Create account</button>
                    </div>
                </form>
            </div>
        </div>
</body>
</html>
```

### 🎨 CSS

```CSS

 @font-face {
    font-family: "Barlow";
    src: url('fonts/Barlow-Regular.otf') format('opentype');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: "Barlow";
    src: url('fonts/Barlow-Bold.otf') format('opentype');
    font-weight: bold;
    font-style: normal;
}

main {
    display: flex;
    background-color: #EFF6FF;
}

.two-columns {
    display: flex;
    max-width: 1600px;
    width: 100%;
    margin: 0 auto;
}


.left-column {
    position: relative;
    overflow: hidden;
    margin-bottom: 80px;
}

.right-column {
    width: 680px;
    height: 1000px;
    margin-top: 80px;
    margin-bottom: 80px;
    background-color: #ffffff;
}

.main-pic {
    margin-top: 80px;
    margin-left: 100px;
    width: 760px;
    height: 1000px;
}

.logo {
    position: absolute;
    width: 137px;
    top: 125px;
    left: 153px;
    height: auto;
}

.facebook-img {
    display: inline-block;
    position: relative;
    width: 20px;
    height: auto;
    bottom: 110px;
    margin-left: 88px;
}

.linkedin-img {
    display: inline-block;
    position: relative;
    width: 20px;
    height: auto;
    bottom: 110px;
    margin-left: 265px;
}

h1 {
    margin-top: 100px;
    margin-left: 75px;
    font-size: 30px;
    font-family: "Barlow";
    letter-spacing: -1.5;
    font-weight: normal;
    color: #7B8A92;
}

p {
    margin-left: 75px;
    font-family: "Barlow";
    font-size: 20px;
    font-style: normal;
    color: #96A5B1;
}

.facebook-button {
    width: 245px;
    height: 42px;
    margin-top: 40px;
    margin-left: 75px;
    border: none;
    border-radius: 0px;    
    cursor: pointer;
    transition: 0.3s;
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
    color: #ffffff;
    background-color: #255b9b;
}

.linkedin-button {
    width: 245px;
    height: 42px;
    margin-top: 40px;
    margin-left: 35px;
    border: none;
    border-radius: 0px;     
    cursor: pointer;
    transition: 0.3s;
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
    color: #ffffff;
    background-color: #0076b6;
}

.OR {
    margin-top: 50px;
    margin-left: 330px;
    font-family: "Barlow";
    font-size: 14px;
    color: #AFAFAF;
}

.registration {
    position: relative;
}

.box-left {
    position: absolute;
    width: 108px;
    height: 1px;
    top: 140px;
    margin-left: 210px;
    background-color: #AFAFAF;
}
.box-right {
    position: absolute;
    width: 108px;
    height: 1px;
    top: 140px;
    margin-left: 360px;
    background-color: #AFAFAF;
}

.enter-form {
    position: relative;

}

.email-input {
    position: relative;
    width: 235px;
    height: 30px;
    top: 20px;
    margin-left: 75px;
    padding-top: 25px;
    padding-left: 5px;
    border-top: 1px solid;
    border-bottom: 1px solid;
    border-right: 1px solid;
    border-color: #EEEEEE ;
    border-left: 2px solid #0076b6;
    background-color: transparent;
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
}

.email {
    position: absolute;
    margin-top: 25px;
    margin-left: 82px;
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
    color: #AFAFAF;
}

.email-input::placeholder {
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
    color: #000000;
}

.phone-input {
   position: relative;
    width: 245px;
    height: 30px;
    top: 20px;
    margin-left: 35px;
    padding-top: 25px;
    padding-left: 5px;
    border-top: 1px solid;
    border-bottom: 1px solid;
    border-left: 1px solid;
    border-right: 1px solid;
    border-color: #EEEEEE ;
    background-color: transparent;
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
}

.phone {
    position: absolute;
    margin-top: 25px;
    margin-left: 45px;
    font-family: "Barlow";
    font-size: 15px;
    font-style: normal;
    color: #AFAFAF;
}

.Main-text h2 {
    position: relative;
    margin-top: 55px;
    margin-left: 75px;
    font-family: "Barlow";
    font-size: 22px;
    font-weight: normal;
    color: #7B8A92;
}

.Main-text p {
    position: relative;
    font-family: "Barlow";
    font-size: 14px;
    font-style: normal;
    color: #96A5B1;
}

.radio-button {
    position: relative;
    margin-top: 50px;
    margin-left: 75px;
}

.radio-button label {
    cursor: pointer;
    margin-right: 30px;
    font-family: "Barlow";
    font-style: normal;
    font-size: 15px;
}

.radio-button input[type="radio"] {
    margin-right: 13px;
}

.radio-button span {
    position: relative;
    left: 3px;
    font-size: 12px;
    color: #96A5B1;
}

.radio-info {
    position: relative;
    width: 250px;
    margin-top: 40px;
    margin-left: 95px;
    border-radius: 1px;
    box-shadow: 0px 0px 5px 1px rgba(209, 209, 209, 0.2);
    font-family: "Barlow";
    font-size: 14px;
    font-style: normal;
    color: #96A5B1;
}

.checkbox {
    position: absolute;
    margin-top: 40px;
    margin-left: 75px;
    font-family: "Barlow";
    font-size: 13px;
    font-style: normal;
    color: #96A5B1;
}

.Create-Account {
    position: relative;
    width: 245px;
    height: 42px;
    margin-top: 110px;
    margin-left: 75px;
    border-radius: 5px;
    border: 1px solid #3698FB;
    background-color: #3698FB;
    font-family: "Barlow";
    font-weight: 600;
    font-size: 15px;
    color: #ffffff;
} 
```
