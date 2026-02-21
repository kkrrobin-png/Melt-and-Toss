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

    <script src="script.js"></script>
</body>
</html>
