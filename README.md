# Virtual-Zoo
Our Team Tech Curious with team id CB271 are here to make a website on the topic of Virtual -Zoo on the Question on CBP40.
So first we make a login page in it to describe there u have to login by set your email and  set password.
Or further there are many options for our users like home page, about page, gallery page, Animal , plants, pricing, Contact .
Also we add many photos in our website to make our website more attractiveand we try to give a experience of like a real zoo and give  user friendly experience.
Also there are pricing system in our website for individuals , school systems and Family .
there are much information we ARE GOING TO UPLOAD on the same so the one who come on our website they get something different and knowledgeable.
There is contact page in website to send messages, by which anyone wants to contact us, they can easily get into touch with with us. 
There are also a NewsLetter for users for latest news or latest updates, like the flora and funa, trees, etc

SO this how our tech curious website represent our Virtual - Zoo 


link for the flow chart
https://docs.google.com/document/d/17OKzCmtkZCxYbGkGwe6Eytoe0S4zwaG3gggqKqZFGJM/edit?usp=drivesdk







code for login page: 
Html code: 
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="script.css" class="JS">
</head>

<body>
    <div class="login_form_container">
        <div class="login_form">
            <h2>Login</h2>
            <div class="input_group">
                <i class="fa fa-user"></i>
                <input type="text" placeholder="Username" class="input_text" autocomplete="off" />
            </div>
            <div class="input_group">
                <i class="fa fa-unlock-alt"></i>
                <input type="password" placeholder="Password" class="input_text" autocomplete="off" />
            </div>
            <div class="button_group" id="login_button">
                <a>Submit</a>
            </div>
            <div class="fotter">
                <a>Forgot Password ?</a>
                <a>SingUp</a>
            </div>
        </div>
    </div>
</body>

</html>


code of CSS:
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    letter-spacing: 1px;
    background-color: #0c1022;
}

.login_form_container {
    position: relative;
    width: 400px;
    height: 470px;
    max-width: 400px;
    max-height: 470px;
    background: #040717;
    border-radius: 50px 5px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    margin-top: 70px;
}

.login_form_container::before {

    position: absolute;
    width: 170%;
    height: 170%;
    content: '';
    background-image: conic-gradient(transparent, transparent, transparent, #ee00ff);
    animation: rotate_border 6s linear infinite;

}

.login_form_container::after {

    position: absolute;
    width: 170%;
    height: 170%;
    content: '';
    background-image: conic-gradient(transparent, transparent, transparent, #00ccff);
    animation: rotate_border 6s linear infinite;
    animation-delay: -3s;
}

@keyframes rotate_border {
    0% {
        transform: rotate(0deg);
    }

    100% {
        transform: rotate(360deg);
    }
}

.login_form {
    position: absolute;
    content: '';
    background-color: #0c1022;
    border-radius: 50px 5px;
    inset: 5px;
    padding: 50px 40px;
    z-index: 10;
    color: #00ccff;

}

h2 {
    font-size: 40px;
    font-weight: 600;
    text-align: center;
}

.input_group {
    margin-top: 40px;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: start;
}

.input_text {
    width: 95%;
    height: 30px;
    background: transparent;
    border: none;
    outline: none;
    border-bottom: 1px solid #00ccff;
    font-size: 20px;
    padding-left: 10px;
    color: #00ccff;

}

::placeholder {
    font-size: 15px;
    color: #00ccff52;
    letter-spacing: 1px;

}

.fa {
    font-size: 20px;

}

#login_button {
    position: relative;
    width: 300px;
    height: 40px;
    transition: 1s;
    margin-top: 70px;


}

#login_button a {
    position: absolute;
    width: 100%;
    height: 100%;
    text-decoration: none;
    z-index: 10;
    cursor: pointer;
    font-size: 22px;
    letter-spacing: 2px;
    border: 1px solid #00ccff;
    border-radius: 50px;
    background-color: #0c1022;
    display: flex;
    justify-content: center;
    align-items: center;
}

.fotter {
    margin-top: 30px;
    display: flex;
    justify-content: space-between;

}

.fotter a {
    text-decoration: none;
    cursor: pointer;
    font-size: 18px;
}

.glowIcon {
    text-shadow: 0 0 10px #00ccff;

}




code of Javascript: 

$(".input_text").focus(function(){
    $(this).prev('.fa').addclass('glowIcon')
})
$(".input_text").focusout(function(){
    $(this).prev('.fa').removeclass('glowIcon')
})
