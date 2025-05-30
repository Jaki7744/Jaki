<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SoundWave - Premium Headphones & Headsets</title>
<script src="https://cdn.tailwindcss.com/3.4.16"></script>
<script>tailwind.config={theme:{extend:{colors:{primary:'#007AFF',secondary:'#1A1A1A'},borderRadius:{'none':'0px','sm':'4px',DEFAULT:'8px','md':'12px','lg':'16px','xl':'20px','2xl':'24px','3xl':'32px','full':'9999px','button':'8px'}}}}</script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/remixicon/4.6.0/remixicon.min.css">
<style>
:where([class^="ri-"])::before { content: "\f3c2"; }
body {
  font-family: 'Inter', sans-serif;
  scroll-behavior: smooth;
}
.feedback-message {
  z-index: 9999;
  opacity: 1;
  transition: opacity 0.3s ease;
}
#loginModal {
  transition: opacity 0.3s ease;
}
#loginForm, #registerForm {
  transition: opacity 0.15s ease;
}
.custom-checkbox:hover .checkmark {
  transform: scale(1.05);
}
.custom-checkbox .checkmark {
  transition: all 0.2s ease;
}
input:focus {
  transition: all 0.2s ease;
  box-shadow: 0 0 0 2px rgba(0, 122, 255, 0.1);
}
.hero-section {
  background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                    url('https://images.unsplash.com/photo-1505740420928-5e560c06d30e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1920&q=80');
  background-size: cover;
  background-position: center;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  -webkit-appearance: none;
  margin: 0;
}
.custom-checkbox {
  position: relative;
  padding-left: 28px;
  cursor: pointer;
  user-select: none;
}
.custom-checkbox input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
}
.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 20px;
  width: 20px;
  background-color: #fff;
  border: 2px solid #e2e8f0;
  border-radius: 4px;
}
.custom-checkbox:hover input ~ .checkmark {
  border-color: #007AFF;
}
.custom-checkbox input:checked ~ .checkmark {
  background-color: #007AFF;
  border-color: #007AFF;
}
.checkmark:after {
  content: "";
  position: absolute;
  display: none;
}
.custom-checkbox input:checked ~ .checkmark:after {
  display: block;
}
.custom-checkbox .checkmark:after {
  left: 6px;
  top: 2px;
  width: 5px;
  height: 10px;
  border: solid white;
  border-width: 0 2px 2px 0;
  transform: rotate(45deg);
}
.tab-active {
  color: #007AFF;
  border-bottom: 2px solid #007AFF;
}
.switch {
  position: relative;
  display: inline-block;
  width: 48px;
  height: 24px;
}
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #e2e8f0;
  transition: .4s;
  border-radius: 24px;
}
.slider:before {
  position: absolute;
  content: "";
  height: 18px;
  width: 18px;
  left: 3px;
  bottom: 3px;
  background-color: white;
  transition: .4s;
  border-radius: 50%;
}
input:checked + .slider {
  background-color: #007AFF;
}
input:checked + .slider:before {
  transform: translateX(24px);
}
.tech-specs-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
}
.tech-spec-item {
  background: #f9fafb;
  border-radius: 12px;
  padding: 20px;
  transition: all 0.3s ease;
}
.tech-spec-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px rgba(0,0,0,0.05);
}
.testimonial-card {
  background: white;
  border-radius: 16px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.05);
  padding: 30px;
  transition: all 0.3s ease;
}
.testimonial-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 35px rgba(0,0,0,0.1);
}
.newsletter-form {
  background: linear-gradient(135deg, #007AFF 0%, #1a56db 100%);
  border-radius: 16px;
  overflow: hidden;
}
.hero-content {
  animation: fadeInUp 1s ease-out;
}
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.product-card {
  transition: all 0.3s ease;
}
.product-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
}
</style>
</head>
<body class="bg-white">
<!-- Header/Navigation -->
<header class="fixed w-full bg-white bg-opacity-95 shadow-sm z-50 transition-all duration-300">
  <div class="container mx-auto px-4 py-4 flex items-center justify-between">
    <a href="#" class="text-3xl font-['Pacifico'] text-primary">SoundWave</a>
    <nav class="hidden md:flex items-center space-x-8">
      <a href="#home" class="text-gray-800 hover:text-primary font-medium transition-colors">Home</a>
      <a href="#products" class="text-gray-800 hover:text-primary font-medium transition-colors">Products</a>
      <a href="#tech" class="text-gray-800 hover:text-primary font-medium transition-colors">Technology</a>
      <a href="#testimonials" class="text-gray-800 hover:text-primary font-medium transition-colors">Testimonials</a>
      <a href="#contact" class="text-gray-800 hover:text-primary font-medium transition-colors">Contact</a>
    </nav>
    <div class="flex items-center space-x-4">
      <div id="searchTrigger" class="relative w-10 h-10 flex items-center justify-center cursor-pointer">
        <i class="ri-search-line ri-xl text-gray-700"></i>
      </div>
      <div id="cartTrigger" class="relative w-10 h-10 flex items-center justify-center cursor-pointer">
        <i class="ri-shopping-cart-line ri-xl text-gray-700"></i>
        <span id="cartCount" class="absolute -top-1 -right-1 bg-primary text-white text-xs w-5 h-5 flex items-center justify-center rounded-full">0</span>
      </div>
      <button id="loginBtn" class="bg-primary text-white px-5 py-2 !rounded-button whitespace-nowrap font-medium hover:bg-opacity-90 transition-colors">Login</button>
      <div class="md:hidden w-10 h-10 flex items-center justify-center cursor-pointer" id="mobileMenuBtn">
        <i class="ri-menu-line ri-xl text-gray-700"></i>
      </div>
    </div>
  </div>
  
  <!-- Mobile Menu -->
  <div id="mobileMenu" class="hidden bg-white w-full border-t border-gray-100 py-4 px-4 md:hidden">
    <nav class="flex flex-col space-y-4">
      <a href="#home" class="text-gray-800 hover:text-primary font-medium transition-colors py-2">Home</a>
      <a href="#products" class="text-gray-800 hover:text-primary font-medium transition-colors py-2">Products</a>
      <a href="#tech" class="text-gray-800 hover:text-primary font-medium transition-colors py-2">Technology</a>
      <a href="#testimonials" class="text-gray-800 hover:text-primary font-medium transition-colors py-2">Testimonials</a>
      <a href="#contact" class="text-gray-800 hover:text-primary font-medium transition-colors py-2">Contact</a>
    </nav>
  </div>
