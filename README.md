/* ===== SHOPIFY DROPSHIPPING STORE CUSTOM CSS ===== */
/* ===== CSS Variables & Reset ===== */
:root {
    --primary: #3a86ff;
    --primary-dark: #2667cc;
    --secondary: #ff006e;
    --dark: #1a1a2e;
    --light: #f8f9fa;
    --gray: #6c757d;
    --light-gray: #e9ecef;
    --success: #38b000;
    --border-radius: 12px;
    --box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    --transition: all 0.3s ease;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Poppins', sans-serif;
    line-height: 1.6;
    color: var(--dark);
    background-color: #fff;
    overflow-x: hidden;
}

h1, h2, h3, h4, h5, h6 {
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
    line-height: 1.3;
    margin-bottom: 1rem;
}

.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

section {
    padding: 80px 0;
}

img {
    max-width: 100%;
    height: auto;
    display: block;
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style: none;
}

.btn {
    display: inline-block;
    padding: 14px 32px;
    border-radius: var(--border-radius);
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    cursor: pointer;
    transition: var(--transition);
    border: none;
    font-family: 'Montserrat', sans-serif;
    font-size: 0.9rem;
}

.btn-primary {
    background-color: var(--primary);
    color: white;
}

.btn-primary:hover {
    background-color: var(--primary-dark);
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(58, 134, 255, 0.2);
}

.btn-secondary {
    background-color: var(--secondary);
    color: white;
}

.btn-secondary:hover {
    background-color: #d8005e;
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(255, 0, 110, 0.2);
}

.section-title {
    text-align: center;
    margin-bottom: 60px;
}

.section-title h2 {
    font-size: 2.5rem;
    position: relative;
    display: inline-block;
    padding-bottom: 15px;
}

.section-title h2:after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 80px;
    height: 4px;
    background-color: var(--primary);
}

/* ===== Header & Navigation ===== */
.header {
    background-color: white;
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.header-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}

.logo {
    font-family: 'Montserrat', sans-serif;
    font-size: 1.8rem;
    font-weight: 700;
    color: var(--dark);
}

.logo span {
    color: var(--primary);
}

.nav-links {
    display: flex;
    gap: 30px;
}

.nav-links a {
    font-weight: 500;
    position: relative;
}

.nav-links a:after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 0;
    height: 2px;
    background-color: var(--primary);
    transition: var(--transition);
}

.nav-links a:hover:after {
    width: 100%;
}

.header-icons {
    display: flex;
    gap: 20px;
    font-size: 1.2rem;
}

.header-icons i {
    cursor: pointer;
    transition: var(--transition);
}

.header-icons i:hover {
    color: var(--primary);
}

.cart-count {
    position: absolute;
    top: -8px;
    right: -8px;
    background-color: var(--secondary);
    color: white;
    font-size: 0.7rem;
    width: 18px;
    height: 18px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.mobile-menu-btn {
    display: none;
    font-size: 1.5rem;
    cursor: pointer;
}

/* ===== Hero Section ===== */
.hero-section {
    background: linear-gradient(135deg, rgba(58, 134, 255, 0.05) 0%, rgba(255, 0, 110, 0.05) 100%);
    padding: 100px 0;
    position: relative;
    overflow: hidden;
}

.hero-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 40px;
}

.hero-content {
    flex: 1;
}

.hero-content h1 {
    font-size: 3.5rem;
    margin-bottom: 20px;
    line-height: 1.2;
}

.hero-content p {
    font-size: 1.1rem;
    color: var(--gray);
    margin-bottom: 30px;
    max-width: 500px;
}

.hero-btns {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
}

.hero-image {
    flex: 1;
    position: relative;
}

.hero-image img {
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    transform: perspective(1000px) rotateY(-10deg);
    transition: var(--transition);
}

.hero-image img:hover {
    transform: perspective(1000px) rotateY(0deg);
}

/* ===== Featured Products ===== */
.featured-products {
    background-color: var(--light);
}

.products-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 30px;
}

.product-card {
    background-color: white;
    border-radius: var(--border-radius);
    overflow: hidden;
    box-shadow: var(--box-shadow);
    transition: var(--transition);
    position: relative;
}

.product-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
}

.product-badge {
    position: absolute;
    top: 15px;
    left: 15px;
    background-color: var(--secondary);
    color: white;
    padding: 5px 12px;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
    z-index: 2;
}

.product-image {
    height: 250px;
    overflow: hidden;
}

.product-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition);
}

.product-card:hover .product-image img {
    transform: scale(1.05);
}

.product-info {
    padding: 20px;
}

.product-title {
    font-size: 1.2rem;
    margin-bottom: 10px;
}

.product-price {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 15px;
}

.current-price {
    font-size: 1.3rem;
    font-weight: 700;
    color: var(--primary);
}

