<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kondeti Dhanush - Portfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@100;400;700&display=swap" rel="stylesheet">
    <style>
        /* Global Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body Styling */
        body {
            background-color: rgb(0, 0, 33);
            color: white;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
        }

        /* Smooth Scrolling */
        html {
            scroll-behavior: smooth;
        }

        /* Navigation Bar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 80px;
            padding: 0 40px;
            background-color: rgba(18, 18, 62, 0.8);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav .left a {
            text-decoration: none;
            color: white;
            font-size: 2rem;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav .left a:hover {
            color: rgb(170, 107, 228);
        }

        nav ul {
            display: flex;
            justify-content: center;
            margin: 0;
            padding: 0;
            list-style: none;
        }

        nav ul li {
            margin: 0 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: white;
            font-size: 1.1rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: rgb(170, 107, 228);
        }

        /* Home Section Styling */
        .firstSection {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 120px 40px 50px;
            padding: 50px;
            background: linear-gradient(145deg, rgba(30,30,60,1) 0%, rgba(0,0,50,1) 100%);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }

        .leftSection {
            width: 45%;
            padding: 20px;
            text-align: left;
            animation: fadeInLeft 1s ease-out;
        }

        .leftSection p {
            font-size: 3.5rem;
            line-height: 1.2;
            font-weight: bold;
        }

        .purple {
            color: rgb(170, 107, 228);
        }

        #element {
            color: rgb(170, 107, 228); /* Typed.js text color */
        }

        /* Button Styling */
        .btn {
            background-color: rgb(170, 107, 228);
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1rem;
            font-weight: bold;
            text-transform: uppercase;
            border-radius: 50px;
            margin-right: 10px;
            cursor: pointer;
            text-decoration: none;
            transition: background-color 0.3s ease, transform 0.3s ease;
            box-shadow: 0 5px 15px rgba(170, 107, 228, 0.5);
        }

        .btn:hover {
            background-color: rgb(153, 153, 226);
            transform: translateY(-5px);
        }

        .btn-container {
            margin-top: 30px;
            display: flex;
        }

        /* Right Section Image */
        .rightSection {
            width: 45%;
            display: flex;
            justify-content: center;
            align-items: center;
            animation: fadeInRight 1s ease-out;
        }

        .rightSection img {
            width: 100%;
            max-width: 400px;
            filter: drop-shadow(0 5px 20px rgba(0, 0, 0, 0.5));
            border-radius: 15px;
        }

        /* Keyframes for animations */
        @keyframes fadeInLeft {
            0% {
                opacity: 0;
                transform: translateX(-50px);
            }
            100% {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes fadeInRight {
            0% {
                opacity: 0;
                transform: translateX(50px);
            }
            100% {
                opacity: 1;
                transform: translateX(0);
            }
        }

        /* Media Query for mobile responsiveness */
        @media only screen and (max-width: 768px) {
            .firstSection {
                flex-direction: column;
                text-align: center;
                margin: 80px 20px;
            }
            .leftSection, .rightSection {
                width: 100%;
            }
            .rightSection img {
                width: 80%;
            }
            nav {
                padding: 0 20px;
            }
            .leftSection p {
                font-size: 2.5rem;
            }
        }

    </style>
</head>
<body>
    <header>
        <nav>
            <div class="left"><a href="/">Kondeti Dhanush's Portfolio</a></div>
            <div class="right">
                <ul>
                    <li><a href="/">Home</a></li>
                    <li><a href='/about'>About</a></li>
                    <li><a href="https://github.com/dhanushbunny26/dhanushbunny26" target="_blank">Projects</a></li>
                    <li><a href='/about#contact'>Contact Me</a></li>
                </ul>
            </div>
        </nav>
    </header>

    <main>
        <!-- Home Section -->
        <section class="firstSection">
            <div class="leftSection">
                <p>Hi, My name is <span class="purple">Kondeti Dhanush</span> and I am a passionate <span id="element"></span></p>
                <div class="btn-container">
                    <!-- Download Resume button redirecting to the external link -->
                    <a href="SIST-BE-CSE-CS-41614046-KONDETI DHANUSH.pdf" target="_blank" class="btn">Download Resume</a>
                    <!-- Visit GitHub button -->
                    <a href="https://github.com/dhanushbunny26/dhanushbunny26" target="_blank" class="btn">Visit GitHub</a>
                </div>
            </div>
            <div class="rightSection">
                <img src="IMG-20240823-WA0019[1].jpg" alt="Kondeti Dhanush Working Image">
            </div>
        </section>
    </main>

    <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            var typed = new Typed('#element', {
                strings: ['Cyber Security Analyst', 'Web Developer', 'UI/UX Designer'],
                typeSpeed: 50,
                backSpeed: 30,
                loop: true,
                startDelay: 500,
                backDelay: 1000
            });
        });
    </script>
</body>
</html>
