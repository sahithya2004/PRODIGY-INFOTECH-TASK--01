# PRODIGY-INFOTECH-TASK--01
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PRODIGY INFOTECH</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header">
        <nav class="navbar" id="navbar">
            <div class="logo">
                <h1>PRODIGY INFOTECH</h1>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="section">
        <h2>Welcome to PRODIGY INFOTECH</h2>
        <p>Your technology partner for innovative solutions.</p>
    </section>
    
    <!-- Additional sections like About, Services, Contact -->

    <script src="script.js"></script>
</body>
</html>

CSS

body {
    margin: 0;
    font-family: Arial, sans-serif;
}

/* Header Styles */
.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background: #333;
    color: #fff;
    z-index: 1000;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
}

.navbar .logo h1 {
    margin: 0;
    font-size: 1.5em;
}

.nav-links {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    text-decoration: none;
    color: #fff;
    font-size: 1em;
    transition: color 0.3s;
}

/* Hover and Scroll Effects */
.nav-links a:hover {
    color: #ffcc00;
}

.scrolled .navbar {
    background: #222; /* Darker background when scrolled */
}

.section {
    padding: 100px 20px 20px;
    text-align: center;
}

.section:nth-child(even) {
    background: #f9f9f9;
}

.section h2 {
    margin: 0;
}

JAVASCRIPT

document.addEventListener('DOMContentLoaded', () => {
    const navbar = document.getElementById('navbar');

    window.addEventListener('scroll', () => {
        if (window.scrollY > 50) {
            navbar.classList.add('scrolled');
        } else {
            navbar.classList.remove('scrolled');
        }
    });
});
