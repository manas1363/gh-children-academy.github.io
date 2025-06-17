# gh-children-academy.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GH Children Academy</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to GH Children Academy</h1>
        <nav>
            <ul>
                <li><a href="#about">About Us</a></li>
                <li><a href="#programs">Programs</a></li>
                <li><a href="#admissions">Admissions</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>About Us</h2>
        <p>GH Children Academy is a nurturing environment where young minds grow and explore. Our play-based curriculum fosters creativity, curiosity, and social development.</p>
    </section>

    <section id="programs">
        <h2>Our Programs</h2>
        <ul>
            <li>Playgroup</li>
            <li>Nursery</li>
            <li>Kindergarten</li>
        </ul>
    </section>

    <section id="admissions">
        <h2>Admissions</h2>
        <p>Enrollment is open for the upcoming academic year. Visit our campus or contact us for more information.</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>Email: info@ghchildrenacademy.com</p>
        <p>Phone: +91 123 456 7890</p>
    </section>

    <footer>
        <p>&copy; 2025 GH Children Academy</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f0f8ff;
    color: #333;
}

header {
    background-color: #ffcc00;
    padding: 20px;
    text-align: center;
}

header h1 {
    margin: 0;
    font-size: 2.5em;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    text-decoration: none;
    color: #333;
    font-weight: bold;
}

section {
    padding: 20px;
    margin: 10px;
    background-color: #ffffff;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

footer {
    background-color: #ffcc00;
    text-align: center;
    padding: 10px;
    position: fixed;
    width: 100%;
    bottom: 0;
}
document.addEventListener('DOMContentLoaded', () => {
    const navLinks = document.querySelectorAll('nav ul li a');
    navLinks.forEach(link => {
        link.addEventListener('click', event => {
            event.preventDefault();
            const targetId = link.getAttribute('href').substring(1);
            const targetSection = document.getElementById(targetId);
            window.scrollTo({
                top: targetSection.offsetTop - 20,
                behavior: 'smooth'
            });
        });
    });
});
