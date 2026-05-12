# Ex02 Commercial Website
## Date: 12/04/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
## index.html:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resale Wheel | Resale Vehicle Marketplace</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="site-header">
        <div class="brand">
            <span class="brand-mark">RW</span>
            <span>Resale Wheel</span>
        </div>

        <nav class="nav-links" aria-label="Main navigation">
            <a href="#vehicles">Vehicles</a>
            <a href="#process">How It Works</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="hero-copy">
                <p class="eyebrow">Verified pre-owned vehicles</p>
                <h1>Buy and sell resale vehicles with confidence.</h1>
                <p class="hero-text">
                    Resale Wheel is a commercial resale vehicle website for inspected cars, bikes,
                    and SUVs with fair pricing, finance guidance, and quick documentation support.
                </p>
                <div class="hero-actions">
                    <a class="btn primary" href="#vehicles">View Vehicles</a>
                    <a class="btn secondary" href="#contact">Sell Your Vehicle</a>
                </div>
            </div>

            <div class="hero-panel" aria-label="Featured vehicle">
                <img src="https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?auto=format&fit=crop&w=900&q=80" alt="Black resale sports car">
                <div class="price-strip">
                    <span>Featured Deal</span>
                    <strong>From Rs. 5.8L</strong>
                </div>
            </div>
        </section>

        <section class="search-strip" aria-label="Vehicle search options">
            <label>
                Vehicle type
                <select>
                    <option>All vehicles</option>
                    <option>Cars</option>
                    <option>SUVs</option>
                    <option>Bikes</option>
                </select>
            </label>
            <label>
                Budget
                <select>
                    <option>Any budget</option>
                    <option>Below Rs. 2L</option>
                    <option>Rs. 2L - Rs. 8L</option>
                    <option>Above Rs. 8L</option>
                </select>
            </label>
            <label>
                Fuel
                <select>
                    <option>All fuel types</option>
                    <option>Petrol</option>
                    <option>Diesel</option>
                    <option>Electric</option>
                </select>
            </label>
            <a class="btn primary" href="#vehicles">Search Stock</a>
        </section>

        <section class="trust-row" aria-label="Business highlights">
            <div>
                <strong>120+</strong>
                <span>Vehicles listed</span>
            </div>
            <div>
                <strong>48 hr</strong>
                <span>Ownership transfer</span>
            </div>
            <div>
                <strong>100%</strong>
                <span>Inspection reports</span>
            </div>
        </section>

        <section class="section" id="vehicles">
            <div class="section-heading">
                <p class="eyebrow">Available stock</p>
                <h2>Popular resale vehicles</h2>
                <p>Each listing is arranged with Flexbox so vehicle cards stay balanced on desktop and wrap naturally on tablets and phones.</p>
            </div>

            <div class="vehicle-list">
                <article class="vehicle-card">
                    <img src="https://images.unsplash.com/photo-1549399542-7e3f8b79c341?auto=format&fit=crop&w=700&q=80" alt="White compact car">
                    <div class="vehicle-content">
                        <h3>Honda City VX</h3>
                        <p>Petrol, 42,000 km, single owner, service history available.</p>
                        <div class="card-bottom">
                            <strong>Rs. 7.45L</strong>
                            <a href="#contact">Enquire</a>
                        </div>
                    </div>
                </article>

                <article class="vehicle-card">
                    <img src="https://images.unsplash.com/photo-1605559424843-9e4c228bf1c2?auto=format&fit=crop&w=700&q=80" alt="Red resale SUV">
                    <div class="vehicle-content">
                        <h3>Hyundai Creta SX</h3>
                        <p>Diesel, 58,000 km, new tyres, insurance valid.</p>
                        <div class="card-bottom">
                            <strong>Rs. 10.9L</strong>
                            <a href="#contact">Enquire</a>
                        </div>
                    </div>
                </article>

                <article class="vehicle-card">
                    <img src="https://images.unsplash.com/photo-1558981806-ec527fa84c39?auto=format&fit=crop&w=700&q=80" alt="Resale motorcycle">
                    <div class="vehicle-content">
                        <h3>Royal Enfield Classic</h3>
                        <p>350cc, 18,500 km, showroom maintained, ready delivery.</p>
                        <div class="card-bottom">
                            <strong>Rs. 1.65L</strong>
                            <a href="#contact">Enquire</a>
                        </div>
                    </div>
                </article>

                <article class="vehicle-card">
                    <img src="https://images.unsplash.com/photo-1593941707882-a5bba14938c7?auto=format&fit=crop&w=700&q=80" alt="Blue electric resale car">
                    <div class="vehicle-content">
                        <h3>Tata Nexon EV</h3>
                        <p>Electric, 24,000 km, company warranty, fast charger included.</p>
                        <div class="card-bottom">
                            <strong>Rs. 9.8L</strong>
                            <a href="#contact">Enquire</a>
                        </div>
                    </div>
                </article>
            </div>
        </section>

        <section class="section process-section" id="process">
            <div class="section-heading">
                <p class="eyebrow">Simple process</p>
                <h2>How Resale Wheel works</h2>
            </div>

            <div class="process-list">
                <div class="process-step">
                    <span>1</span>
                    <h3>Choose</h3>
                    <p>Browse verified vehicle listings with photos, mileage, fuel type, and price.</p>
                </div>
                <div class="process-step">
                    <span>2</span>
                    <h3>Inspect</h3>
                    <p>Book a test drive and check inspection details before making a decision.</p>
                </div>
                <div class="process-step">
                    <span>3</span>
                    <h3>Purchase</h3>
                    <p>Complete payment, finance, insurance, and transfer support in one place.</p>
                </div>
            </div>
        </section>

        <section class="section info-section" id="about">
            <div class="info-copy">
                <p class="eyebrow">Working principle</p>
                <h2>Flexbox layout explanation</h2>
                <p>
                    This website uses CSS Flexbox to arrange items in rows on large screens and stack
                    them neatly on smaller screens. The header uses Flexbox to place the logo and
                    navigation side by side. The search strip, trust boxes, product cards, process
                    steps, information block, and footer also use <strong>display: flex</strong>.
                    Product cards use <strong>display: flex</strong> with
                    <strong>flex-wrap</strong>, so cards move to the next line when screen width is limited.
                </p>
                <p>
                    Flex properties such as <strong>justify-content</strong>, <strong>align-items</strong>,
                    <strong>gap</strong>, and <strong>flex-basis</strong> control alignment, spacing, and
                    minimum card size. Media queries adjust direction, spacing, and card width for mobile devices. This
                    keeps the navigation, vehicle section, process boxes, and footer readable without
                    horizontal scrolling.
                </p>
            </div>
            <aside class="contact-box" id="contact">
                <h2>Contact Resale Wheel</h2>
                <p>Call: +91 98765 43210</p>
                <p>Email: sales@resalewheel.example</p>
                <a class="btn primary" href="mailto:sales@resalewheel.example">Send Enquiry</a>
            </aside>
        </section>
    </main>

    <footer class="site-footer">
        <div>
            <strong>Resale Wheel</strong>
            <p>Trusted marketplace for pre-owned cars, bikes, and SUVs.</p>
        </div>
        <p>&copy; 2026 Resale Wheel. All rights reserved.</p>
    </footer>
