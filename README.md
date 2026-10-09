=========================================
  ABUJA INSTANT MEAL
  Nigerian Restaurant Website
=========================================

A modern, responsive single-page website for a Nigerian restaurant 
specializing in local dishes like Suya, Jollof Rice, Pounded Yam, 
and more. Built with HTML, CSS, and PHP.

-----------------------------------------
  PROJECT OVERVIEW
-----------------------------------------

This project contains two versions of the website:

1. index.html  - Static HTML version (hardcoded menu items with 
                 external image URLs from Pexels).

2. index.php   - Dynamic PHP version (menu items stored in a PHP 
                 array, using local images from the /image folder, 
                 and includes basic form handling).

Both versions use the same stylesheet (style.css).

-----------------------------------------
  FILE STRUCTURE
-----------------------------------------

/ (root)
│
├── index.html          # Static HTML version
├── index.php           # Dynamic PHP version (recommended)
├── style.css           # Main stylesheet for both versions
├── README.txt          # This file
│
└── image/              # Local images for the PHP version
    ├── suya.jpeg
    ├── jollof.jpg
    ├── pounded-yam.jpg
    ├── pepperedsnail.jfif
    ├── moi.jfif
    └── ofada.jfif

-----------------------------------------
  FEATURES
-----------------------------------------

- Fully responsive design (mobile, tablet, desktop)
- Fixed navigation bar with blur backdrop effect
- Animated hero section with floating spice particles
- Dynamic menu grid (PHP loop or static HTML)
- About section with stats
- Contact/Reservation form with PHP POST handling
- Smooth hover animations and transitions
- Font Awesome icons & Google Fonts (Playfair Display + Poppins)
- Nigerian-themed color palette (smoky red-orange, warm yam, 
  pepper green)

-----------------------------------------
  TECHNOLOGIES USED
-----------------------------------------

- HTML5
- CSS3 (Flexbox, Grid, CSS Variables, Animations)
- PHP (for dynamic content & form processing)
- Font Awesome 6 (CDN)
- Google Fonts (CDN)
- Pexels (image hosting for HTML version)

-----------------------------------------
  SETUP & INSTALLATION
-----------------------------------------

REQUIREMENTS:
- A web server with PHP support (Apache, Nginx, XAMPP, WAMP, 
  MAMP, or Laragon).
- A modern web browser.

STEPS:

1. STATIC VERSION (index.html):
   - Simply open index.html in any web browser.
   - No server required.
   - Note: Images are loaded from Pexels CDN, so an internet 
     connection is needed to see them.

2. DYNAMIC VERSION (index.php):
   - Place the entire project folder in your web server's root 
     directory (e.g., htdocs for XAMPP, www for WAMP).
   - Ensure the /image folder contains all required images with 
     the exact filenames listed above.
   - Start your local server (Apache).
   - Open your browser and navigate to:
     http://localhost/your-folder-name/index.php

-----------------------------------------
  CUSTOMIZATION GUIDE
-----------------------------------------

1. CHANGING MENU ITEMS (PHP Version):
   - Open index.php.
   - Locate the $dishes array (around line 80).
   - Edit the 'name', 'desc', 'price', and 'img' values.
   - Add or remove array entries as needed.

2. CHANGING COLORS:
   - Open style.css.
   - Edit the CSS variables in the :root section:
     --primary        (main brand color)
     --primary-light  (hover states)
     --secondary      (accents)
     --accent         (green highlights)
     --dark           (text color)
     --light          (background)

3. CHANGING LOGO NAME:
   - In index.php or index.html, find the .logo div.
   - Replace "Abuja<em>Suya</em>" or "Instant<em>Meal</em>" 
     with your desired name.

4. CONTACT INFORMATION:
   - Edit the .contact-info section in both files.
   - Update address, phone, email, and hours.

5. FORM HANDLING:
   - The PHP version processes the form on the same page.
   - To send emails, replace the echo statement with mail() 
     function or integrate a library like PHPMailer.
   - To store submissions in a database, add MySQL connection 
     code in the PHP block.

-----------------------------------------
  IMPORTANT NOTES
-----------------------------------------

- The HTML version uses external Pexels image URLs. If you 
  want to use local images in the HTML version, replace the 
  src attributes with paths like ./image/suya.jpeg.

- The PHP version requires the /image folder to exist with 
  all referenced image files. Missing images will show as 
  empty cards.

- The order buttons ("Add to order") are currently non-
  functional. You will need to add JavaScript or backend 
  logic to implement a shopping cart or ordering system.

- The form in index.php uses basic validation (name & email 
  required). For production, add CSRF protection, sanitize 
  inputs, and use a proper mail/database solution.

- The footer year in index.html says "2025" while index.php 
  says "2026". Update as needed.

-----------------------------------------
  BROWSER SUPPORT
-----------------------------------------

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

Note: backdrop-filter may not work in older browsers.

-----------------------------------------
  LICENSE
-----------------------------------------

This project is open-source and available for personal and 
commercial use. Feel free to modify and distribute.

-----------------------------------------
  CREDITS
-----------------------------------------

- Design & Development: [Your Name]
- Fonts: Google Fonts (Playfair Display, Poppins)
- Icons: Font Awesome 6
- Images: Pexels (HTML version) & Local (PHP version)

-----------------------------------------
  CONTACT
-----------------------------------------

For questions or support, contact:
Email: gregzirra2005@gmail.com
Phone: +234 915 4343 417

=========================================
  Made with ❤️ in Nigeria
=========================================
