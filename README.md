<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pinnacle Wealth Solution Ltd</title>

<!-- Google Analytics (Replace G-XXXXXXX) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXX"></script>
<script>
window.dataLayer = window.dataLayer || [];
function gtag(){dataLayer.push(arguments);}
gtag('js', new Date());
gtag('config', 'G-XXXXXXX');
</script>

<style>
body {font-family: Arial; margin:0; background:#f9fafb;}
header {background:#0b3d91; color:white; padding:15px; display:flex; justify-content:space-between; align-items:center;}
nav a {color:white; margin:0 10px; text-decoration:none;}
section {padding:60px 20px; text-align:center;}
.hero {background:linear-gradient(to right,#0b3d91,#f4b400); color:white;}
.btn {background:white; color:#0b3d91; padding:12px 25px; border-radius:25px; text-decoration:none; font-weight:bold; display:inline-block; margin:5px;}
.services {display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:15px;}
.services div {background:white; padding:20px; border-radius:12px; box-shadow:0 2px 10px rgba(0,0,0,0.1);}
form {max-width:400px; margin:auto; display:grid; gap:10px;}
input, textarea {padding:10px; border-radius:8px; border:1px solid #ccc;}
footer {background:#0b3d91; color:white; padding:15px;}
.whatsapp {position:fixed; bottom:20px; right:20px; background:#25D366; color:white; padding:15px; border-radius:50%; text-decoration:none;}
</style>
</head>

<body>

<header>
<h2>Pinnacle Wealth Solution Ltd</h2>
<nav>
<a href="#">Home</a>
<a href="#about">About</a>
<a href="#services">Services</a>
<a href="#agreement">Agreement</a>
<a href="#booking">Booking</a>
<a href="#contact">Contact</a>
</nav>
</header>

<section class="hero">
<h1>Travel Smarter With Confidence</h1>
<p>Visa, Travel & Financial Services You Can Trust</p>
<br>
<a class="btn" href="#contact">Get Started</a>
</section>

<section id="about">
<h2>About Pinnacle Wealth Solution Limited</h2>
<p>
Pinnacle Wealth Solution Limited is a professional travel and financial consultancy company based in Abuja, Nigeria.
We specialize in visa assistance, international travel planning, and financial advisory services.
Our mission is to provide reliable, transparent, and efficient solutions to individuals and corporate clients.
</p>
</section>

<section id="services">
<h2>Our Services</h2>
<div class="services">
<div>Visa Assistance</div>
<div>Flight Booking</div>
<div>Hotel Reservation</div>
<div>Travel Consultancy</div>
<div>Financial Advisory</div>
<div>Corporate Travel</div>
</div>
</section>

<section id="agreement">
<h2>Client Agreement</h2>
<p>Download and sign before service</p>
<a class="btn" href="agreement.pdf" download>Download Agreement</a>
</section>

<section id="booking">
<h2>Book a Service</h2>
<form action="https://formspree.io/f/YOUR-ID" method="POST">
<input type="text" name="name" placeholder="Full Name" required>
<input type="email" name="email" placeholder="Email" required>
<input type="tel" name="phone" placeholder="Phone Number" required>
<textarea name="message" placeholder="Service Needed"></textarea>
<button class="btn">Submit Booking</button>
</form>
</section>

<section id="payment">
<h2>Make Payment</h2>
<p>Pay securely online</p>
<button class="btn" onclick="payWithPaystack()">Pay Now</button>
</section>

<section id="testimonials">
<h2>What Our Clients Say</h2>
<div class="services">
<div>
⭐️⭐️⭐️⭐️⭐️<br>
"Excellent service! Got my visa without stress."<br><b>- Chinedu A.</b>
</div>
<div>
⭐️⭐️⭐️⭐️⭐️<br>
"Very reliable and fast processing."<br><b>- Aisha M.</b>
</div>
<div>
⭐️⭐️⭐️⭐️⭐️<br>
"Highly recommended travel agency."<br><b>- Musa K.</b>
</div>
</div>
</section>

<section id="contact">
<h2>Contact Us</h2>
<p>📍 Abuja, Nigeria</p>
<p>📞 +2348060325830</p>
<p>✉️ preciousgreat2019@gmail.com</p>
</section>

<a href="https://wa.me/2348060325830" class="whatsapp">💬</a>

<footer>
<p>© 2026 Pinnacle Wealth Solution Ltd</p>
</footer>

<!-- Paystack -->
<script src="https://js.paystack.co/v1/inline.js"></script>
<script>
function payWithPaystack(){
  let handler = PaystackPop.setup({
    key: 'YOUR_PUBLIC_KEY',
    email: 'customer@email.com',
    amount: 5000000,
    currency: 'NGN',
    callback: function(response){
      alert('Payment successful. Ref: ' + response.reference);
    },
  });
  handler.openIframe();
}
</script>

</body>
</html>
