<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minini</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
        }
        header {
            background: #333;
            color: white;
            padding: 1em;
        }
        main {
            padding: 20px;
        }
        .hero {
            width: 100%;
            height: 300px;
            background: url('hero-image.jpg') center/cover no-repeat;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2em;
            font-weight: bold;
            animation: fadeIn 2s ease-in-out;
        }
        .content {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
        }
        .content img {
            width: 300px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            transition: transform 0.3s ease-in-out;
        }
        .content img:hover {
            transform: scale(1.1);
        }
        footer {
            background: #333;
            color: white;
            padding: 1em;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const images = document.querySelectorAll(".content img");
            images.forEach(img => {
                img.addEventListener("click", function() {
                    alert("You clicked on " + this.alt);
                });
            });
        });
    </script>
</head>
<body>
    <header>
        <h1>Minini</h1>
    </header>
    <div class="hero">Amazing Views Await</div>
    <main>
        <p>Explore stunning landscapes and breathtaking moments captured just for you.</p>
        <div class="content">
            <img src="image1.jpg" alt="Beautiful Scenery">
            <img src="image2.jpg" alt="Mountain View">
            <img src="image3.jpg" alt="Sunset by the Beach">
        </div>
    </main>
    <footer>
        <p>&copy; 2025 My Website</p>
    </footer>
</body>
</html>

