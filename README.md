<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SwiftNet - Landing Page</title>
  <style>
    /* === BASE RESET === */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      line-height: 1.6;
      background: #f4f4f4;
    }

    a {
      text-decoration: none;
      color: white;
    }

    button {
      cursor: pointer;
    }

    /* === NAVBAR === */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background-color: #24292e;
      color: white;
      flex-wrap: wrap;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav-links {
      display: flex;
      gap: 1rem;
    }

    .nav-links a {
      color: white;
      font-weight: 500;
    }

    /* === HERO SECTION === */
    .hero {
      background: linear-gradient(135deg, #0077cc, #66ccff);
      color: white;
      padding: 4rem 2rem;
      text-align: center;
      animation: fadeIn 2s ease-in-out;
    }

    .hero h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.2rem;
      max-width: 700px;
      margin: 0 auto 2rem;
    }

    .hero button {
      padding: 0.8rem 1.5rem;
      font-size: 1rem;
      background: white;
      color: #0077cc;
      border: none;
      border-radius: 5px;
      transition: transform 0.3s, background 0.3s;
    }

    .hero button:hover {
      background: #e0f0ff;
      transform: scale(1.1);
    }

    /* === FEATURE SECTION === */
    .features {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 2rem;
      gap: 1.5rem;
      background-color: #ffffff;
    }

    .card {
      background: #fefefe;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      border-radius: 8px;
      width: 300px;
      padding: 1.5rem;
      text-align: center;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card:hover {
      transform: scale(1.05);
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
    }

    .card h3 {
      margin-bottom: 1rem;
      color: #333;
    }

    .card p {
      margin-bottom: 1.5rem;
      color: #666;
    }

    .card button {
      background: #0077cc;
      color: white;
      border: none;
      padding: 0.6rem 1.2rem;
      border-radius: 4px;
      transition: background 0.3s ease;
    }

    .card button:hover {
      background: #005fa3;
    }

    /* === FOOTER === */
    .footer {
      background: #24292e;
      color: white;
      text-align: center;
      padding: 1.5rem;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    /* === ANIMATIONS === */
    @keyframes fadeIn {
      0% {
        opacity: 0;
        transform: translateY(-20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes slideIn {
      0% {
        transform: translateX(-100%);
        opacity: 0;
      }
      100% {
        transform: translateX(0);
        opacity: 1;
      }
    }

    .card:nth-child(2) {
      animation: slideIn 1s ease forwards;
    }

    /* === RESPONSIVE === */
    @media (max-width: 768px) {
      .nav-links {
        width: 100%;
        justify-content: center;
        margin-top: 1rem;
      }

      .navbar {
        flex-direction: column;
        align-items: flex-start;
      }

      .hero h1 {
        font-size: 2.2rem;
      }

      .features {
        padding: 1rem;
      }
    }

    @media (max-width: 480px) {
      .card {
        width: 100%;
      }

      .hero {
        padding: 2rem 1rem;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="navbar">
    <div class="logo">SwiftNet</div>
    <div class="nav-links">
      <a href="#">Home</a>
      <a href="#">Services</a>
      <a href="#">About</a>
      <a href="#">Pricing</a>
      <a href="#">Contact</a>
    </div>
  </nav>

  <!-- HERO SECTION -->
  <section class="hero">
    <h1>Welcome to SwiftNet</h1>
    <p>Connecting the world with blazing fast internet and reliable digital solutions for businesses and homes.</p>
    <button>Get Started</button>
  </section>

  <!-- FEATURES -->
  <section class="features">
    <div class="card">
      <h3>High-Speed Internet</h3>
      <p>Experience lightning-fast internet speeds at your home or office.</p>
      <button>More Details</button>
    </div>
    <div class="card">
      <h3>24/7 Support</h3>
      <p>Our dedicated team is always ready to help you anytime, anywhere.</p>
      <button>More Details</button>
    </div>
    <div class="card">
      <h3>Business Solutions</h3>
      <p>Custom packages and tools to power your business online.</p>
      <button>More Details</button>
    </div>
    <div class="card">
      <h3>Secure Network</h3>
      <p>We ensure your data and network stay secure at all times.</p>
      <button>More Details</button>
    </div>
    <div class="card">
      <h3>Flexible Plans</h3>
      <p>Choose from affordable and flexible pricing to suit your needs.</p>
      <button>More Details</button>
    </div>
    <div class="card">
      <h3>Fast Installation</h3>
      <p>Quick and easy setup so you can get online faster.</p>
      <button>More Details</button>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <p>&copy; 2025 SwiftNet. All rights reserved.</p>
  </footer>

</body>
</html>
