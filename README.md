<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real Estate</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

<header>
    <nav class="navbar">
        <a href="#" class="nav-logo">
            <h2 class="logo-text">Real Estate</h2>
        </a>
        <ul class="nav-menu">
            <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
            <li class="nav-item"><a href="About.html" class="nav-link">About</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Properties</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Gallery</a></li>
            <li class="contact-section"><a class="nav-link" href="contact.html">Contact Us</a></li>
        </ul>
    </nav>
</header>

<main>
    <section class="hero-section">
        <div class="section-content">
            <div class="hero-details">
                <h2 class="title">Find Your Dream Home</h2>
                <section class="center">
                    <form action="search.html" method="post">
                        <h3>FIND YOUR PERFECT HOME</h3>
                        <div class="box">
                            <p>Enter Location <span>*</span></p>
                            <input type="text" name="location" required maxlength="50" placeholder="Enter city name" class="input">
                        </div>
                        <div class="flex">
                            <div class="box">
                                <p>Property Type <span>*</span></p>
                                <select name="type" class="input" required>
                                    <option value="flat">Flat</option>
                                    <option value="house">House</option>
                                    <option value="land">Land</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Select City <span>*</span></p>
                                <select name="place" class="input" required>
                                    <option value="Kathmandu">Kathmandu</option>
                                    <option value="Lalitpur">Lalitpur</option>
                                    <option value="Bhaktapur">Bhaktapur</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Minimum Budget <span>*</span></p>
                                <select name="budget" class="input" required>
                                    <option value="200000-500000">20K-50K</option>
                                    <option value="1000000-2000000">1Lac-2Lac</option>
                                    <option value="10000000-500000000">1Crore-5Crore</option>
                                </select>
                            </div>
                        </div>
                        <input type="submit" value="Search Property" name="search" class="btn">
                    </form>
                </section>
            </div>
        </div>
        
    </section>
</main>
<footer>
    <div class="footer-container">
        <div class="footer-info">
            <h3>Contact Us</h3>
            <p><strong>Phone:</strong> +977-1234567890</p>
            <p><strong>Email:</strong> info@realestate.com</p>
            <p><strong>Location:</strong> Kathmandu, Nepal</p>
        </div>
        <div class="footer-links">
            <h3>Quick Links</h3>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Properties</a></li>
                <li><a href="#">Gallery</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </div>
    </div>
    <div class="footer-bottom">
        <p>&copy; 2025 Real Estate. All rights reserved.</p>
    </div>
</footer>
</body>
</html>
