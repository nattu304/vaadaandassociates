<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vaada and Associates Name | Professional Accounting Services</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #34495e;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Header styles */
        header {
            background-color: var(--primary-color);
            color: white;
            padding: 20px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: white;
            text-decoration: none;
        }
        
        .nav-menu {
            display: flex;
            list-style: none;
        }
        
        .nav-menu li {
            margin-left: 30px;
        }
        
        .nav-menu a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-menu a:hover {
            color: var(--secondary-color);
        }
        
        .hamburger {
            display: none;
            cursor: pointer;
        }
        
        /* Hero section */
        .hero {
            background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(44, 62, 80, 0.8)), url('/api/placeholder/1200/600') center/cover no-repeat;
            height: 80vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
            margin-top: 70px;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary-color);
            color: white;
            padding: 12px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        /* Services section */
        .section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            font-size: 2.2rem;
            color: var(--primary-color);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
        }
        
        .service-card h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
            font-size: 1.4rem;
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
        }
        
        /* About section */
        .about {
            background-color: var(--light-color);
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-text h2 {
            color: var(--primary-color);
            margin-bottom: 20px;
            font-size: 2rem;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        /* Team section */
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .team-member {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
        }
        
        .team-image {
            height: 250px;
            background-color: #ddd;
        }
        
        .team-info {
            padding: 20px;
        }
        
        .team-info h3 {
            color: var(--primary-color);
            margin-bottom: 5px;
        }
        
        .team-info p {
            color: var(--secondary-color);
            font-weight: 500;
            margin-bottom: 15px;
        }
        
        /* Testimonials section */
        .testimonials {
            background-color: var(--primary-color);
            color: white;
        }
        
        .testimonials .section-title {
            color: white;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 10px;
            position: relative;
        }
        
        .testimonial-text {
            margin-bottom: 20px;
            font-style: italic;
        }
        
        .client-info {
            display: flex;
            align-items: center;
        }
        
        .client-image {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: var(--secondary-color);
            margin-right: 15px;
        }
        
        /* Contact section */
        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }
        
        .contact-info h3 {
            color: var(--primary-color);
            margin-bottom: 20px;
            font-size: 1.5rem;
        }
        
        .contact-details {
            margin-bottom: 30px;
        }
        
        .contact-details p {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }
        
        .contact-icon {
            color: var(--secondary-color);
            margin-right: 10px;
            font-size: 1.2rem;
        }
        
        .contact-form .form-group {
            margin-bottom: 20px;
        }
        
        .contact-form label {
            display: block;
            margin-bottom: 5px;
            color: var(--primary-color);
            font-weight: 500;
        }
        
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        .contact-form textarea {
            height: 150px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: var(--secondary-color);
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #bbb;
            font-size: 0.9rem;
        }
        
        /* Responsive styles */
        @media (max-width: 768px) {
            .header-container {
                padding: 0 20px;
            }
            
            .nav-menu {
                position: fixed;
                top: 70px;
                left: -100%;
                flex-direction: column;
                background-color: var(--primary-color);
                width: 100%;
                text-align: center;
                transition: 0.3s;
                box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
                padding: 10px 0;
            }
            
            .nav-menu.active {
                left: 0;
            }
            
            .nav-menu li {
                margin: 15px 0;
            }
            
            .hamburger {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .about-content,
            .contact-content {
                grid-template-columns: 1fr;
            }
            
            .about-image {
                order: -1;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Vaada and Associates</a>
            <ul class="nav-menu">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#team">Our Team</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburger">
                <div class="bar"></div>
                <div class="bar"></div>
                <div class="bar"></div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Professional Accounting Services for Your Business</h1>
                <p>We provide expert financial guidance to help your business thrive in today's complex economic landscape.</p>
                <a href="#contact" class="btn">Schedule a Consultation</a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section" id="services">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">📊</div>
                    <h3>Tax Planning & Preparation</h3>
                    <p>Strategic tax planning and preparation services to minimize your tax burden and ensure compliance with all regulations.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📈</div>
                    <h3>Financial Advisory</h3>
                    <p>Expert financial guidance to help you make informed decisions for sustainable business growth and profitability.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📝</div>
                    <h3>Auditing Services</h3>
                    <p>Comprehensive auditing services to verify financial statements and ensure accuracy and compliance with standards.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">💼</div>
                    <h3>Business Consulting</h3>
                    <p>Strategic business consulting to optimize your operations, improve performance, and achieve your business goals.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📚</div>
                    <h3>Bookkeeping</h3>
                    <p>Reliable bookkeeping services to maintain accurate financial records and provide you with clear insights into your finances.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">⚖️</div>
                    <h3>Regulatory Compliance</h3>
                    <p>Expert guidance to navigate complex regulatory requirements and ensure your business remains compliant at all times.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="section about" id="about">
        <div class="container">
            <h2 class="section-title">About Us</h2>
            <div class="about-content">
                <div class="about-text">
                    <h2>Your Trusted Financial Partner</h2>
                    <p>With over 15 years of experience in the accounting industry, our firm has been providing exceptional financial services to businesses of all sizes. Our team of certified professionals is dedicated to helping you navigate the complex world of finance and taxation.</p>
                    <p>We pride ourselves on our personalized approach, taking the time to understand your unique business needs and tailoring our services accordingly. Our commitment to excellence, integrity, and client satisfaction has made us a trusted partner for hundreds of businesses.</p>
                    <p>Whether you're a startup looking for guidance or an established company seeking to optimize your financial operations, we have the expertise and resources to help you succeed.</p>
                </div>
                <div class="about-image">
                    <img src="/api/placeholder/600/400" alt="Our office">
                </div>
            </div>
        </div>
    </section>

    <!-- Team Section -->
    <section class="section" id="team">
        <div class="container">
            <h2 class="section-title">Our Expert Team</h2>
            <div class="team-grid">
                <div class="team-member">
                    <div class="team-image">
                        <!-- Placeholder for team member image -->
                    </div>
                    <div class="team-info">
                        <h3>John Smith</h3>
                        <p>Managing Partner</p>
                        <p>With over 20 years of experience in accounting and finance, John leads our team with expertise and vision.</p>
                    </div>
                </div>
                <div class="team-member">
                    <div class="team-image">
                        <!-- Placeholder for team member image -->
                    </div>
                    <div class="team-info">
                        <h3>Sarah Johnson</h3>
                        <p>Tax Specialist</p>
                        <p>Sarah's expertise in tax planning has helped countless clients optimize their tax positions and save money.</p>
                    </div>
                </div>
                <div class="team-member">
                    <div class="team-image">
                        <!-- Placeholder for team member image -->
                    </div>
                    <div class="team-info">
                        <h3>Michael Chen</h3>
                        <p>Audit Manager</p>
                        <p>Michael ensures all our audit processes meet the highest standards of accuracy and compliance.</p>
                    </div>
                </div>
                <div class="team-member">
                    <div class="team-image">
                        <!-- Placeholder for team member image -->
                    </div>
                    <div class="team-info">
                        <h3>Emily Rodriguez</h3>
                        <p>Business Advisor</p>
                        <p>Emily combines financial expertise with strategic thinking to provide valuable business insights.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="section testimonials" id="testimonials">
        <div class="container">
            <h2 class="section-title">What Our Clients Say</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "Vaada and Associates has been instrumental in helping our business navigate complex tax regulations. Their expert advice has saved us both time and money."
                    </div>
                    <div class="client-info">
                        <div class="client-image"></div>
                        <div>
                            <h4>Robert Johnson</h4>
                            <p>CEO, Johnson Enterprises</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "We've been working with Vaada and Associates for over 5 years now, and their service has been consistently excellent. Their attention to detail and proactive approach sets them apart."
                    </div>
                    <div class="client-info">
                        <div class="client-image"></div>
                        <div>
                            <h4>Linda Miller</h4>
                            <p>Owner, Miller Retail Group</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "As a small business owner, I was struggling with financial management until I found Vaada and Associates. Their guidance has been invaluable to our growth."
                    </div>
                    <div class="client-info">
                        <div class="client-image"></div>
                        <div>
                            <h4>David Thompson</h4>
                            <p>Founder, Thompson Design</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section" id="contact">
        <div class="container">
            <h2 class="section-title">Get In Touch</h2>
            <div class="contact-content">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <div class="contact-details">
                        <p><span class="contact-icon">📍</span> 123 Business Avenue, Suite 200, City, State 12345</p>
                        <p><span class="contact-icon">📞</span> (123) 456-7890</p>
                        <p><span class="contact-icon">📧</span> info@yourcafirm.com</p>
               