.original-price {
    font-size: 1rem;
    color: var(--gray);
    text-decoration: line-through;
}

.product-rating {
    color: #ffc107;
    margin-bottom: 15px;
}

.add-to-cart {
    width: 100%;
    padding: 12px;
    background-color: var(--light-gray);
    color: var(--dark);
    font-weight: 600;
}

.add-to-cart:hover {
    background-color: var(--primary);
    color: white;
}

/* ===== Promotional Banner ===== */
.promo-banner {
    background: linear-gradient(rgba(26, 26, 46, 0.85), rgba(26, 26, 46, 0.9)), url('https://images.unsplash.com/photo-1441986300917-64674bd600d8?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80');
    background-size: cover;
    background-position: center;
    color: white;
    text-align: center;
    padding: 100px 20px;
    border-radius: var(--border-radius);
    margin: 40px 0;
}

.promo-banner h2 {
    font-size: 2.8rem;
    margin-bottom: 20px;
}

.promo-banner p {
    font-size: 1.2rem;
    max-width: 700px;
    margin: 0 auto 30px;
    opacity: 0.9;
}

.countdown {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-bottom: 40px;
}

.countdown-item {
    background-color: rgba(255, 255, 255, 0.15);
    border-radius: 10px;
    padding: 20px;
    min-width: 100px;
    backdrop-filter: blur(10px);
}

.countdown-number {
    font-size: 2.5rem;
    font-weight: 700;
    display: block;
}

.countdown-label {
    font-size: 0.9rem;
    opacity: 0.8;
}

/* ===== Benefits Section ===== */
.benefits-section {
    background-color: var(--light);
}

.benefits-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
}

.benefit-card {
    background-color: white;
    padding: 40px 30px;
    border-radius: var(--border-radius);
    text-align: center;
    box-shadow: var(--box-shadow);
    transition: var(--transition);
}

.benefit-card:hover {
    transform: translateY(-10px);
}

.benefit-icon {
    width: 70px;
    height: 70px;
    background-color: rgba(58, 134, 255, 0.1);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 20px;
    font-size: 1.8rem;
    color: var(--primary);
}

.benefit-card h3 {
    font-size: 1.4rem;
    margin-bottom: 15px;
}

/* ===== Testimonials ===== */
.testimonials-section {
    padding: 80px 0;
}

.testimonials-slider {
    max-width: 800px;
    margin: 0 auto;
    position: relative;
}

.testimonial-card {
    background-color: white;
    padding: 40px;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    text-align: center;
    margin: 0 20px;
}

.customer-avatar {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    overflow: hidden;
    margin: 0 auto 20px;
    border: 5px solid var(--light-gray);
}

.customer-avatar img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.testimonial-text {
    font-style: italic;
    margin-bottom: 20px;
    font-size: 1.1rem;
}

.customer-name {
    font-weight: 600;
    color: var(--dark);
}

.stars {
    color: #ffc107;
    margin-bottom: 10px;
}

/* ===== Product Collection Grid ===== */
.collection-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
    margin-top: 40px;
}

.collection-card {
    position: relative;
    border-radius: var(--border-radius);
    overflow: hidden;
    height: 400px;
}

.collection-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition);
}

.collection-card:hover img {
    transform: scale(1.05);
}

.collection-overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
    padding: 30px;
    color: white;
}

/* ===== Newsletter Section ===== */
.newsletter-section {
    background-color: var(--primary);
    color: white;
    text-align: center;
    padding: 80px 0;
}

.newsletter-content {
    max-width: 600px;
    margin: 0 auto;
}

.newsletter-form {
    display: flex;
    max-width: 500px;
    margin: 30px auto;
}

.newsletter-form input {
    flex: 1;
    padding: 16px 20px;
    border: none;
    border-radius: var(--border-radius) 0 0 var(--border-radius);
    font-family: 'Poppins', sans-serif;
    font-size: 1rem;
}

.newsletter-form button {
    background-color: var(--secondary);
    color: white;
    border: none;
    border-radius: 0 var(--border-radius) var(--border-radius) 0;
    padding: 0 30px;
    cursor: pointer;
    font-weight: 600;
    transition: var(--transition);
}

.newsletter-form button:hover {
    background-color: #d8005e;
}

/* ===== Footer ===== */
.main-footer {
    background-color: var(--dark);
    color: white;
    padding: 80px 0 30px;
}

.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 40px;
    margin-bottom: 50px;
}

.footer-column h3 {
    font-size: 1.3rem;
    margin-bottom: 25px;
    position: relative;
    padding-bottom: 10px;
}

.footer-column h3:after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 40px;
    height: 3px;
    background-color: var(--primary);
}

.footer-links li {
    margin-bottom: 12px;
}

.footer-links a {
    color: #b0b7c3;
    transition: var(--transition);
}

