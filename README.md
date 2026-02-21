# Melt-and-Toss
cloud kitchen with amazing taste and food at affordable price, newly launched dishes and taste like never before .
Owner - Ramesh  Kumar Jhamb/Yash Jhamb
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Melt and Toss - Cloud Kitchen</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="container">
            <div class="logo">🍳 Melt and Toss</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#reviews">Reviews</a></li>
                <li><a href="#location">Location</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Melt and Toss</h1>
            <p>Premium Cloud Kitchen - Freshly Made, Quickly Delivered</p>
            <button class="cta-btn" onclick="scrollToSection('menu')">Explore Menu</button>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" class="menu-section">
        <div class="container">
            <h2>Our Menu</h2>
            <div class="menu-filters">
                <button class="filter-btn active" onclick="filterMenu('all')">All</button>
                <button class="filter-btn" onclick="filterMenu('starters')">Starters</button>
                <button class="filter-btn" onclick="filterMenu('mains')">Mains</button>
                <button class="filter-btn" onclick="filterMenu('desserts')">Desserts</button>
                <button class="filter-btn" onclick="filterMenu('beverages')">Beverages</button>
            </div>
            <div class="menu-grid" id="menuGrid">
                <!-- Menu items will be loaded here by JavaScript -->
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="gallery-section">
        <div class="container">
            <h2>Photo Gallery</h2>
            <div class="gallery-grid" id="galleryGrid">
                <!-- Gallery images will be loaded here by JavaScript -->
            </div>
        </div>
    </section>

    <!-- Reviews Section -->
    <section id="reviews" class="reviews-section">
        <div class="container">
            <h2>Customer Reviews</h2>
            <div class="reviews-grid" id="reviewsGrid">
                <!-- Reviews will be loaded here by JavaScript -->
            </div>
        </div>
    </section>

    <!-- Location Section -->
    <section id="location" class="location-section">
        <div class="container">
            <h2>Find Us</h2>
            <div class="location-content">
                <div class="map-container">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3888.789353300876!2d77.22008!3d28.60915!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x390cef0c2c7a0001%3A0x1c1c1c1c1c1c1c1c!2sDelhi!5e0!3m2!1sen!2sin!4v1234567890" width="100%" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
                <div class="location-info">
                    <h3>Melt and Toss</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Food Street, Delhi, India 110001</p>
                    <p><i class="fas fa-phone"></i> +91-9876543210</p>
                    <p><i class="fas fa-envelope"></i> info@meltandtoss.com</p>
                    <p><i class="fas fa-clock"></i> Open: 11 AM - 11 PM (Daily)</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <div class="container">
            <h2>Get in Touch</h2>
            <div class="contact-content">
                <form class="contact-form" id="contactForm">
                    <input type="text" placeholder="Your Name" required>
                    <input type="email" placeholder="Your Email" required>
                    <textarea placeholder="Your Message" rows="5" required></textarea>
                    <button type="submit" class="submit-btn">Send Message</button>
                </form>
                <div class="social-links">
                    <h3>Follow Us</h3>
                    <a href="https://facebook.com/meltandtoss" target="_blank"><i class="fab fa-facebook"></i></a>
                    <a href="https://instagram.com/meltandtoss" target="_blank"><i class="fab fa-instagram"></i></a>
                    <a href="https://twitter.com/meltandtoss" target="_blank"><i class="fab fa-twitter"></i></a>
                    <a href="https://youtube.com/meltandtoss" target="_blank"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2026 Melt and Toss Cloud Kitchen. All rights reserved.</p>
            <p>Designed with ❤️ by Your Team</p>
        </div>
    </footer>

    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #FF6B35;
    --secondary-color: #F7931E;
    --dark-color: #1a1a1a;
    --light-color: #f4f4f4;
    --text-color: #333;
    --border-radius: 8px;
    --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Navigation */
.navbar {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: var(--box-shadow);
}

.navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.8rem;
    font-weight: bold;
    color: white;
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-weight: 500;
    transition: opacity 0.3s;
}

.nav-links a:hover {
    opacity: 0.8;
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: white;
    padding: 100px 20px;
    text-align: center;
    min-height: 500px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.hero-content h1 {
    font-size: 3.5rem;
    margin-bottom: 1rem;
    animation: slideDown 0.8s ease;
}

.hero-content p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
    animation: slideUp 0.8s ease;
}

.cta-btn {
    background: white;
    color: var(--primary-color);
    border: none;
    padding: 12px 30px;
    font-size: 1.1rem;
    border-radius: var(--border-radius);
    cursor: pointer;
    font-weight: bold;
    transition: transform 0.3s, box-shadow 0.3s;
}

.cta-btn:hover {
    transform: translateY(-3px);
    box-shadow: var(--box-shadow);
}

/* Menu Section */
.menu-section {
    padding: 60px 20px;
    background: var(--light-color);
}

.menu-section h2,
.gallery-section h2,
.reviews-section h2,
.location-section h2,
.contact-section h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 2rem;
    color: var(--primary-color);
}

.menu-filters {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin-bottom: 2rem;
    flex-wrap: wrap;
}

.filter-btn {
    padding: 10px 20px;
    border: 2px solid var(--primary-color);
    background: white;
    color: var(--primary-color);
    border-radius: var(--border-radius);
    cursor: pointer;
    font-weight: 600;
    transition: all 0.3s;
}

