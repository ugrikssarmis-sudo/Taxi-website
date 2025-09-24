<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>City Taxi Service</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Reset and basic styles */
        * {margin: 0; padding: 0; box-sizing: border-box;}
        body {font-family: 'Roboto', sans-serif; line-height: 1.6; color: #333;}
        a {text-decoration: none; color: inherit;}
        header {background: #ffcc00; padding: 20px 0;}
        header nav {display: flex; justify-content: space-between; align-items: center; width: 90%; margin: 0 auto;}
        header nav ul {display: flex; list-style: none;}
        header nav ul li {margin-left: 20px;}
        header nav ul li a {font-weight: bold;}
        
        /* Hero Section */
        .hero {background: url('https://images.unsplash.com/photo-1563729784474-7c4d9f49b6f3') no-repeat center center/cover; height: 90vh; display: flex; justify-content: center; align-items: center; color: white; text-align: center;}
        .hero h1 {font-size: 3rem; margin-bottom: 20px;}
        .hero p {font-size: 1.2rem; margin-bottom: 30px;}
        .hero button {padding: 15px 30px; background: #ff6600; border: none; color: white; font-size: 1rem; cursor: pointer; border-radius: 5px;}

        /* Sections */
        section {padding: 80px 0; width: 90%; margin: 0 auto;}
        h2 {text-align: center; margin-bottom: 50px; color: #ff6600;}

        /* Services */
        .services {display: flex; justify-content: space-around; flex-wrap: wrap;}
        .service {background: #f4f4f4; padding: 30px; border-radius: 10px; width: 30%; margin-bottom: 20px; text-align: center;}
        .service h3 {margin-bottom: 15px;}

        /* Booking Form */
        form {max-width: 600px; margin: 0 auto; display: flex; flex-direction: column;}
        form input, form select, form textarea {padding: 15px; margin-bottom: 20px; border: 1px solid #ccc; border-radius: 5px;}
        form button {padding: 15px; background: #ff6600; border: none; color: white; cursor: pointer; border-radius: 5px; font-size: 1rem;}

        /* Footer */
        footer {background: #333; color: white; text-align: center; padding: 20px 0; margin-top: 40px;}

        /* Responsive */
        @media(max-width: 768px){
            .services {flex-direction: column; align-items: center;}
            .service {width: 80%;}
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <div class="logo"><h2>City Taxi</h2></div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#booking">Booking</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div>
            <h1>Reliable Taxi Service</h1>
            <p>Fast, safe, and comfortable rides anytime, anywhere.</p>
            <button onclick="document.getElementById('booking').scrollIntoView({ behavior: 'smooth' })">Book Now</button>
        </div>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p style="text-align:center; max-width:700px; margin:0 auto;">
            City Taxi has been providing top-notch transportation services for over 10 years. Our fleet is modern, our drivers are experienced, and customer satisfaction is our top priority.
        </p>
    </section>

    <section id="services">
        <h2>Our Services</h2>
        <div class="services">
            <div class="service">
                <h3>Airport Transfers</h3>
                <p>Fast and reliable airport pickup and drop-off services.</p>
            </div>
            <div class="service">
                <h3>City Rides</h3>
                <p>Comfortable rides around the city at affordable prices.</p>
            </div>
            <div class="service">
                <h3>Outstation Trips</h3>
                <p>Plan your outstation trips with our safe and spacious vehicles.</p>
            </div>
        </div>
    </section>

    <section id="booking">
        <h2>Book a Ride</h2>
        <form>
            <input type="text" placeholder="Full Name" required>
            <input type="email" placeholder="Email" required>
            <input type="tel" placeholder="Phone Number" required>
            <input type="text" placeholder="Pickup Location" required>
            <input type="text" placeholder="Drop Location" required>
            <select required>
                <option value="">Select Vehicle Type</option>
                <option value="sedan">Sedan</option>
                <option value="suv">SUV</option>
                <option value="van">Van</option>
            </select>
            <button type="submit">Book Now</button>
        </form>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p style="text-align:center;">Email: support@citytaxi.com | Phone: +123-456-7890</p>
        <p style="text-align:center;">Address: 123 Main Street, Your City</p>
    </section>

    <footer>
        &copy; 2025 City Taxi. All rights reserved.
    </footer>

</body>
</html>
