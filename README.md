<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real Estate</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <nav class="navbar">
        <a href="#" class="nav-logo">
            <h2 class="logo-text">Real Estate</h2>
        </a>
        <ul class="nav-menu">
            <li class="nav-item"><a href="index.html" class="nav-link">Home</a></li>
            <li class="nav-item"><a href="Aboutus.html" class="nav-link">About Us</a></li>
            <li class="nav-item"><a href="buy.html" class="nav-link">Buy/Rent</a></li>
            <li class="nav-item"><a href="Contact.html" class="nav-link">Contact Us</a></li>
            <li><button class="btnlogin-popup"id="loginBtn">Login</button></li>            
        </ul>
    </nav>
</header>

<main>
    <section class="hero-section">
        <div class="section-content">
            <div class="hero-details">
                <h2 class="title">Find Your Dream Home</h2>
                <section class="center">
                    <form action="buy.html" method="get">
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
                                    <option value="Jhapa">Jhapa</option>
                                    <option value="Mustang">Mustang</option>
                                    <option value="Pokhara">Pokhara</option>
                                    <option value="Bharatpur">Bharatpur</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Minimum Budget <span>*</span></p>
                                <select name="budget" class="input" required>
                                    <option value="200000-500000">20K-50K</option>
                                    <option value="1000000-2000000">1Lakh-2Lakh</option>
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
    

<div id="loginModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    <form class="login-form">
      <h2>Login</h2>
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" name="password" required>
       </div>      
        <div class="show-password">  
        <input type="checkbox" id="showPassword">
        <label for="showPassword">Show Password</label>
      </div>
      <button type="submit" class="btn-login">Login</button>
      <p class="extra-linl">Don’t have an account? <a href="#">Register</a></p>
    </form>
  </div>
</div>

<!-- Properties Section -->
<section class="properties" id="properties">
    <div class="title-box">
        <h2 class="section-title">LATEST LISTING</h2>
    </div>

    <div class="property-grid">
        <div class="property-card" data-name="home1">
            <img src="home1.jpg" alt="Jhapa Home">
            <h3>RS 3,00,00,000</h3>
            <p>Jhapa</p>
            <p>House</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card" data-name="home2">
            <img src="home2.jpg" alt="Bharatpur Home">
            <h3>RS 4,00,00,000</h3>
            <p>Bharatpur</p>
            <p>House</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card" data-name="home3">
            <img src="home3.jpg" alt="Mustang Home">
            <h3>RS  2,00,00,000</h3>
            <p>Mustang</p>
            <p>House</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card hidden" data-name="home4">
            <img src="home4.jpg" alt="Kathmandu Home">
            <h3>RS 1,50,00,000 </h3>
            <p>Kathmandu</p>
            <p>Land</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card hidden" data-name="home5">
            <img src="home5.jpg" alt="Pokhara Home">
            <h3>RS 80,00,000 </h3>
            <p>Pokhara</p>
            <p>Land</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card hidden" data-name="home6">
            <img src="home6.webp" alt="Lalitpur Home">
            <h3>RS 60000</h3>
            <p>Lalitpur</p>
            <p>Flat</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card hidden" data-name="home7">
            <img src="home7.jpeg" alt="Mustang Home">
            <h3>RS  50,000</h3>
            <p>Mustang</p>
            <p>Flat</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
    </div>

    <div class="view-all-container">
        <button id="viewAllBtn">View All</button>
    </div>
</section>
</main>

<script>
document.getElementById("viewAllBtn").addEventListener("click", function() {
const hiddenCards = document.querySelectorAll(".property-card.hidden");
hiddenCards.forEach(card => card.classList.remove("hidden"));
this.style.display = "none";
});

// JavaScript to handle enlarge and blur effects
document.querySelectorAll('.property-card').forEach(card => {
card.addEventListener('click', function() {
    // Check if the clicked card is already enlarged
    if (this.classList.contains('enlarged')) {
        // If it's enlarged, reset all cards to normal
        document.querySelectorAll('.property-card').forEach(c => {
            c.classList.remove('enlarged');
            c.classList.remove('blurred');
        });
    } else {
        // Otherwise, enlarge the clicked card and blur others
        document.querySelectorAll('.property-card').forEach(c => {
            c.classList.add('blurred'); // Blur all cards
        });
        this.classList.remove('blurred'); // Remove blur from the clicked card
        this.classList.add('enlarged'); // Enlarge the clicked card
    }
});
});
</script>



<script>
  const modal = document.getElementById("loginModal");
  const loginBtn = document.getElementById("loginBtn");
  const closeBtn = document.querySelector(".close");
  const loginForm = document.querySelector(".login-form");
  const passwordInput = document.getElementById("password");
  const showPasswordCheckbox = document.getElementById("showPassword");
  
  showPasswordCheckbox.addEventListener("change", function(){
  if(this.checked){
   passwordInput.type="text";
  }
  else{
   passwordInput.type="password";
  }
});   
  
  loginForm.addEventListener("submit", function(event){
   event.preventDefault();

   const email = document.getElementById("email").value;
   const password = document.getElementById("password").value;
    
   console.log("Email:", email);
   console.log("Password:", password);

   modal.classList.remove("active");
});

  loginBtn.addEventListener("click", function(event) {
    event.preventDefault(); // Prevent link navigation if it's an <a>
    modal.classList.add("active"); 
  });

  closeBtn.addEventListener("click", function() {
    modal.classList.remove("active");
  });

 
  window.addEventListener("click", function(event) {
    if (event.target === modal) {
      modal.classList.remove("active");
    }
  });
</script>
<script>
    document.getElementById("viewAllBtn").addEventListener("click", function() {
        const hiddenCards = document.querySelectorAll(".property-card.hidden");
        hiddenCards.forEach(card => card.classList.remove("hidden"));
        this.style.display = "none"; // Hide the button after clicking
    });
    </script>
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
                <li><a href="index.html">Home</a></li>
                <li><a href="aboutus.html">About</a></li>
                <li><a href="#">Buy/sell</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </div>
    </div>
    <div class="footer-bottom">
        <p>&copy; 2025 Real Estate. All rights reserved.</p>
    </div>
</footer>
</main>
</body>
</html>
