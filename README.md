# blueushersuganda.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blue Ushers Uganda Ltd - Professional Ushering Services</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #2c5aa0, #1e3d72);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #87ceeb;
        }

        .menu-toggle {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(44, 90, 160, 0.8), rgba(30, 61, 114, 0.8)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23f0f8ff" width="1200" height="600"/><path fill="%232c5aa0" opacity="0.1" d="M0,300 Q300,200 600,300 T1200,300 L1200,600 L0,600 Z"/></svg>');
            height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            animation: fadeInUp 1s ease;
        }

        .hero-content p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            animation: fadeInUp 1s ease 0.3s both;
        }

        .cta-button {
            display: inline-block;
            background: #ff6b35;
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: all 0.3s;
            animation: fadeInUp 1s ease 0.6s both;
        }

        .cta-button:hover {
            background: #e55a2b;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }

        /* Sections */
        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #2c5aa0;
        }

        /* Services */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .service-icon {
            width: 80px;
            height: 80px;
            background: #2c5aa0;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1rem;
            color: white;
            font-size: 2rem;
        }

        /* About */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text {
            font-size: 1.1rem;
            line-height: 1.8;
        }

        .about-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1rem;
            margin-top: 2rem;
        }

        .stat-card {
            background: #f8f9fa;
            padding: 1.5rem;
            border-radius: 10px;
            text-align: center;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #2c5aa0;
        }

        /* Booking Form */
        .booking-form {
            background: #f8f9fa;
            padding: 3rem;
            border-radius: 15px;
            max-width: 600px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
            color: #2c5aa0;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }

        .form-group textarea {
            height: 120px;
            resize: vertical;
        }

        .submit-btn {
            background: #2c5aa0;
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
            width: 100%;
        }

        .submit-btn:hover {
            background: #1e3d72;
        }

        /* Contact */
        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .contact-card {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
        }

        .contact-icon {
            width: 60px;
            height: 60px;
            background: #ff6b35;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1rem;
            color: white;
            font-size: 1.5rem;
        }

        /* Footer */
        footer {
            background: #1e3d72;
            color: white;
            text-align: center;
            padding: 2rem 0;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Responsive */
        @media (max-width: 768px) {
            .menu-toggle {
                display: block;
            }

            .nav-links {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: #2c5aa0;
                flex-direction: column;
                padding: 1rem;
            }

            .nav-links.active {
                display: flex;
            }

            .hero-content h1 {
                font-size: 2.5rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .services-grid,
            .contact-info {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <div class="logo">Blue Ushers Uganda</div>
            <button class="menu-toggle" id="menuToggle">☰</button>
            <ul class="nav-links" id="navLinks">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#book">Book Now</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>Professional Ushering Services</h1>
                <p>Elevating events with grace, professionalism, and exceptional service across Uganda</p>
                <a href="#book" class="cta-button">Book Our Services</a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">🎭</div>
                    <h3>Event Ushering</h3>
                    <p>Professional ushers for conferences, seminars, and corporate events. We ensure smooth guest management and exceptional hospitality.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">💒</div>
                    <h3>Wedding Ushering</h3>
                    <p>Make your special day perfect with our elegant wedding ushers who guide guests with grace and ensure seamless ceremony flow.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🎓</div>
                    <h3>Graduation Ceremonies</h3>
                    <p>Experienced ushers for graduation events, managing crowd flow and ensuring dignified proceedings for this milestone occasion.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🎪</div>
                    <h3>Entertainment Events</h3>
                    <p>Dynamic ushering services for concerts, shows, and entertainment venues with focus on safety and guest satisfaction.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🏢</div>
                    <h3>Corporate Functions</h3>
                    <p>Professional support for board meetings, AGMs, and corporate gatherings with discretion and efficiency.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">⛪</div>
                    <h3>Religious Ceremonies</h3>
                    <p>Respectful and courteous ushering for religious events, maintaining the sanctity and order of the occasion.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <h2 class="section-title">About Blue Ushers Uganda</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Blue Ushers Uganda Ltd is a premier ushering company dedicated to providing exceptional hospitality services across Uganda. With years of experience in event management and customer service, we pride ourselves on delivering professional, courteous, and reliable ushering services.</p>
                    
                    <p>Our team consists of highly trained professionals who understand the importance of first impressions and seamless event execution. We work closely with event organizers to ensure every guest feels welcomed and every detail is perfectly managed.</p>
                    
                    <p>Whether it's a corporate event, wedding, graduation, or any special occasion, Blue Ushers Uganda is committed to elevating your event experience through our dedication to excellence and professionalism.</p>
                </div>
                <div class="about-stats">
                    <div class="stat-card">
                        <div class="stat-number">500+</div>
                        <p>Events Served</p>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">98%</div>
                        <p>Client Satisfaction</p>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">50+</div>
                        <p>Trained Ushers</p>
                    </div>
                    <div class="stat-card">
                        <div class="stat-number">5</div>
                        <p>Years Experience</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Booking Section -->
    <section id="book">
        <div class="container">
            <h2 class="section-title">Book Our Services</h2>
            <form class="booking-form" id="bookingForm">
                <div class="form-group">
                    <label for="eventType">Event Type</label>
                    <select id="eventType" required>
                        <option value="">Select Event Type</option>
                        <option value="wedding">Wedding</option>
                        <option value="corporate">Corporate Event</option>
                        <option value="conference">Conference/Seminar</option>
                        <option value="graduation">Graduation</option>
                        <option value="entertainment">Entertainment Event</option>
                        <option value="religious">Religious Ceremony</option>
                        <option value="other">Other</option>
                    </select>
                </div>
                
                <div class="form-group">
                    <label for="clientName">Your Name</label>
                    <input type="text" id="clientName" required>
                </div>
                
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" required>
                </div>
                
                <div class="form-group">
                    <label for="phone">Phone Number</label>
                    <input type="tel" id="phone" required>
                </div>
                
                <div class="form-group">
                    <label for="eventDate">Event Date</label>
                    <input type="date" id="eventDate" required>
                </div>
                
                <div class="form-group">
                    <label for="venue">Venue</label>
                    <input type="text" id="venue" required>
                </div>
                
                <div class="form-group">
                    <label for="guestCount">Expected Guest Count</label>
                    <input type="number" id="guestCount" min="1" required>
                </div>
                
                <div class="form-group">
                    <label for="ushersNeeded">Number of Ushers Needed</label>
                    <input type="number" id="ushersNeeded" min="1" required>
                </div>
                
                <div class="form-group">
                    <label for="requirements">Special Requirements</label>
                    <textarea id="requirements" placeholder="Please describe any special requirements or additional information..."></textarea>
                </div>
                
                <button type="submit" class="submit-btn">Submit Booking Request</button>
            </form>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <h2 class="section-title">Contact Us</h2>
            <div class="contact-info">
                <div class="contact-card">
                    <div class="contact-icon">📍</div>
                    <h3>Our Office</h3>
                    <p>Kampala, Uganda<br>Plot 123, Business District</p>
                </div>
                <div class="contact-card">
                    <div class="contact-icon">📞</div>
                    <h3>Phone</h3>
                    <p>+256 700 123 456<br>+256 750 789 012</p>
                </div>
                <div class="contact-card">
                    <div class="contact-icon">✉️</div>
                    <h3>Email</h3>
                    <p>info@blueushersuganda.com<br>bookings@blueushersuganda.com</p>
                </div>
                <div class="contact-card">
                    <div class="contact-icon">⏰</div>
                    <h3>Business Hours</h3>
                    <p>Monday - Friday: 8AM - 6PM<br>Saturday: 9AM - 4PM</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 Blue Ushers Uganda Ltd. All rights reserved. | Professional Ushering Services</p>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');

        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                target.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
                // Close mobile menu if open
                navLinks.classList.remove('active');
            });
        });

        // Form submission
        const bookingForm = document.getElementById('bookingForm');
        bookingForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(bookingForm);
            const bookingData = {};
            formData.forEach((value, key) => {
                bookingData[key] = value;
            });
            
            // Simulate form submission
            alert('Thank you for your booking request! We will contact you within 24 hours to confirm your booking and discuss further details.');
            bookingForm.reset();
        });

        // Set minimum date to today for event date input
        const eventDateInput = document.getElementById('eventDate');
        const today = new Date().toISOString().split('T')[0];
        eventDateInput.setAttribute('min', today);

        // Dynamic usher count suggestion based on guest count
        const guestCountInput = document.getElementById('guestCount');
        const ushersNeededInput = document.getElementById('ushersNeeded');

        guestCountInput.addEventListener('input', function() {
            const guestCount = parseInt(this.value);
            if (guestCount > 0) {
                // Suggest 1 usher per 50 guests (minimum 2)
                const suggestedUshers = Math.max(2, Math.ceil(guestCount / 50));
                ushersNeededInput.value = suggestedUshers;
            }
        });

        // Header scroll effect
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.background = 'linear-gradient(135deg, #1e3d72, #0f2749)';
            } else {
                header.style.background = 'linear-gradient(135deg, #2c5aa0, #1e3d72)';
            }
        });
    </script>
</body>
</html>