.filter-btn.active {
    background: var(--primary-color);
    color: white;
}

.filter-btn:hover {
    background: var(--primary-color);
    color: white;
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 2rem;
}

.menu-item {
    background: white;
    border-radius: var(--border-radius);
    overflow: hidden;
    box-shadow: var(--box-shadow);
    transition: transform 0.3s, box-shadow 0.3s;
}

.menu-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
}

.menu-item-image {
    width: 100%;
    height: 200px;
    object-fit: cover;
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 3rem;
}

.menu-item-content {
    padding: 1.5rem;
}

.menu-item-content h3 {
    color: var(--primary-color);
    margin-bottom: 0.5rem;
}

.menu-item-content p {
    color: #666;
    font-size: 0.9rem;
    margin-bottom: 1rem;
}

.menu-item-price {
    font-size: 1.5rem;
    color: var(--secondary-color);
    font-weight: bold;
}

/* Gallery Section */
.gallery-section {
    padding: 60px 20px;
}

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 1rem;
}

.gallery-item {
    position: relative;
    border-radius: var(--border-radius);
    overflow: hidden;
    height: 250px;
    cursor: pointer;
    box-shadow: var(--box-shadow);
}

.gallery-item-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 3rem;
    transition: transform 0.3s;
}

.gallery-item:hover .gallery-item-image {
    transform: scale(1.05);
}

.gallery-overlay {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.5);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.3s;
}

.gallery-item:hover .gallery-overlay {
    opacity: 1;
}

.gallery-overlay i {
    color: white;
    font-size: 2rem;
}

/* Reviews Section */
.reviews-section {
    padding: 60px 20px;
    background: var(--light-color);
}

.reviews-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 2rem;
}

.review-card {
    background: white;
    padding: 2rem;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    border-left: 4px solid var(--primary-color);
}

.review-header {
    display: flex;
    align-items: center;
    margin-bottom: 1rem;
}

.review-avatar {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-size: 1.5rem;
    margin-right: 1rem;
}

.review-info h3 {
    margin: 0;
    color: var(--primary-color);
}

.review-info p {
    margin: 0;
    color: #999;
    font-size: 0.9rem;
}

.stars {
    color: var(--secondary-color);
    margin: 0.5rem 0;
}

.review-text {
    color: #666;
    font-size: 0.95rem;
    line-height: 1.6;
}

/* Location Section */
.location-section {
    padding: 60px 20px;
}

.location-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    align-items: center;
}

.map-container {
    border-radius: var(--border-radius);
    overflow: hidden;
    box-shadow: var(--box-shadow);
}

.location-info {
    padding: 2rem;
}

.location-info h3 {
    font-size: 2rem;
    color: var(--primary-color);
    margin-bottom: 1.5rem;
}

.location-info p {
    margin-bottom: 1rem;
    font-size: 1.1rem;
    display: flex;
    align-items: center;
    gap: 1rem;
}

.location-info i {
    color: var(--primary-color);
    font-size: 1.3rem;
}

/* Contact Section */
.contact-section {
    padding: 60px 20px;
    background: var(--light-color);
}

.contact-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
}

.contact-form {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

.contact-form input,
.contact-form textarea {
    padding: 12px;
    border: 2px solid #ddd;
    border-radius: var(--border-radius);
    font-family: inherit;
    font-size: 1rem;
    transition: border-color 0.3s;
}

.contact-form input:focus,
.contact-form textarea:focus {
    outline: none;
    border-color: var(--primary-color);
}

.submit-btn {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: white;
    border: none;
    padding: 12px 30px;
    border-radius: var(--border-radius);
    font-size: 1.1rem;
    font-weight: bold;
    cursor: pointer;
    transition: transform 0.3s, box-shadow 0.3s;
}

.submit-btn:hover {
    transform: translateY(-3px);
    box-shadow: var(--box-shadow);
}

.social-links {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.social-links h3 {
    color: var(--primary-color);
    margin-bottom: 1.5rem;
}

.social-links {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.social-links a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 50px;
    height: 50px;
    background: var(--primary-color);
    color: white;
    border-radius: 50%;
    margin: 0.5rem;
    transition: background 0.3s, transform 0.3s;
    font-size: 1.5rem;
}

.social-links a:hover {
    background: var(--secondary-color);
    transform: translateY(-3px);
}

/* Footer */
.footer {
    background: var(--dark-color);
    color: white;
    padding: 2rem;
    text-align: center;
}

.footer p {
    margin: 0.5rem 0;
}

/* Animations */
@keyframes slideDown {
    from {
        opacity: 0;
        transform: translateY(-30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes slideUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Responsive Design */
@media (max-width: 768px) {
    .navbar .container {
        flex-direction: column;
        gap: 1rem;
    }

    .nav-links {
        flex-direction: column;
        gap: 0.5rem;
        text-align: center;
    }

    .hero-content h1 {
        font-size: 2.5rem;
    }

    .hero-content p {
        font-size: 1.1rem;
    }

    .menu-grid,
    .gallery-grid,
    .reviews-grid {
        grid-template-columns: 1fr;
    }

    .location-content,
    .contact-content {
        grid-template-columns: 1fr;
    }

    .menu-filters {
        flex-direction: column;
    }

    .filter-btn {
        width: 100%;
    }
}

    <script src="script.js"></script>
</body>
</html>
