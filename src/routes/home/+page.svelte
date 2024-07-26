<script>
    let features = [
        {
            title: "Empowering Financial Independence",
            icon: "/images/hand.png"
        },
        {
            title: "Ensuring Transparency & Trust",
            icon: "/images/transparency.png"
        },
        {
            title: "Efficiency & Automation",
            icon: "/images/efficiency.png"
        }
    ];

    
</script>

<header class="header">
    <div class="logo">
        <img src="/images/hand.png" alt="Logo" class="logo-icon" />
        Timechain Finance</div>
    <nav class="nav">
        <a href="/" class="nav-link">Home</a>
        <a href="#product" class="nav-link">Product</a>
        <a href="#about" class="nav-link">About</a>
        <a href="#contact" class="nav-link">Contact</a>
    </nav>
</header>
<main class="main">

<div class="main-content">
    <div class="content">
        <h1 class="title">Welcome to Timechain Finance!</h1>
        <p class="description">
            Welcome to Timechain Finance, the leading platform for decentralized lending and borrowing of assets.
        </p>
        <div class="features">
            {#each features as feature}
                <div class="feature-item">
                    <img src={feature.icon} alt={feature.title} class="feature-icon" />
                    <span class="feature-title">{feature.title}</span>
                </div>
            {/each}
        </div>
        <div class="auth-buttons">
            <a href="/register" class="cta-button">Register Here</a>
            <a href="/login" class="cta-button">Login</a>
        </div>
    </div>
    <div class="main-image">
        <!-- svelte-ignore a11y-img-redundant-alt -->
        <img src="/images/lending-borrowing-1.png" alt="Main Image" class="image" />
    </div>
</div>


    <div class="info-section">
        <div class="info-image">
            <img src="/images/about img.png" alt="About Us" class="info-img" />
        </div>
        <div class="about-us">
            <h2>About Us</h2>
            <p>
                Timechain Finance is dedicated to revolutionizing the financial industry through innovative decentralized technologies. 
                Our mission is to provide a <span class="highlight"></span>secure and <span class="highlight"></span>transparent platform for lending and borrowing, empowering users to achieve financial independence.
            </p>
            <p>
                We believe in harnessing the power of blockchain to create a more equitable financial ecosystem. Our team of experts works tirelessly to ensure that our platform is user-friendly, reliable, and secure.
            </p>
            <p>
                Join us on our journey to redefine finance and be part of a community that values transparency, efficiency, and innovation.
            </p>
        </div>
    </div>

    <div class="contact-us">
        <h2>Contact Us</h2>
        <p>Follow us on social media:</p>
        <div class="social-media-links">
            <a href="https://facebook.com" class="social-link">Facebook</a>
            <a href="https://twitter.com" class="social-link">Twitter</a>
            <a href="https://linkedin.com" class="social-link">LinkedIn</a>
        </div>
        <p class="contact-info">
            For inquiries, email us at <a href="mailto:support@timechainfinance.com" class="contact-email">support@timechainfinance.com</a>
        </p>
    </div>
</main>
<footer class="footer">
    <p>&copy; 2024 Timechain Finance. All rights reserved.</p>
</footer>

<style lang="scss">
    $primary-color: #1e3a8a;
    $secondary-color: #3b82f6;

   

    .logo {
        display: flex;
        align-items: center;
    }

    .logo-icon {
        width: 60px; 
        height: auto;
        margin-right: 0.5rem; 
    }

    .header {
        background-color: hsl(174, 81%, 44%);
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        padding: 1rem 1.5rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .logo {
        font-size: 2.0rem;
        font-weight: bold;
    }

    .nav {
        display: flex;
        gap: 2rem;
        margin-left: auto;
        margin-right: 1rem;
    }

    .nav-link {
        color: #070d2a;
        text-decoration: none;
        transition: color 0.3s;
        font-size: 2.0rem;
        font-weight: bold;
    }

    .nav-link:hover {
        color: #2d3748;
    }

    .main {
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center; 
        background-color: white;
        padding: 2.5rem 1rem;
        gap: 2rem;
    }
    .main-image {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
}

.image {
    max-width: 100%;
    height: auto;
    border-radius: 0.375rem;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

    .main-content {
        display: flex;
        gap: 2rem;
        width: 100%;
        max-width: 105rem;
        justify-content: center; 
    }

    .content {
        padding: 1.5rem;
        background-color: white;
        border-radius: 0.375rem;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        max-width: 60rem; 
    }

    .title {
        font-size: 3.7rem;
        font-weight: bold;
        background: linear-gradient(45deg, #1e3a8a, #3b82f6); /* Blue gradient */
        -webkit-background-clip: text; 
        background-clip: text; 
        -webkit-text-fill-color: transparent; 
    }

    .description {
        font-size: 2.0rem;
        margin-bottom: 1.5rem;
    }

    .features {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    .feature-item {
        display: flex;
        align-items: center;
        gap: 0.5rem;
    }

    .feature-icon {
        width: 4rem;
        height: 4rem;
    }

    .feature-title {
        font-size: 2.0rem;
    }

    .auth-buttons {
        display: flex;
        gap: 2rem;
        margin-top: 2rem;
        justify-content: flex-start;
    }

    .cta-button {
        background: linear-gradient(45deg, #1e3a8a, #3b82f6); 
        color: transparent;
        font-weight: bold;
        padding: 0.8rem 1.5rem; 
        border-radius: 1rem;
        text-decoration: none;
        transition: background-color 0.3s, color 0.3s, border 0.3s;
        font-size: 2.0rem;
        background-clip: text; 
        -webkit-background-clip: text; 
        -webkit-text-fill-color: transparent; 
        border: 2px solid #1e3a8a;
        display: inline-block;
        box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15); 
    }

    .cta-button:hover {
        background-color: #e0eb11; 
        color: rgb(184, 24, 24);
        border: 2px solid rgb(19, 2, 15); 
        box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15); 
    }

    .info-section {
        display: flex;
        align-items: center;
        justify-content: space-between;
        gap: 2rem;
        padding: 2rem 1rem;
    }

    .info-image {
        flex: 1;
        display: flex;
        justify-content: center;
    }

    .info-img {
        max-width: 65%;
        height: auto;
        border-radius: 0.375rem;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .about-us {
        flex: 1;
        max-width: 60rem; 
        background-color: white;
        border-radius: 0.375rem;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        padding: 1.5rem;
        text-align: center;
    }

    .about-us h2 {
        font-size: 3.7rem;
        font-weight: bold;
        margin-bottom: 1rem;
        background: linear-gradient(45deg, #1e3a8a, #3b82f6); 
        -webkit-background-clip: text; 
        background-clip: text; 
        -webkit-text-fill-color: transparent; 
    }

    .about-us p {
        font-size: 2.0rem;
        margin-bottom: 1.5rem;
    }

    .contact-us {
        width: 100%;
        max-width: 100rem; 
        padding: 2rem;
        background-color: hsl(210, 100%, 95%);
        border-radius: 0.375rem;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        text-align: center;
    }

    .contact-us h2 {
        font-size: 3.0rem;
        font-weight: bold;
        margin-bottom: 1rem;
    }

    .contact-us p {
        font-size: 1.8rem; 
        margin-bottom: 1.5rem;
    }

    .contact-us .social-media-links {
        display: flex;
        justify-content: center;
        gap: 1.5rem;
        margin-top: 1.5rem;
    }

    .social-link {
        font-size: 1.8rem;
        color: #1e3a8a;
        text-decoration: none;
        transition: color 0.3s;
    }

    .social-link:hover {
        color: #3b82f6;
    }

    .contact-email {
        color: #1e3a8a;
        text-decoration: none;
    }

    .contact-email:hover {
        text-decoration: underline;
    }

    .footer {
        background-color: hsl(174, 81%, 44%);
        padding: 1cm 1.5rem;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 4rem;
    }

    .footer p {
        color: #fff;
        font-size: 2rem;
    }
</style>