</header>

<!-- Main Content -->
<main>
  <!-- Hero Section -->
  <section id="home" class="hero-section min-h-screen flex items-center pt-20">
    <div class="container mx-auto px-6 py-20">
      <div class="max-w-xl hero-content">
        <h1 class="text-5xl md:text-6xl font-bold text-white mb-6 leading-tight">Experience Sound Like Never Before</h1>
        <p class="text-xl text-gray-100 mb-8">Premium headphones engineered for audiophiles with cutting-edge noise cancellation and immersive sound quality.</p>
        <div class="flex flex-wrap gap-4">
          <button class="bg-primary text-white px-8 py-3 !rounded-button whitespace-nowrap font-medium hover:bg-opacity-90 transition-colors">Shop Now</button>
          <button class="bg-white text-gray-900 px-8 py-3 !rounded-button whitespace-nowrap font-medium hover:bg-opacity-90 transition-colors">Learn More</button>
        </div>
      </div>
    </div>
  </section>

  <!-- Featured Products -->
  <section id="products" class="py-20 bg-gray-50">
    <div class="container mx-auto px-4">
      <div class="text-center mb-16">
        <h2 class="text-4xl font-bold mb-4">Featured Products</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">Explore our most popular headphones and headsets, designed for exceptional sound quality and comfort.</p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
        <!-- Product 1 -->
        <div class="bg-white rounded-lg shadow-sm overflow-hidden transition-transform product-card">
          <div class="h-64 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="SoundWave Pro X" class="w-full h-full object-cover">
          </div>
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <span class="text-primary font-medium">Wireless</span>
              <div class="flex items-center">
                <i class="ri-star-fill text-yellow-400"></i>
                <span class="ml-1 text-gray-700">4.9</span>
              </div>
            </div>
            <h3 class="text-xl font-semibold mb-2">SoundWave Pro X</h3>
            <p class="text-gray-600 mb-4">Premium wireless headphones with active noise cancellation.</p>
            <div class="flex justify-between items-center">
              <span class="text-2xl font-bold">₹17,999</span>
              <button class="add-to-cart w-10 h-10 flex items-center justify-center bg-primary text-white !rounded-button hover:bg-opacity-90" data-id="1" data-name="SoundWave Pro X" data-price="17999">
                <i class="ri-shopping-cart-line"></i>
              </button>
            </div>
          </div>
        </div>
        
        <!-- Product 2 -->
        <div class="bg-white rounded-lg shadow-sm overflow-hidden transition-transform product-card">
          <div class="h-64 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1546435770-a3e426bf472b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="GameMaster Elite" class="w-full h-full object-cover">
          </div>
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <span class="text-primary font-medium">Gaming</span>
              <div class="flex items-center">
                <i class="ri-star-fill text-yellow-400"></i>
                <span class="ml-1 text-gray-700">4.8</span>
              </div>
            </div>
            <h3 class="text-xl font-semibold mb-2">GameMaster Elite</h3>
            <p class="text-gray-600 mb-4">Professional gaming headset with 7.1 surround sound.</p>
            <div class="flex justify-between items-center">
              <span class="text-2xl font-bold">₹10,999</span>
              <button class="add-to-cart w-10 h-10 flex items-center justify-center bg-primary text-white !rounded-button hover:bg-opacity-90" data-id="2" data-name="GameMaster Elite" data-price="10999">
                <i class="ri-shopping-cart-line"></i>
              </button>
            </div>
          </div>
        </div>
        
        <!-- Product 3 -->
        <div class="bg-white rounded-lg shadow-sm overflow-hidden transition-transform product-card">
          <div class="h-64 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1583394838336-acd977736f90?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="StudioMaster Pro" class="w-full h-full object-cover">
          </div>
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <span class="text-primary font-medium">Studio</span>
              <div class="flex items-center">
                <i class="ri-star-fill text-yellow-400"></i>
                <span class="ml-1 text-gray-700">4.9</span>
              </div>
            </div>
            <h3 class="text-xl font-semibold mb-2">StudioMaster Pro</h3>
            <p class="text-gray-600 mb-4">Professional studio monitor headphones for audio production.</p>
            <div class="flex justify-between items-center">
              <span class="text-2xl font-bold">₹14,999</span>
              <button class="add-to-cart w-10 h-10 flex items-center justify-center bg-primary text-white !rounded-button hover:bg-opacity-90" data-id="3" data-name="StudioMaster Pro" data-price="14999">
                <i class="ri-shopping-cart-line"></i>
              </button>
            </div>
          </div>
        </div>
        
        <!-- Product 4 -->
        <div class="bg-white rounded-lg shadow-sm overflow-hidden transition-transform product-card">
          <div class="h-64 overflow-hidden">
            <img src="https://images.unsplash.com/photo-1590658268037-6bf12165a8df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=500&q=80" alt="AirPods Ultra" class="w-full h-full object-cover">
          </div>
          <div class="p-6">
            <div class="flex justify-between items-center mb-2">
              <span class="text-primary font-medium">Earbuds</span>
              <div class="flex items-center">
                <i class="ri-star-fill text-yellow-400"></i>
                <span class="ml-1 text-gray-700">4.7</span>
              </div>
            </div>
            <h3 class="text-xl font-semibold mb-2">SoundWave Air</h3>
            <p class="text-gray-600 mb-4">True wireless earbuds with active noise cancellation.</p>
            <div class="flex justify-between items-center">
              <span class="text-2xl font-bold">₹12,999</span>
              <button class="add-to-cart w-10 h-10 flex items-center justify-center bg-primary text-white !rounded-button hover:bg-opacity-90" data-id="4" data-name="SoundWave Air" data-price="12999">
                <i class="ri-shopping-cart-line"></i>
              </button>
            </div>
          </div>
        </div>
      </div>
      <div class="text-center mt-12">
        <button class="bg-white border border-gray-300 text-gray-800 px-8 py-3 !rounded-button whitespace-nowrap font-medium hover:bg-gray-50 transition-colors">View All Products</button>
      </div>
    </div>
  </section>

  <!-- Technology Section -->
  <section id="tech" class="py-20 bg-white">
    <div class="container mx-auto px-4">
      <div class="text-center mb-16">
        <h2 class="text-4xl font-bold mb-4">Advanced Audio Technology</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">Discover the innovation behind our premium sound experience</p>
      </div>
      
      <div class="tech-specs-grid">
        <div class="tech-spec-item">
          <div class="w-12 h-12 rounded-full bg-primary bg-opacity-10 flex items-center justify-center mb-4">
            <i class="ri-sound-module-line text-primary text-2xl"></i>
          </div>
          <h3 class="text-xl font-semibold mb-2">Active Noise Cancellation</h3>
          <p class="text-gray-600">Advanced technology that blocks out ambient noise for immersive listening.</p>
        </div>
        
        <div class="tech-spec-item">
          <div class="w-12 h-12 rounded-full bg-primary bg-opacity-10 flex items-center justify-center mb-4">
            <i class="ri-surround-sound-line text-primary text-2xl"></i>
          </div>
          <h3 class="text-xl font-semibold mb-2">3D Spatial Audio</h3>
          <p class="text-gray-600">Experience sound that moves around you with theater-like immersion.</p>
        </div>
        
        <div class="tech-spec-item">
          <div class="w-12 h-12 rounded-full bg-primary bg-opacity-10 flex items-center justify-center mb-4">
            <i class="ri-battery-charge-line text-primary text-2xl"></i>
          </div>
          <h3 class="text-xl font-semibold mb-2">30-Hour Battery Life</h3>
          <p class="text-gray-600">Extended playback with quick charging capabilities.</p>
        </div>
        
        <div class="tech-spec-item">
          <div class="w-12 h-12 rounded-full bg-primary bg-opacity-10 flex items-center justify-center mb-4">
            <i class="ri-heart-pulse-line text-primary text-2xl"></i>
          </div>
          <h3 class="text-xl font-semibold mb-2">Ergonomic Design</h3>
          <p class="text-gray-600">Memory foam ear cushions for all-day comfort.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonials -->
  <section id="testimonials" class="py-20 bg-gray-50">
    <div class="container mx-auto px-4">
      <div class="text-center mb-16">
        <h2 class="text-4xl font-bold mb-4">Customer Experiences</h2>
        <p class="text-gray-600 max-w-2xl mx-auto">See what our customers say about SoundWave products</p>
      </div>
      
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div class="testimonial-card">
          <div class="flex items-center mb-4">
            <div class="w-12 h-12 rounded-full bg-gray-300 mr-4 overflow-hidden">
              <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80" alt="Sarah" class="w-full h-full object-cover">
            </div>
            <div>
              <h4 class="font-semibold">Sarah Johnson</h4>
              <div class="flex text-yellow-400">
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
              </div>
            </div>
          </div>
          <p class="text-gray-600 italic">"The noise cancellation is incredible! I can focus on my work even in busy coffee shops. The sound quality is studio-grade."</p>
        </div>
        
        <div class="testimonial-card">
          <div class="flex items-center mb-4">
            <div class="w-12 h-12 rounded-full bg-gray-300 mr-4 overflow-hidden">
              <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80" alt="Michael" class="w-full h-full object-cover">
            </div>
            <div>
              <h4 class="font-semibold">Michael Chen</h4>
              <div class="flex text-yellow-400">
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-half-fill"></i>
              </div>
            </div>
          </div>
          <p class="text-gray-600 italic">"As a professional gamer, the GameMaster Elite gives me the competitive edge. The surround sound is incredibly accurate."</p>
        </div>
        
        <div class="testimonial-card">
          <div class="flex items-center mb-4">
            <div class="w-12 h-12 rounded-full bg-gray-300 mr-4 overflow-hidden">
              <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80" alt="Priya" class="w-full h-full object-cover">
            </div>
            <div>
              <h4 class="font-semibold">Priya Patel</h4>
              <div class="flex text-yellow-400">
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
                <i class="ri-star-fill"></i>
              </div>
            </div>
          </div>
          <p class="text-gray-600 italic">"The comfort is unmatched. I wear these for 8+ hours daily and never experience ear fatigue. Sound quality is phenomenal."</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Newsletter -->
  <section class="py-20">
    <div class="container mx-auto px-4">
      <div class="newsletter-form p-8 md:p-12 max-w-4xl mx-auto">
        <div class="flex flex-col md:flex-row items-center">
          <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
            <h3 class="text-2xl md:text-3xl font-bold text-white mb-4">Join Our Audiophile Community</h3>
            <p class="text-blue-100">Get exclusive deals, early access to new products, and audio tips from our experts.</p>
          </div>
          <div class="md:w-1/2 w-full">
            <div class="flex">
              <input type="email" placeholder="Your email address" class="flex-grow px-4 py-3 rounded-l-lg focus:outline-none">
              <button class="bg-secondary text-white px-6 py-3 whitespace-nowrap font-medium hover:bg-opacity-90 transition-colors rounded-r-lg">Subscribe</button>
            </div>
            <p class="text-blue-100 text-sm mt-3">We respect your privacy. Unsubscribe at any time.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</main>

