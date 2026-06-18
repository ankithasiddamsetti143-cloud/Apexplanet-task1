#<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ApexPlanet Static Website | Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header class="navbar">
        <div class="logo">ApexPlanet</div>
        <nav>
            <ul class="nav-links">
                <li><a href="index.html" class="active">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1>Welcome to Modern Web Development</h1>
                <p>Building high-performance, responsive static websites using HTML5 & CSS3.</p>
                <a href="#features" class="btn">Explore Features</a>
            </div>
        </section>

        <section id="features" class="container">
            <h2 class="section-title">Our Core Pillars</h2>
            <div class="grid-layout">
                <div class="card">
                    <h3>Semantic HTML5</h3>
                    <p>Utilizing clean, accessible, and SEO-friendly structures to give your content clear meaning.</p>
                </div>
                <div class="card">
                    <h3>Responsive CSS3</h3>
                    <p>Leveraging Flexbox and CSS Grid to ensure pixel-perfect layouts across mobile, tablet, and desktop.</p>
                </div>
                <div class="card">
                    <h3>Clean Architecture</h3>
                    <p>Maintainable, scalable folder structures designed for modern static deployment pipelines.</p>
                </div>
            </div>
        </section>
    </main>

    <footer class="footer">
        <p>&copy; 2026 ApexPlanet Software Pvt. Ltd. All rights reserved.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us | ApexPlanet</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <header class="navbar">
        <div class="logo">ApexPlanet</div>
        <nav>
            <ul class="nav-links">
                <li><a href="index.html">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="contact.html" class="active">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main class="container">
        <h2 class="section-title">Get In Touch</h2>
        
        <div class="contact-wrapper">
            <div class="form-container">
                <form action="#" method="POST" class="contact-form">
                    <div class="form-group">
                        <label for="name">Full Name</label>
                        <input type="text" id="name" name="name" placeholder="John Doe" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email Address</label>
                        <input type="email" id="email" name="email" placeholder="john@example.com" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Your Message</label>
                        <textarea id="message" name="message" rows="5" placeholder="How can we help you?" required></textarea>
                    </div>
                    <button type="submit" class="btn">Send Message</button>
                </form>
            </div>

            <div class="map-container">
                <iframe 
                    src="https://www.google.com/maps/embed?pb=!11m18!1m12!1m3!1d3806.7507644365775!2d78.3820251!3d17.4477532!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3bcb91c5f3e53d59%3A0x6b77ad987f2e15b6!2sHITEC%20City%2C%20Hyderabad%2C%20Telangana!5e0!3m2!1sen!2sin!4v1710000000000!5m2!1sen!2sin" 
                    width="100%" 
                    height="100%" 
                    style="border:0; min-height: 300px;" 
                    allowfullscreen="" 
                    loading="lazy" 
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
        </div>
    </main>

    <footer class="footer">
        <p>&copy; 2026 ApexPlanet Software Pvt. Ltd. All rights reserved.</p>
    </footer>

</body>
</html>
/* --- Global Reset & Box Model --- */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f8f9fa;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

main {
    flex: 1;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 40px 20px;
}

/* --- Header / Navigation Bar (Flexbox) --- */
.navbar {
    background-color: #0f4c3a; /* Matching the green theme from your slide */
    color: #fff;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 40px;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.navbar .logo {
    font-size: 1.5rem;
    font-weight: bold;
    letter-spacing: 1px;
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 20px;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav-links a:hover, 
.nav-links a.active {
    color: #a3e635; /* Accent light green highlighting */
}

/* --- Hero Section --- */
.hero {
    background: linear-gradient(rgba(15, 76, 58, 0.85), rgba(15, 76, 58, 0.95)), 
                url('https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?q=80&w=1200') no-repeat center center/cover;
    color: #fff;
    height: 60vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 20px;
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: 30px;
    max-width: 600px;
    margin-inline: auto;
}

.btn {
    display: inline-block;
    background-color: #a3e635;
    color: #0f4c3a;
    padding: 12px 28px;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    border: none;
    cursor: pointer;
    transition: background 0.3s;
}

.btn:hover {
    background-color: #84cc16;
}

/* --- Card Layout (CSS Grid) --- */
.section-title {
    text-align: center;
    font-size: 2.2rem;
    margin-bottom: 40px;
    color: #0f4c3a;
}

.grid-layout {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.card {
    background: #fff;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
    border-top: 5px solid #0f4c3a;
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
}

.card h3 {
    margin-bottom: 15px;
    color: #0f4c3a;
}

/* --- Contact Page Layout (Flexbox / Grid Combo) --- */
.contact-wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 40px;
    background: #fff;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
}

.contact-form {
    display: flex;
    flex-direction: column;
    gap: 20px;
}

.form-group {
    display: flex;
    flex-direction: column;
    gap: 8px;
}

.form-group label {
    font-weight: 600;
    color: #0f4c3a;
}

.form-group input, 
.form-group textarea {
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 1rem;
}

.form-group input:focus, 
.form-group textarea:focus {
    outline: 2px solid #0f4c3a;
}

.map-container {
    border-radius: 6px;
    overflow: hidden;
}

/* --- Footer --- */
.footer {
    background-color: #111;
    color: #aaa;
    text-align: center;
    padding: 20px;
    font-size: 0.9rem;
    margin-top: auto;
}

/* --- Media Queries (Responsiveness) --- */

/* Tablets and below (max-width: 768px) */
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
        gap: 15px;
        padding: 15px;
    }

    .hero-content h1 {
        font-size: 2.2rem;
    }

    .contact-wrapper {
        grid-template-columns: 1fr; /* Stack form and map vertically */
    }
}

/* Mobile Screens (max-width: 480px) */
@media (max-width: 480px) {
    .nav-links {
        flex-direction: column;
        align-items: center;
        gap: 10px;
    }
    
    .hero-content h1 {
        font-size: 1.8rem;
    }
}