</body>
</html>

```
## style.css
```
:root {
    --ink: #17212b;
    --muted: #66717f;
    --paper: #f6f4ef;
    --surface: #ffffff;
    --soft: #edf7f4;
    --line: #dcd8cf;
    --accent: #0f766e;
    --accent-dark: #0b504b;
    --gold: #d99a2b;
}

* {
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
    color: var(--ink);
    background: var(--paper);
    line-height: 1.6;
}

img {
    display: block;
    max-width: 100%;
}

a {
    color: inherit;
}

.site-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 24px;
    padding: 18px 7%;
    background: var(--surface);
    border-bottom: 1px solid var(--line);
    position: sticky;
    top: 0;
    z-index: 10;
}

.brand,
.nav-links,
.hero,
.hero-actions,
.search-strip,
.trust-row,
.vehicle-list,
.card-bottom,
.process-list,
.info-section,
.site-footer {
    display: flex;
}

.brand {
    align-items: center;
    gap: 10px;
    font-size: 1.25rem;
    font-weight: 800;
}

.brand-mark {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 42px;
    height: 42px;
    border-radius: 50%;
    color: white;
    background: var(--accent);
    font-size: 0.9rem;
    letter-spacing: 0;
}

.nav-links {
    align-items: center;
    gap: 22px;
    font-weight: 700;
}

