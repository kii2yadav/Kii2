<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Kii2_Yadav World</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: 'Poppins', sans-serif;
}

body{
    overflow:hidden;
    background:#000;
    color:white;
}

/* Animated Background */

.background{
    position:fixed;
    width:100%;
    height:100%;
    overflow:hidden;
    z-index:-1;
    background:linear-gradient(135deg,#000000,#0f172a,#1e293b);
}

.circle{
    position:absolute;
    border-radius:50%;
    background:rgba(255,255,255,0.08);
    animation:float 10s infinite linear;
}

.circle:nth-child(1){
    width:250px;
    height:250px;
    top:10%;
    left:10%;
}

.circle:nth-child(2){
    width:180px;
    height:180px;
    top:60%;
    left:70%;
    animation-duration:14s;
}

.circle:nth-child(3){
    width:120px;
    height:120px;
    top:30%;
    left:80%;
    animation-duration:8s;
}

@keyframes float{
    0%{
        transform:translateY(0px) rotate(0deg);
    }
    50%{
        transform:translateY(-40px) rotate(180deg);
    }
    100%{
        transform:translateY(0px) rotate(360deg);
    }
}

/* Main Content */

.container{
    width:100%;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    flex-direction:column;
    text-align:center;
    padding:20px;
}

h1{
    font-size:60px;
    margin-bottom:20px;
    text-shadow:0 0 20px #00ffff;
    animation:glow 2s infinite alternate;
}

@keyframes glow{
    from{
        text-shadow:0 0 10px #00ffff;
    }
    to{
        text-shadow:0 0 30px #00ffff,
                     0 0 50px #00ffff;
    }
}

p{
    font-size:24px;
    margin-bottom:30px;
}

.search-box{
    position:relative;
    width:400px;
    max-width:90%;
}

.search-box input{
    width:100%;
    padding:15px;
    border:none;
    border-radius:40px;
    outline:none;
    font-size:18px;
    background:rgba(255,255,255,0.1);
    color:white;
    backdrop-filter:blur(10px);
    border:2px solid rgba(255,255,255,0.2);
}

.search-box input::placeholder{
    color:#ddd;
}

.search-box button{
    margin-top:20px;
    padding:12px 30px;
    border:none;
    border-radius:30px;
    background:#00ffff;
    color:#000;
    font-size:18px;
    cursor:pointer;
    transition:0.3s;
    font-weight:bold;
}

.search-box button:hover{
    background:white;
    transform:scale(1.05);
}

.note{
    margin-top:20px;
    color:#ccc;
}

.footer{
    position:absolute;
    bottom:20px;
    font-size:14px;
    color:#bbb;
}

/* Responsive */

@media(max-width:768px){
    h1{
        font-size:40px;
    }

    p{
        font-size:18px;
    }
}
</style>
</head>

<body>

<div class="background">
    <div class="circle"></div>
    <div class="circle"></div>
    <div class="circle"></div>
</div>

<div class="container">

    <h1>Hi I'm kii2_yadav</h1>
    <p>Welcome To My World</p>

    <div class="search-box">
        <input type="text" id="searchInput" placeholder="Search 1, 2, or 3">
        <button onclick="openPage()">Search</button>
    </div>

    <div class="note">
        Type:<br>
        1 = Official Profile<br>
        2 = About Us<br>
        3 = Contact Us
    </div>

</div>

<div class="footer">
    Thanks For Visiting
</div>

<script>

function openPage(){

    const value = document.getElementById("searchInput").value;

    if(value == "1"){

        let newWindow = window.open("");

        newWindow.document.write(`

        <html>
        <head>
        <title>Official Account</title>

        <style>

        body{
            margin:0;
            background:black;
            overflow:hidden;
            font-family:Arial;
            color:white;
            display:flex;
            justify-content:center;
            align-items:center;
            height:100vh;
        }

        .lion{
            position:absolute;
            width:300px;
            height:300px;
            background:radial-gradient(circle,#ff6600,#000);
            border-radius:50%;
            animation:roar 3s infinite;
            filter:blur(10px);
        }

        @keyframes roar{
            0%{transform:scale(1);}
            50%{transform:scale(1.2);}
            100%{transform:scale(1);}
        }

        .content{
            position:relative;
            text-align:center;
            z-index:2;
        }

        h1{
            font-size:50px;
            color:#ff6600;
        }

        p{
            font-size:22px;
        }

        </style>
        </head>

        <body>

        <div class="lion"></div>

        <div class="content">
            <h1>Kii2_Yadav</h1>
            <p>Official Account</p>
            <p>Model</p>
            <p>Live Like An Angry Lion</p>
            <p>Wish Me On 16 Oct</p>
            <p>Live In HYD</p>
        </div>

        </body>
        </html>

        `);

    }

    else if(value == "2"){

        let newWindow = window.open("");

        newWindow.document.write(`

        <html>
        <head>
        <title>About Us</title>

        <style>

        body{
            margin:0;
            font-family:Arial;
            color:white;
            overflow:hidden;
            background:linear-gradient(45deg,#111,#1e3a8a,#000);
            background-size:400% 400%;
            animation:bg 10s infinite alternate;
            display:flex;
            justify-content:center;
            align-items:center;
            height:100vh;
            text-align:center;
            padding:20px;
        }

        @keyframes bg{
            0%{background-position:left;}
            100%{background-position:right;}
        }

        .box{
            max-width:800px;
            background:rgba(255,255,255,0.08);
            padding:40px;
            border-radius:20px;
            backdrop-filter:blur(10px);
        }

        h1{
            font-size:50px;
            margin-bottom:20px;
            color:#00ffff;
        }

        p{
            font-size:22px;
            line-height:1.8;
        }

        </style>
        </head>

        <body>

        <div class="box">

            <h1>About Us</h1>

            <p>
            Treating everyone you meet with equal dignity,
            regardless of their background.
            </p>

            <p>
            The willingness to admit when you are wrong,
            apologize, and learn from your mistakes without making excuses.
            </p>

            <p>
            Doing what you say you will do and standing by your moral values,
            even when it's difficult.
            </p>

        </div>

        </body>
        </html>

        `);

    }

    else if(value == "3"){

        let newWindow = window.open("");

        newWindow.document.write(`

        <html>
        <head>
        <title>Contact Us</title>

        <style>

        body{
            margin:0;
            background:black;
            color:white;
            overflow:hidden;
            font-family:Arial;
            display:flex;
            justify-content:center;
            align-items:center;
            height:100vh;
        }

        .stars{
            position:absolute;
            width:100%;
            height:100%;
            background:url('https://i.imgur.com/YKY28eT.png');
            animation:move 30s linear infinite;
        }

        @keyframes move{
            from{
                background-position:0 0;
            }
            to{
                background-position:1000px 1000px;
            }
        }

        .contact{
            position:relative;
            z-index:2;
            background:rgba(255,255,255,0.08);
            padding:40px;
            border-radius:20px;
            text-align:center;
            backdrop-filter:blur(10px);
        }

        h1{
            color:#00ffff;
            margin-bottom:20px;
            font-size:50px;
        }

        p{
            font-size:22px;
            margin:15px 0;
        }

        .thanks{
            margin-top:25px;
            color:#00ffff;
            font-size:28px;
        }

        </style>
        </head>

        <body>

        <div class="stars"></div>

        <div class="contact">

            <h1>Contact Us</h1>

            <p>Instagram : kii2_yadav</p>
            <p>WhatsApp : 9542724618</p>
            <p>Snap : krish2898ad</p>
            <p>Email : kurrakittu704@gmail.com</p>

            <div class="thanks">
                Thanks For Visiting
            </div>

        </div>

        </body>
        </html>

        `);

    }

    else{
        alert("Please Enter 1, 2, or 3");
    }
}

</script>

</body>
</html>