<!-- Footer -->
<footer class="bg-gray-900 text-white pt-16 pb-8">
  <div class="container mx-auto px-4">
    <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-12">
      <div>
        <h4 class="text-xl font-semibold mb-4">SoundWave</h4>
        <p class="text-gray-400 mb-4">Premium audio products designed for those who demand exceptional sound quality.</p>
        <div class="flex space-x-4">
          <a href="#" class="text-gray-400 hover:text-white"><i class="ri-facebook-fill ri-lg"></i></a>
          <a href="#" class="text-gray-400 hover:text-white"><i class="ri-twitter-fill ri-lg"></i></a>
          <a href="#" class="text-gray-400 hover:text-white"><i class="ri-instagram-line ri-lg"></i></a>
          <a href="#" class="text-gray-400 hover:text-white"><i class="ri-youtube-fill ri-lg"></i></a>
        </div>
      </div>
      
      <div>
        <h4 class="text-xl font-semibold mb-4">Shop</h4>
        <ul class="space-y-2">
          <li><a href="#" class="text-gray-400 hover:text-white">Headphones</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Earbuds</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Gaming Headsets</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Studio Monitors</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Accessories</a></li>
        </ul>
      </div>
      
      <div>
        <h4 class="text-xl font-semibold mb-4">Support</h4>
        <ul class="space-y-2">
          <li><a href="#" class="text-gray-400 hover:text-white">Product Help</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Register Your Product</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Updates & Downloads</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Contact Support</a></li>
          <li><a href="#" class="text-gray-400 hover:text-white">Warranty</a></li>
        </ul>
      </div>
      
      <div>
        <h4 class="text-xl font-semibold mb-4">Contact Us</h4>
        <ul class="space-y-3">
          <li class="flex items-start">
            <i class="ri-map-pin-line text-gray-400 mt-1 mr-3"></i>
            <span class="text-gray-400">123 Audio Street, Bangalore, India 560001</span>
          </li>
          <li class="flex items-start">
            <i class="ri-phone-line text-gray-400 mt-1 mr-3"></i>
            <span class="text-gray-400">+91 98765 43210</span>
          </li>
          <li class="flex items-start">
            <i class="ri-mail-line text-gray-400 mt-1 mr-3"></i>
            <span class="text-gray-400">support@soundwave.com</span>
          </li>
        </ul>
      </div>
    </div>
    
    <div class="border-t border-gray-800 pt-8 text-center">
      <p class="text-gray-400">© 2023 SoundWave. All rights reserved.</p>
    </div>
  </div>