.nav-links a {
    text-decoration: none;
    color: var(--muted);
}

.nav-links a:hover {
    color: var(--accent);
}

.hero {
    align-items: center;
    justify-content: space-between;
    gap: 44px;
    padding: 58px 7% 36px;
}

.hero-copy,
.hero-panel {
    flex: 1 1 420px;
}

.eyebrow {
    margin: 0 0 8px;
    color: var(--accent);
    font-size: 0.78rem;
    font-weight: 800;
    text-transform: uppercase;
    letter-spacing: 0.08em;
}

h1,
h2,
h3,
p {
    margin-top: 0;
}

h1 {
    margin-bottom: 18px;
    max-width: 720px;
    font-size: clamp(2.3rem, 5vw, 4.9rem);
    line-height: 1;
    letter-spacing: 0;
}

h2 {
    margin-bottom: 10px;
    font-size: clamp(1.65rem, 3vw, 2.55rem);
    line-height: 1.15;
    letter-spacing: 0;
}

h3 {
    margin-bottom: 8px;
}

.hero-text {
    max-width: 610px;
    color: var(--muted);
    font-size: 1.08rem;
}

.hero-actions {
    flex-wrap: wrap;
    gap: 12px;
    margin-top: 26px;
}

.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 46px;
    padding: 0 20px;
    border-radius: 6px;
    text-decoration: none;
    font-weight: 800;
}

.btn.primary {
    color: white;
    background: var(--accent);
}

.btn.primary:hover {
    background: var(--accent-dark);
}

.btn.secondary {
    border: 1px solid var(--accent);
    color: var(--accent-dark);
    background: transparent;
}

.hero-panel {
    position: relative;
    min-height: 340px;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 22px 46px rgba(23, 33, 43, 0.18);
}

.hero-panel img {
    width: 100%;
    height: 100%;
    min-height: 340px;
    object-fit: cover;
}

.price-strip {
    position: absolute;
    left: 18px;
    right: 18px;
    bottom: 18px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 18px;
    padding: 14px 16px;
    border-radius: 6px;
    color: white;
    background: rgba(23, 33, 43, 0.86);
}

.search-strip {
    align-items: end;
    flex-wrap: wrap;
    gap: 16px;
    width: 86%;
    margin: 0 auto 38px;
    padding: 18px;
    border: 1px solid var(--line);
    border-radius: 8px;
    background: var(--surface);
    box-shadow: 0 14px 32px rgba(23, 33, 43, 0.08);
}

.search-strip label {
    flex: 1 1 180px;
    color: var(--muted);
    font-size: 0.82rem;
    font-weight: 800;
}

.search-strip select {
    width: 100%;
    min-height: 44px;
    margin-top: 6px;
    padding: 0 12px;
    border: 1px solid var(--line);
    border-radius: 6px;
    color: var(--ink);
    background: var(--soft);
    font: inherit;
}

.search-strip .btn {
    flex: 0 0 auto;
}

.trust-row {
    justify-content: center;
    flex-wrap: wrap;
    gap: 16px;
    padding: 0 7% 46px;
}

.trust-row div {
    flex: 1 1 210px;
    max-width: 320px;
    padding: 18px;
    border: 1px solid var(--line);
    border-radius: 8px;
    background: var(--surface);
}

.trust-row strong {
    display: block;
    color: var(--accent-dark);
    font-size: 1.8rem;
    line-height: 1.1;
}

.trust-row span,
.vehicle-card p,
.process-step p,
.info-copy p,
.site-footer p,
.contact-box p {
    color: var(--muted);
}

