# Axjav
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Axjav - Support Creators</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <!-- HEADER -->
    <header>
        <div class="logo">Axjav</div>
        <nav>
            <a href="#features">Features</a>
            <a href="#pricing">Pricing</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <!-- HERO SECTION -->
    <section class="hero">
        <h1>Empower Your Creativity</h1>
        <p>Join Axjav — a platform where creators connect with supporters and bring ideas to life.</p>
        <a href="#pricing" class="btn-primary">Get Started</a>
    </section>

    <!-- FEATURES -->
    <section id="features" class="features">
        <h2>Why Choose Axjav?</h2>
        <div class="feature-grid">
            <div class="feature">
                <h3>Direct Support</h3>
                <p>Receive contributions from fans and patrons directly.</p>
            </div>
            <div class="feature">
                <h3>Flexible Plans</h3>
                <p>Offer different membership levels with unique perks.</p>
            </div>
            <div class="feature">
                <h3>Creator Friendly</h3>
                <p>Keep more of what you earn with low fees.</p>
            </div>
        </div>
    </section>

    <!-- PRICING -->
    <section id="pricing" class="pricing">
        <h2>Pricing</h2>
        <div class="pricing-grid">
            <div class="plan">
                <h3>Starter</h3>
                <p>$5/month</p>
                <ul>
                    <li>Basic creator tools</li>
                    <li>Direct messaging</li>
                </ul>
                <a href="#" class="btn-secondary">Select</a>
            </div>
            <div class="plan">
                <h3>Pro</h3>
                <p>$15/month</p>
                <ul>
                    <li>Advanced analytics</li>
                    <li>Priority support</li>
                </ul>
                <a href="#" class="btn-secondary">Select</a>
            </div>
        </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Email: support@axjav.com</p>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>© 2025 Axjav. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: #f9f9f9;
    color: #333;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background: #111;
    color: white;
}

header .logo {
    font-size: 1.5rem;
    font-weight: bold;
}

header nav a {
    color: white;
    text-decoration: none;
    margin-left: 1.5rem;
}

.hero {
    text-align: center;
    padding: 4rem 2rem;
    background: linear-gradient(to right, #ff6a00, #ee0979);
    color: white;
}

.hero h1 {
    font-size: 2.5rem;
}

.btn-primary {
    display: inline-block;
    padding: 0.8rem 1.5rem;
    background: white;
    color: #ff6a00;
    text-decoration: none;
    font-weight: bold;
    border-radius: 4px;
}

.features, .pricing, .contact {
    padding: 3rem 2rem;
    text-align: center;
}

.feature-grid, .pricing-grid {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
}

.feature, .plan {
    background: white;
    padding: 1.5rem;
    border-radius: 8px;
    width: 250px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.btn-secondary {
    display: inline-block;
    padding: 0.6rem 1.2rem;
    background: #ff6a00;
    color: white;
    text-decoration: none;
    border-radius: 4px;
}

footer {
    background: #111;
    color: white;
    text-align: center;
    padding: 1rem;
}

// Smooth scroll for nav links
document.querySelectorAll('nav a').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            window.scrollTo({
                top: target.offsetTop - 60,
                behavior: 'smooth'
            });
        }
    });
});
