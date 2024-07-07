<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Unique Webpage</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav class="navbar">
            <div class="container">
                <a href="#" class="logo">My Webpage</a>
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
        </nav>
    </header>
    <section id="home" class="hero">
        <div class="container">
            <h1>Welcome to My Unique Webpage</h1>
            <p>Your solution for product management</p>
            <a href="#features" class="btn">Learn More</a>
        </div>
    </section>
    <section id="features" class="features">
        <div class="container">
            <h2>Features</h2>
            <div class="feature-item">
                <h3>Feature 1</h3>
                <p>Description of feature 1.</p>
            </div>
            <div class="feature-item">
                <h3>Feature 2</h3>
                <p>Description of feature 2.</p>
            </div>
            <div class="feature-item">
                <h3>Feature 3</h3>
                <p>Description of feature 3.</p>
            </div>
        </div>
    </section>
    <section id="testimonials" class="testimonials">
        <div class="container">
            <h2>Testimonials</h2>
            <div class="testimonial-item">
                <p>"This is the best product ever!"</p>
                <h4>- Happy Customer</h4>
            </div>
            <div class="testimonial-item">
                <p>"I can't imagine my life without it."</p>
                <h4>- Satisfied User</h4>
            </div>
        </div>
    </section>
    <footer id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Email: info@mywebpage.com</p>
            <p>Phone: +123 456 7890</p>
            <p>&copy; 2024 My Unique Webpage. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>




import Link from 'next/link';

const Header = () => (
  <header>
    <nav className="bg-gray-800 p-4">
      <div className="container mx-auto flex justify-between items-center">
        <Link href="/">
          <a className="text-white text-2xl font-bold">My Webpage</a>
        </Link>
        <ul className="flex space-x-4">
          <li><Link href="#home"><a className="text-white">Home</a></Link></li>
          <li><Link href="#features"><a className="text-white">Features</a></Link></li>
          <li><Link href="#testimonials"><a className="text-white">Testimonials</a></Link></li>
          <li><Link href="#contact"><a className="text-white">Contact</a></Link></li>
        </ul>
      </div>
    </nav>
  </header>
);

export default Header;




// components/Hero.js

const Hero = () => (
  <section id="home" className="flex flex-col justify-center items-center text-white" style={{ background: "url('hero-background.jpg') no-repeat center center/cover", height: "100vh" }}>
    <div className="text-center">
      <h1 className="text-5xl font-bold">Welcome to My Unique Webpage</h1>
      <p className="text-xl mt-4">Your solution for product management</p>
      <a href="#features" className="mt-8 inline-block bg-green-500 text-white py-2 px-4 rounded">Learn More</a>
    </div>
  </section>
);

export default Hero;




// components/Features.js

const Features = () => (
  <section id="features" className="py-16">
    <div className="container mx-auto text-center">
      <h2 className="text-3xl font-bold mb-8">Features</h2>
      <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div>
          <h3 className="text-xl font-semibold">Feature 1</h3>
          <p className="mt-2">Description of feature 1.</p>
        </div>
        <div>
          <h3 className="text-xl font-semibold">Feature 2</h3>
          <p className="mt-2">Description of feature 2.</p>
        </div>
        <div>
          <h3 className="text-xl font-semibold">Feature 3</h3>
          <p className="mt-2">Description of feature 3.</p>
        </div>
      </div>
    </div>
  </section>
);

export default Features;




// components/Testimonials.js

const Testimonials = () => (
  <section id="testimonials" className="py-16 bg-gray-100">
    <div className="container mx-auto text-center">
      <h2 className="text-3xl font-bold mb-8">Testimonials</h2>
      <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div>
          <p className="italic">"This is the best product ever!"</p>
          <h4 className="mt-4">- Happy Customer</h4>
        </div>
        <div>
          <p className="italic">"I can't imagine my life without it."</p>
          <h4 className="mt-4">- Satisfied User</h4>
        </div>
      </div>
    </div>
  </section>
);

export default Testimonials;




// components/Footer.js

const Footer = () => (
  <footer id="contact" className="py-8 bg-gray-800 text-white text-center">
    <div className="container mx-auto">
      <h2 className="text-2xl mb-4">Contact Us</h2>
      <p>Email: info@mywebpage.com</p>
      <p>Phone: +123 456 7890</p>
      <p>&copy; 2024 My Unique Webpage. All rights reserved.</p>
    </div>
  </footer>
);

export default Footer;