</footer>

<!-- Login Modal -->
<div id="loginModal" class="hidden fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 p-4">
  <div class="bg-white rounded-xl w-full max-w-md overflow-hidden">
    <div class="p-6">
      <div class="flex justify-between items-center mb-6">
        <h3 class="text-2xl font-bold">Welcome to SoundWave</h3>
        <button id="closeModal" class="text-gray-500 hover:text-gray-700">
          <i class="ri-close-line ri-xl"></i>
        </button>
      </div>
      
      <div class="flex border-b mb-6">
        <button id="loginTab" class="tab-active py-2 px-4 font-medium">Sign In</button>
        <button id="registerTab" class="py-2 px-4 font-medium text-gray-500 hover:text-gray-700">Register</button>
      </div>
      
      <form id="loginForm">
        <div class="mb-4">
          <label class="block text-gray-700 mb-2" for="email">Email</label>
          <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-primary">
        </div>
        <div class="mb-6">
          <label class="block text-gray-700 mb-2" for="password">Password</label>
          <input type="password" id="password" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-primary">
        </div>
        <div class="flex items-center justify-between mb-6">
          <label class="custom-checkbox flex items-center">
            <input type="checkbox">
            <span class="checkmark"></span>
            <span class="ml-2 text-gray-700">Remember me</span>
          </label>
          <a href="#" class="text-primary hover:underline">Forgot password?</a>
        </div>
        <button type="submit" class="w-full bg-primary text-white py-3 rounded-lg font-medium hover:bg-opacity-90 transition-colors">Sign In</button>
      </form>
      
      <form id="registerForm" class="hidden">
        <div class="mb-4">
          <label class="block text-gray-700 mb-2" for="name">Full Name</label>
          <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-primary">
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 mb-2" for="reg-email">Email</label>
          <input type="email" id="reg-email" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-primary">
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 mb-2" for="reg-password">Password</label>
          <input type="password" id="reg-password" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-primary">
        </div>
        <div class="mb-6">
          <label class="block text-gray-700 mb-2" for="confirm-password">Confirm Password</label>
          <input type="password" id="confirm-password" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-primary">
        </div>
        <button type="submit" class="w-full bg-primary text-white py-3 rounded-lg font-medium hover:bg-opacity-90 transition-colors">Create Account</button>
      </form>
      
      <div class="mt-6 text-center">
        <p class="text-gray-600">Or continue with</p>
        <div class="flex justify-center space-x-4 mt-4">
          <button class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center">
            <i class="ri-google-fill text-xl"></i>
          </button>
          <button class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center">
            <i class="ri-facebook-fill text-xl text-blue-600"></i>
          </button>
          <button class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center">
            <i class="ri-apple-fill text-xl"></i>
          </button>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Feedback Message -->
