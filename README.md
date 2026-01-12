index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <div class="fade-container">

        <!-- Hero Section -->
        <section class="hero">
            <h1>Happy Birthday, Her Name</h1>
            <p class="subline">You mean more to me than I can ever put into words.</p>
        </section>

        <!-- Message Section -->
        <section class="message">
            <p>
                Thank you for being a ray of calm in my life. You bring a kind of happiness I didn't know I needed.
                I might not have much to give right now, but I wanted to make something that reminds you how special you are to me.
                I hope this small corner of the internet makes you smile today. Happiest birthday to you.
            </p>
        </section>

        <!-- Gallery Section -->
        <section class="gallery">
            <div class="img-box">Image 1</div>
            <div class="img-box">Image 2</div>
            <div class="img-box">Image 3</div>
        </section>

        <!-- Final Note -->
        <section class="final-note">
            <p>I’m grateful for you. Today and always.</p>
        </section>

        <!-- Footer -->
        <footer>
            <div class="heart">❤</div>
        </footer>

    </div>

<script src="script.js"></script>
</body>
</html>
styles.css
/* Soft pastel background */
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #fde5ec, #e8f0ff);
    color: #333;
    text-align: center;
}

/* Smooth fade container */
.fade-container {
    opacity: 0;
    transition: opacity 1.5s ease;
}

/* Hero Section */
.hero {
    padding: 80px 20px 50px;
}

.hero h1 {
    font-size: 2.3rem;
    font-weight: 600;
    color: #444;
}

.subline {
    font-size: 1.1rem;
    margin-top: 10px;
    color: #666;
}

/* Message Section */
.message {
    padding: 20px 25px;
    max-width: 600px;
    margin: auto;
    line-height: 1.7;
    color: #555;
}

/* Gallery Section */
.gallery {
    display: flex;
    justify-content: center;
    gap: 15px;
    padding: 30px 10px;
    flex-wrap: wrap;
}

.img-box {
    width: 160px;
    height: 180px;
    background: #ffffffaa;
    border-radius: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #777;
    font-size: 0.9rem;
    border: 1px solid #eee;
}

/* Final Note */
.final-note {
    padding: 20px 20px 40px;
    font-size: 1.1rem;
    color: #444;
}

/* Footer */
footer {
    padding-bottom: 25px;
}

.heart {
    font-size: 22px;
    animation: glow 2s infinite ease-in-out;
}

@keyframes glow {
    0% { opacity: 0.5; }
    50% { opacity: 1; }
    100% { opacity: 0.5; }
}
script.js
window.onload = () => {
    document.querySelector(".fade-container").style.opacity = "1";
};