.section {
    padding: 54px 7%;
}

.section-heading {
    max-width: 680px;
    margin-bottom: 26px;
}

.section-heading p:not(.eyebrow) {
    color: var(--muted);
}

.vehicle-list {
    flex-wrap: wrap;
    gap: 22px;
}

.vehicle-card {
    flex: 1 1 280px;
    overflow: hidden;
    border: 1px solid var(--line);
    border-radius: 8px;
    background: var(--surface);
    box-shadow: 0 12px 28px rgba(23, 33, 43, 0.08);
}

.vehicle-card img {
    width: 100%;
    height: 210px;
    object-fit: cover;
}

.vehicle-content {
    padding: 20px;
}

.card-bottom {
    align-items: center;
    justify-content: space-between;
    gap: 14px;
    margin-top: 18px;
}

.card-bottom strong {
    color: var(--accent-dark);
    font-size: 1.2rem;
}

.card-bottom a {
    color: var(--accent);
    font-weight: 800;
    text-decoration: none;
}

.process-section {
    background: var(--ink);
    color: white;
}

.process-section .eyebrow,
.process-section h2 {
    color: white;
}

.process-list {
    flex-wrap: wrap;
    gap: 18px;
}

.process-step {
    flex: 1 1 240px;
    padding: 24px;
    border: 1px solid rgba(255, 255, 255, 0.16);
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.06);
}

.process-step span {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 38px;
    height: 38px;
    margin-bottom: 16px;
    border-radius: 50%;
    color: var(--ink);
    background: var(--gold);
    font-weight: 800;
}

.process-step p {
    color: #d7dde3;
}

.info-section {
    align-items: stretch;
    gap: 24px;
}

.info-copy {
    flex: 2 1 520px;
}

.contact-box {
    flex: 1 1 280px;
    padding: 26px;
    border-radius: 8px;
    color: white;
    background: var(--accent-dark);
}

.contact-box h2 {
    font-size: 1.6rem;
}

.contact-box p {
    color: #d9fffb;
}

.contact-box .btn {
    width: 100%;
    margin-top: 10px;
    background: white;
    color: var(--accent-dark);
}

.site-footer {
    align-items: center;
    justify-content: space-between;
    gap: 24px;
    padding: 28px 7%;
    color: white;
    background: #111820;
}

.site-footer p {
    margin-bottom: 0;
    color: #c3cbd3;
}

@media (max-width: 820px) {
    .site-header,
    .hero,
    .search-strip,
    .info-section,
    .site-footer {
        flex-direction: column;
        align-items: flex-start;
    }

    .nav-links {
        width: 100%;
        flex-wrap: wrap;
        gap: 12px 18px;
    }

    .hero {
        padding-top: 36px;
    }

    .hero-panel,
    .hero-panel img {
        min-height: 280px;
    }

    .search-strip {
        align-items: stretch;
        width: 86%;
    }

    .search-strip .btn {
        width: 100%;
    }

    .price-strip {
        align-items: flex-start;
        flex-direction: column;
        gap: 4px;
    }
}

@media (max-width: 540px) {
    .site-header,
    .hero,
    .search-strip,
    .section,
    .site-footer {
        padding-left: 5%;
        padding-right: 5%;
    }

    .nav-links {
        flex-direction: column;
        align-items: flex-start;
    }

    .hero-actions,
    .btn {
        width: 100%;
    }

    .trust-row {
        padding-left: 5%;
        padding-right: 5%;
    }

    .vehicle-card,
    .process-step {
        flex-basis: 100%;
    }
}

```

## OUTPUT
<img width="1521" height="697" alt="image" src="https://github.com/user-attachments/assets/62c31f2d-4077-4ace-947d-8f77111799ec" />
<img width="1522" height="662" alt="image" src="https://github.com/user-attachments/assets/2d4c65f8-14f4-42b2-9333-b4c7a7de33ce" />
<img width="1522" height="697" alt="image" src="https://github.com/user-attachments/assets/e41fbbe9-645c-4d8e-a8c9-58636d7c7a5e" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
