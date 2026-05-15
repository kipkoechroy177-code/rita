```html id="p7x4zm"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rita & Roy ❤️ Forever</title>

    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>

        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
        }

        body{
            font-family:'Poppins',sans-serif;
            background:linear-gradient(135deg,#ff4d6d,#ff8fa3,#ffb3c1);
            color:white;
            overflow-x:hidden;
        }

        html{
            scroll-behavior:smooth;
        }

        /* HERO SECTION */

        .hero{
            min-height:100vh;
            display:flex;
            justify-content:center;
            align-items:center;
            flex-direction:column;
            text-align:center;
            padding:30px;
            position:relative;
        }

        .heart{
            font-size:70px;
            animation:pulse 1.5s infinite;
        }

        @keyframes pulse{
            0%{transform:scale(1);}
            50%{transform:scale(1.2);}
            100%{transform:scale(1);}
        }

        .hero h1{
            font-size:4rem;
            margin-top:15px;
            text-shadow:0 0 15px rgba(255,255,255,0.6);
        }

        .hero p{
            max-width:800px;
            margin-top:20px;
            line-height:2;
            font-size:20px;
        }

        .hero button{
            margin-top:30px;
            padding:15px 35px;
            border:none;
            border-radius:40px;
            background:white;
            color:#ff4d6d;
            font-size:18px;
            cursor:pointer;
            font-weight:600;
            transition:0.3s;
        }

        .hero button:hover{
            transform:scale(1.08);
        }

        /* LOVE QUOTE */

        .quote{
            padding:70px 20px;
            text-align:center;
            background:rgba(255,255,255,0.1);
            backdrop-filter:blur(10px);
        }

        .quote h2{
            font-size:2.3rem;
            margin-bottom:20px;
        }

        .quote p{
            max-width:800px;
            margin:auto;
            font-size:20px;
            line-height:2;
        }

        /* GALLERY */

        .gallery-section{
            padding:80px 20px;
            text-align:center;
        }

        .gallery-section h2{
            font-size:2.8rem;
            margin-bottom:20px;
        }

        .gallery-section p{
            margin-bottom:40px;
            font-size:18px;
        }

        .gallery{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:25px;
            max-width:1200px;
            margin:auto;
        }

        .photo-card{
            position:relative;
            overflow:hidden;
            border-radius:25px;
            box-shadow:0 10px 25px rgba(0,0,0,0.3);
            transition:0.4s;
            height:350px;
            background:white;
        }

        .photo-card:hover{
            transform:translateY(-10px) scale(1.03);
        }

        .photo-card img{
            width:100%;
            height:100%;
            object-fit:cover;
            transition:0.5s;
        }

        .photo-card:hover img{
            transform:scale(1.1);
        }

        .overlay{
            position:absolute;
            bottom:0;
            width:100%;
            padding:20px;
            background:linear-gradient(to top,rgba(0,0,0,0.8),transparent);
            text-align:left;
        }

        .overlay h3{
            font-size:20px;
        }

        .overlay p{
            font-size:14px;
            margin-top:5px;
        }

        /* MEMORY SECTION */

        .memory{
            padding:80px 20px;
            text-align:center;
            background:rgba(255,255,255,0.08);
        }

        .memory h2{
            font-size:2.5rem;
            margin-bottom:25px;
        }

        .memory p{
            max-width:900px;
            margin:auto;
            line-height:2;
            font-size:19px;
        }

        /* FOOTER */

        .footer{
            padding:60px 20px;
            text-align:center;
        }

        .footer h2{
            font-size:2.5rem;
            margin-bottom:20px;
        }

        .footer p{
            max-width:800px;
            margin:auto;
            line-height:2;
            font-size:18px;
        }

        .footer span{
            display:block;
            margin-top:30px;
            font-size:30px;
            font-weight:bold;
        }

        /* FLOATING HEARTS */

        .floating-heart{
            position:fixed;
            color:white;
            animation:float 6s linear infinite;
            opacity:0.5;
            pointer-events:none;
        }

        @keyframes float{
            0%{
                transform:translateY(100vh) scale(0);
            }
            100%{
                transform:translateY(-120vh) scale(1.5);
            }
        }

        /* RESPONSIVE */

        @media(max-width:768px){

            .hero h1{
                font-size:2.5rem;
            }

            .hero p{
                font-size:17px;
            }

            .gallery-section h2,
            .memory h2,
            .footer h2,
            .quote h2{
                font-size:2rem;
            }

        }

    </style>
</head>

<body>

    <!-- FLOATING HEARTS -->
    <script>
        for(let i=0;i<25;i++){

            let heart=document.createElement("div");

            heart.className="floating-heart";

            heart.innerHTML="❤️";

            heart.style.left=Math.random()*100+"vw";

            heart.style.fontSize=(20+Math.random()*30)+"px";

            heart.style.animationDuration=(4+Math.random()*6)+"s";

            document.body.appendChild(heart);
        }
    </script>

    <!-- HERO -->

    <section class="hero">

        <div class="heart">❤️</div>

        <h1>Rita & Roy ✨</h1>

        <p>
            Some people enter your life and change everything forever 🥺💖  
            Rita, you are my peace, my happiness, my comfort, and my favorite person in the world 🌍❤️  
            Every moment with you feels magical ✨  
            Every picture with you holds a memory I never want to lose 📸💕
        </p>

        <button onclick="document.querySelector('.gallery-section').scrollIntoView()">
            View Our Memories 📸
        </button>

    </section>

    <!-- LOVE QUOTE -->

    <section class="quote">

        <h2>💌 A Love Message For Rita</h2>

        <p>
            Loving you is the softest and most beautiful feeling my heart has ever known ❤️  
            Your smile lights up my darkest days 🌸  
            Your voice calms my soul 🫂  
            And your love makes life feel worth it every single day 💖
        </p>

    </section>

    <!-- GALLERY -->

    <section class="gallery-section">

        <h2>📸 Our Beautiful Memories</h2>

        <p>
            Every photo here tells a story of love, happiness, laughter, and unforgettable moments ❤️✨
        </p>

        <div class="gallery">

            <!-- PHOTO 1 -->
            <div class="photo-card">
                <img src="https://github.com/user-attachments/assets/7adaee96-3cc2-4015-9aaa-0c8773b9db9f" alt="">
                <div class="overlay">
                    <h3>My Beautiful Girl ❤️</h3>
                    <p>Your smile means everything to me 🥺</p>
                </div>
            </div>

            <!-- PHOTO 2 -->
            <div class="photo-card">
                <img src="https://github.com/user-attachments/assets/362142cd-8d8f-4215-8435-3e0037671b85" alt="">
                <div class="overlay">
                    <h3>Forever My Favorite ✨</h3>
                    <p>You make life feel beautiful 💖</p>
                </div>
            </div>

            <!-- PHOTO 3 -->
            <div class="photo-card">
                <img src="photo3.jpg" alt="">
                <div class="overlay">
                    <h3>Us Together 🫶🏽</h3>
                    <p>The best memories are with you ❤️</p>
                </div>
            </div>

            <!-- PHOTO 4 -->
            <div class="photo-card">
                <img src="photo4.jpg" alt="">
                <div class="overlay">
                    <h3>Beautiful Moments 🌸</h3>
                    <p>I never want to lose these memories 💕</p>
                </div>
            </div>

            <!-- PHOTO 5 -->
            <div class="photo-card">
                <img src="photo5.jpg" alt="">
                <div class="overlay">
                    <h3>My Happiness 😊</h3>
                    <p>You are my peace and comfort 🥺</p>
                </div>
            </div>

            <!-- PHOTO 6 -->
            <div class="photo-card">
                <img src="photo6.jpg" alt="">
                <div class="overlay">
                    <h3>Forever Us 💍</h3>
                    <p>No matter what, I choose you ❤️</p>
                </div>
            </div>

        </div>

    </section>

    <!-- MEMORY SECTION -->

    <section class="memory">

        <h2>🌍 Why You Are Special To Me</h2>

        <p>
            Rita, your heart is one of the purest things I have ever known ❤️  
            You are sweet, caring, beautiful, loving, and truly unforgettable 🥺💖  
            Thank you for every smile, every conversation, every moment, and every memory ✨  
            Life feels softer and happier with you in it 🌸
        </p>

    </section>

    <!-- FOOTER -->

    <section class="footer">

        <h2>❤️ Forever Appreciated ❤️</h2>

        <p>
            No matter where life takes us, one thing will always remain true —  
            you will always have a special place in my heart 💖✨
        </p>

        <span>
            Rita & Roy Forever 🥺❤️
        </span>

    </section>

</body>

</html>
```