<div id="feedbackMessage" class="feedback-message hidden fixed top-6 right-6 bg-green-500 text-white px-6 py-3 rounded-lg shadow-lg">
  <div class="flex items-center">
    <i class="ri-check-line mr-2"></i>
    <span>Item added to cart!</span>
  </div>
</div>

<!-- Cart Dropdown -->
<div id="cartDropdown" class="hidden absolute right-0 top-full mt-2 w-80 bg-white rounded-lg shadow-lg border border-gray-100 z-50">
  <div class="p-4">
    <h3 class="font-semibold text-lg mb-4">Your Cart</h3>
    <div id="cartItems" class="space-y-4 mb-4">
      <!-- Cart items will be added dynamically -->
      <div class="text-center py-8 text-gray-500">
        <i class="ri-shopping-cart-line text-4xl mb-2"></i>
        <p>Your cart is empty</p>
      </div>
    </div>
    <div class="border-t border-gray-100 pt-3 mb-4">
      <div class="flex justify-between items-center mb-1">
        <span class="font-medium">Subtotal</span>
        <span id="cartSubtotal" class="font-medium">₹0</span>
      </div>
      <p class="text-gray-500 text-sm">Shipping & taxes calculated at checkout</p>
    </div>
    <div class="grid grid-cols-2 gap-2">
      <button class="bg-gray-100 text-gray-800 px-4 py-2 !rounded-button whitespace-nowrap font-medium hover:bg-gray-200 transition-colors">View Cart</button>
      <button class="bg-primary text-white px-4 py-2 !rounded-button whitespace-nowrap font-medium hover:bg-opacity-90 transition-colors">Checkout</button>
    </div>
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  // Mobile menu toggle
  const mobileMenuBtn = document.getElementById('mobileMenuBtn');
  const mobileMenu = document.getElementById('mobileMenu');
  
  mobileMenuBtn.addEventListener('click', () => {
    mobileMenu.classList.toggle('hidden');
  });
  
  // Login modal
  const loginBtn = document.getElementById('loginBtn');
  const loginModal = document.getElementById('loginModal');
  const closeModal = document.getElementById('closeModal');
  const loginTab = document.getElementById('loginTab');
  const registerTab = document.getElementById('registerTab');
  const loginForm = document.getElementById('loginForm');
  const registerForm = document.getElementById('registerForm');
  
  loginBtn.addEventListener('click', () => {
    loginModal.classList.remove('hidden');
  });
  
  closeModal.addEventListener('click', () => {
    loginModal.classList.add('hidden');
  });
  
  loginTab.addEventListener('click', () => {
    loginTab.classList.add('tab-active');
    registerTab.classList.remove('tab-active');
    loginForm.classList.remove('hidden');
    registerForm.classList.add('hidden');
  });
  
  registerTab.addEventListener('click', () => {
    registerTab.classList.add('tab-active');
    loginTab.classList.remove('tab-active');
    registerForm.classList.remove('hidden');
    loginForm.classList.add('hidden');
  });
  
  // Cart functionality
  const cartTrigger = document.getElementById('cartTrigger');
  const cartDropdown = document.getElementById('cartDropdown');
  const cartCount = document.getElementById('cartCount');
  const cartItems = document.getElementById('cartItems');
  const cartSubtotal = document.getElementById('cartSubtotal');
  const addToCartButtons = document.querySelectorAll('.add-to-cart');
  const feedbackMessage = document.getElementById('feedbackMessage');
  
  let cart = [];
  
  cartTrigger.addEventListener('click', (e) => {
    e.stopPropagation();
    cartDropdown.classList.toggle('hidden');
  });
  
  document.addEventListener('click', (e) => {
    if (!cartDropdown.contains(e.target) {
      cartDropdown.classList.add('hidden');
    }
  });
  
  addToCartButtons.forEach(button => {
    button.addEventListener('click', () => {
      const id = button.getAttribute('data-id');
      const name = button.getAttribute('data-name');
      const price = parseInt(button.getAttribute('data-price'));
      
      // Check if item already in cart
      const existingItem = cart.find(item => item.id === id);
      
      if (existingItem) {
        existingItem.quantity += 1;
      } else {
        cart.push({
          id,
          name,
          price,
          quantity: 1
        });
      }
      
      updateCart();
      
      // Show feedback message
      feedbackMessage.classList.remove('hidden');
      setTimeout(() => {
        feedbackMessage.classList.add('hidden');
      }, 3000);
    });
  });
  
  function updateCart() {
    // Update cart count
    const totalItems = cart.reduce((total, item) => total + item.quantity, 0);
    cartCount.textContent = totalItems;
    
    // Update cart items
    if (cart.length === 0) {
      cartItems.innerHTML = `
        <div class="text-center py-8 text-gray-500">
          <i class="ri-shopping-cart-line text-4xl mb-2"></i>
          <p>Your cart is empty</p>
        </div>
      `;
      cartSubtotal.textContent = '₹0';
      return;
    }
    
    let itemsHTML = '';
    let subtotal = 0;
    
    cart.forEach(item => {
      const itemTotal = item.price * item.quantity;
      subtotal += itemTotal;
      
      itemsHTML += `
        <div class="flex items-center gap-3">
          <div class="w-16 h-16 bg-gray-200 rounded flex items-center justify-center">
            <i class="ri-headphone-line text-2xl text-gray-600"></i>
          </div>
          <div class="flex-grow">
            <h4 class="font-medium">${item.name}</h4>
            <p class="text-gray-500 text-sm">₹${item.price.toLocaleString('en-IN')}</p>
            <div class="flex items-center gap-2 mt-1">
              <div class="flex items-center border border-gray-200 rounded">
                <button class="decrease-item w-6 h-6 flex items-center justify-center text-gray-500 hover:bg-gray-100" data-id="${item.id}">
                  <i class="ri-subtract-line"></i>
                </button>
                <span class="quantity w-8 text-center">${item.quantity}</span>
                <button class="increase-item w-6 h-6 flex items-center justify-center text-gray-500 hover:bg-gray-100" data-id="${item.id}">
                  <i class="ri-add-line"></i>
                </button>
              </div>
              <button class="remove-item text-red-500 hover:text-red-600" data-id="${item.id}">
                <i class="ri-delete-bin-line"></i>
              </button>
            </div>
          </div>
        </div>
      `;
    });
    
    cartItems.innerHTML = itemsHTML;
    cartSubtotal.textContent = `₹${subtotal.toLocaleString('en-IN')}`;
    
    // Add event listeners for new buttons
    document.querySelectorAll('.decrease-item').forEach(button => {
      button.addEventListener('click', () => {
        const id = button.getAttribute('data-id');
        const item = cart.find(item => item.id === id);
        
        if (item.quantity > 1) {
          item.quantity -= 1;
        } else {
          cart = cart.filter(item => item.id !== id);
        }
        
        updateCart();
      });
    });
    
    document.querySelectorAll('.increase-item').forEach(button => {
      button.addEventListener('click', () => {
        const id = button.getAttribute('data-id');
        const item = cart.find(item => item.id === id);
        item.quantity += 1;
        updateCart();
      });
    });
    
    document.querySelectorAll('.remove-item').forEach(button => {
      button.addEventListener('click', () => {
        const id = button.getAttribute('data-id');
        cart = cart.filter(item => item.id !== id);
        updateCart();
      });
    });
  }
  
  // Form submission
  loginForm.addEventListener('submit', (e) => {
    e.preventDefault();
    alert('Login functionality would be implemented here');
    loginModal.classList.add('hidden');
  });
  
  registerForm.addEventListener('submit', (e) => {
    e.preventDefault();
    alert('Registration functionality would be implemented here');
    loginModal.classList.add('hidden');
  });
  
  // Smooth scrolling for anchor links
  document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
      e.preventDefault();
      
      const target = document.querySelector(this.getAttribute('href'));
      if (target) {
        window.scrollTo({
          top: target.offsetTop - 80,
          behavior: 'smooth'
        });
        
        // Close mobile menu if open
        mobileMenu.classList.add('hidden');
      }
    });
  });
});
</script>
</body>
</html>