.footer-links a:hover {
    color: var(--primary);
    padding-left: 5px;
}

.newsletter p {
    color: #b0b7c3;
    margin-bottom: 20px;
}

.social-links {
    display: flex;
    gap: 15px;
    margin-top: 20px;
}

.social-links a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 50%;
    transition: var(--transition);
}

.social-links a:hover {
    background-color: var(--primary);
    transform: translateY(-5px);
}

.footer-bottom {
    text-align: center;
    padding-top: 30px;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    color: #b0b7c3;
    font-size: 0.9rem;
}

/* ===== Shopify Specific Overrides ===== */
/* Product Page Enhancements */
.product-template .product-images img {
    border-radius: var(--border-radius);
}

.product-template .product-price {
    font-size: 1.8rem;
    color: var(--primary);
}

.product-template .add-to-cart-button {
    background-color: var(--primary);
    color: white;
    padding: 16px 40px;
    border-radius: var(--border-radius);
    border: none;
    font-weight: 600;
    transition: var(--transition);
}

.product-template .add-to-cart-button:hover {
    background-color: var(--primary-dark);
    transform: translateY(-3px);
}

/* Collection Page */
.collection-template .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 30px;
}

/* Cart Page */
.cart-page .cart-item {
    border-bottom: 1px solid var(--light-gray);
    padding: 20px 0;
}

.cart-page .update-cart,
.cart-page .checkout-button {
    background-color: var(--primary);
    color: white;
    border: none;
    padding: 12px 30px;
    border-radius: var(--border-radius);
    font-weight: 600;
    transition: var(--transition);
}

.cart-page .update-cart:hover,
.cart-page .checkout-button:hover {
    background-color: var(--primary-dark);
}

/* ===== Responsive Design ===== */
@media (max-width: 992px) {
    .hero-container {
        flex-direction: column;
        text-align: center;
    }
    
    .hero-content h1 {
        font-size: 2.8rem;
    }
    
    .hero-btns {
        justify-content: center;
    }
    
    .section-title h2 {
        font-size: 2.2rem;
    }
    
    .promo-banner h2 {
        font-size: 2.2rem;
    }
    
    .collection-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 768px) {
    .nav-links {
        display: none;
    }
    
    .mobile-menu-btn {
        display: block;
    }
    
    .header-icons {
        gap: 15px;
    }
    
    .hero-content h1 {
        font-size: 2.3rem;
    }
    
    .countdown {
        flex-wrap: wrap;
    }
    
    .countdown-item {
        min-width: 80px;
        padding: 15px;
    }
    
    .countdown-number {
        font-size: 2rem;
    }
    
    .testimonial-card {
        padding: 30px 20px;
    }
    
    section {
        padding: 60px 0;
    }
    
    .collection-grid {
        grid-template-columns: 1fr;
    }
    
    .newsletter-form {
        flex-direction: column;
    }
    
    .newsletter-form input,
    .newsletter-form button {
        width: 100%;
        border-radius: var(--border-radius);
        margin-bottom: 10px;
    }
}

@media (max-width: 576px) {
    .hero-content h1 {
        font-size: 2rem;
    }
    
    .section-title h2 {
        font-size: 1.8rem;
    }
    
    .promo-banner h2 {
        font-size: 1.8rem;
    }
    
    .promo-banner {
        padding: 60px 20px;
    }
    
    .btn {
        padding: 12px 24px;
    }
    
    .products-grid {
        grid-template-columns: 1fr;
    }
    
    .footer-content {
        grid-template-columns: 1fr;
    }
}

/* ===== Animation Classes ===== */
.fade-in {
    animation: fadeIn 0.8s ease-out;
}

.slide-up {
    animation: slideUp 0.6s ease-out;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes slideUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* ===== Loading Animation ===== */
.loading-spinner {
    display: inline-block;
    width: 50px;
    height: 50px;
    border: 3px solid var(--light-gray);
    border-top: 3px solid var(--primary);
    border-radius: 50%;
    animation: spin 1s linear infinite;
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

/* ===== Success/Error Messages ===== */
.success-message {
    background-color: #d4edda;
    color: #155724;
    padding: 12px 20px;
    border-radius: var(--border-radius);
    border-left: 4px solid var(--success);
    margin: 10px 0;
}

.error-message {
    background-color: #f8d7da;
    color: #721c24;
    padding: 12px 20px;
    border-radius: var(--border-radius);
    border-left: 4px solid #dc3545;
    margin: 10px 0;
}

/* ===== Custom Scrollbar ===== */
::-webkit-scrollbar {
    width: 10px;
}

::-webkit-scrollbar-track {
    background: var(--light-gray);
}

::-webkit-scrollbar-thumb {
    background: var(--primary);
    border-radius: 5px;
}

::-webkit-scrollbar-thumb:hover {
    background: var(--primary-dark);
}
