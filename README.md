<!DOCTYPE html>
<html lang="en">
<head><script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-3170236932288677"
     crossorigin="anonymous"></script>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>J ENTERPRICES - Creative Digital Solutions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
        
        .gradient-bg {
            background: linear-gradient(-45deg, #667eea, #764ba2, #f093fb, #f5576c);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .floating {
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .card-3d {
            transform-style: preserve-3d;
            transition: all 0.3s ease;
        }
        
        .card-3d:hover {
            transform: rotateY(10deg) rotateX(10deg) scale(1.05);
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
        }
        
        .glass-nav {
            backdrop-filter: blur(10px);
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .bounce-emoji {
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        
        .pulse-button {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(102, 126, 234, 0.7); }
            70% { box-shadow: 0 0 0 10px rgba(102, 126, 234, 0); }
            100% { box-shadow: 0 0 0 0 rgba(102, 126, 234, 0); }
        }
        
        .chatbot {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
            animation: float 3s ease-in-out infinite;
        }
        
        .hidden-page {
            display: none;
        }
        
        .active-page {
            display: block;
        }
    </style>
</head>
<body class="bg-gray-900 text-white overflow-x-hidden">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 glass-nav">
        <div class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-bold text-white">
                    J ENTERPRICES <span class="bounce-emoji">🏢</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#" onclick="showPage('home')" class="nav-link text-white hover:text-purple-300 transition-colors">Home</a>
                    <a href="#" onclick="showPage('services')" class="nav-link text-white hover:text-purple-300 transition-colors">Services</a>
                    <a href="#" onclick="showPage('articles')" class="nav-link text-white hover:text-purple-300 transition-colors">Articles</a>
                    <a href="#" onclick="showPage('about')" class="nav-link text-white hover:text-purple-300 transition-colors">About</a>
                    <a href="#" onclick="showPage('contact')" class="nav-link text-white hover:text-purple-300 transition-colors">Contact</a>
                </div>
                <div class="md:hidden">
                    <button onclick="toggleMobileMenu()" class="text-white">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
            <div id="mobile-menu" class="hidden md:hidden mt-4 space-y-2">
                <a href="#" onclick="showPage('home')" class="block text-white hover:text-purple-300 transition-colors">Home</a>
                <a href="#" onclick="showPage('services')" class="block text-white hover:text-purple-300 transition-colors">Services</a>
                <a href="#" onclick="showPage('articles')" class="block text-white hover:text-purple-300 transition-colors">Articles</a>
                <a href="#" onclick="showPage('about')" class="block text-white hover:text-purple-300 transition-colors">About</a>
                <a href="#" onclick="showPage('contact')" class="block text-white hover:text-purple-300 transition-colors">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Page 1: Home -->
    <div id="home-page" class="active-page">
        <section class="min-h-screen gradient-bg flex items-center justify-center relative overflow-hidden">
            <div class="absolute inset-0 opacity-20">
                <div class="floating absolute top-20 left-10 text-6xl">💻</div>
                <div class="floating absolute top-40 right-20 text-4xl" style="animation-delay: 1s;">🎨</div>
                <div class="floating absolute bottom-40 left-20 text-5xl" style="animation-delay: 2s;">✨</div>
                <div class="floating absolute bottom-20 right-10 text-4xl" style="animation-delay: 0.5s;">🚀</div>
            </div>
            
            <div class="text-center z-10 px-6">
                <h1 class="text-6xl md:text-8xl font-bold mb-6 fade-in">
                    Welcome to <span class="text-yellow-300">J ENTERPRICES</span>
                </h1>
                <p class="text-xl md:text-2xl mb-4 fade-in" style="animation-delay: 0.3s;">
                    Your one-stop solution for creative and digital design services
                </p>
                <p class="text-lg mb-8 fade-in" style="animation-delay: 0.6s;">
                    Founded by <span class="text-purple-300 font-semibold">Jahangir Yousuf Kacher</span>
                </p>
                <button onclick="showPage('services')" class="bg-purple-600 hover:bg-purple-700 text-white font-bold py-4 px-8 rounded-full text-lg transition-all duration-300 transform hover:scale-105 pulse-button fade-in" style="animation-delay: 0.9s;">
                    Explore Our Services <span class="bounce-emoji ml-2">💼</span>
                </button>
            </div>
        </section>
    </div>

    <!-- Page 2: Services -->
    <div id="services-page" class="hidden-page">
        <section class="min-h-screen bg-gradient-to-br from-gray-900 via-purple-900 to-gray-900 pt-24 pb-12">
            <div class="container mx-auto px-6">
                <h1 class="text-5xl md:text-6xl font-bold text-center mb-16 fade-in">
                    Our Services <span class="bounce-emoji">🛠️</span>
                </h1>
                
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <div class="card-3d bg-gradient-to-br from-blue-600 to-purple-600 p-8 rounded-2xl fade-in">
                        <div class="text-6xl mb-4 floating">🌐</div>
                        <h3 class="text-2xl font-bold mb-4">Web Designing</h3>
                        <p class="text-gray-200">Modern, responsive websites that captivate your audience and drive results.</p>
                    </div>
                    
                    <div class="card-3d bg-gradient-to-br from-pink-600 to-red-600 p-8 rounded-2xl fade-in" style="animation-delay: 0.2s;">
                        <div class="text-6xl mb-4 floating" style="animation-delay: 1s;">🎨</div>
                        <h3 class="text-2xl font-bold mb-4">Graphic Designing</h3>
                        <p class="text-gray-200">Eye-catching graphics that tell your brand's story and engage customers.</p>
                    </div>
                    
                    <div class="card-3d bg-gradient-to-br from-green-600 to-teal-600 p-8 rounded-2xl fade-in" style="animation-delay: 0.4s;">
                        <div class="text-6xl mb-4 floating" style="animation-delay: 2s;">🖌️</div>
                        <h3 class="text-2xl font-bold mb-4">Logo Designing</h3>
                        <p class="text-gray-200">Memorable logos that represent your brand's identity and values.</p>
                    </div>
                    
                    <div class="card-3d bg-gradient-to-br from-yellow-600 to-orange-600 p-8 rounded-2xl fade-in" style="animation-delay: 0.6s;">
                        <div class="text-6xl mb-4 floating" style="animation-delay: 0.5s;">📸</div>
                        <h3 class="text-2xl font-bold mb-4">Social Media Graphics</h3>
                        <p class="text-gray-200">Stunning visuals that boost your social media presence and engagement.</p>
                    </div>
                    
                    <div class="card-3d bg-gradient-to-br from-indigo-600 to-purple-600 p-8 rounded-2xl fade-in" style="animation-delay: 0.8s;">
                        <div class="text-6xl mb-4 floating" style="animation-delay: 1.5s;">🧠</div>
                        <h3 class="text-2xl font-bold mb-4">AI-based Design Consulting</h3>
                        <p class="text-gray-200">Cutting-edge AI solutions to optimize your design strategy and workflow.</p>
                    </div>
                    
                    <div class="card-3d bg-gradient-to-br from-purple-600 to-pink-600 p-8 rounded-2xl fade-in" style="animation-delay: 1s;">
                        <div class="text-6xl mb-4 floating" style="animation-delay: 2.5s;">✨</div>
                        <h3 class="text-2xl font-bold mb-4">Creative Online Services</h3>
                        <p class="text-gray-200">Comprehensive digital solutions tailored to your unique business needs.</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Page 3: Articles -->
    <div id="articles-page" class="hidden-page">
        <section class="min-h-screen bg-gradient-to-br from-gray-900 via-blue-900 to-gray-900 pt-24 pb-12">
            <div class="container mx-auto px-6">
                <h1 class="text-5xl md:text-6xl font-bold text-center mb-16 fade-in">
                    Insights & Articles <span class="bounce-emoji">📚</span>
                </h1>
                
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <article class="bg-white bg-opacity-10 backdrop-blur-lg rounded-2xl overflow-hidden card-3d fade-in">
                        <div class="h-48 bg-gradient-to-br from-purple-500 to-pink-500 flex items-center justify-center">
                            <span class="text-6xl floating">🎯</span>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-3">Why Every Business Needs a Custom Logo</h3>
                            <p class="text-gray-300 mb-4">Discover how a well-designed logo can transform your brand identity and boost customer recognition...</p>
                            <span class="text-purple-300 text-sm">Design Tips • 5 min read</span>
                        </div>
                    </article>
                    
                    <article class="bg-white bg-opacity-10 backdrop-blur-lg rounded-2xl overflow-hidden card-3d fade-in" style="animation-delay: 0.2s;">
                        <div class="h-48 bg-gradient-to-br from-blue-500 to-teal-500 flex items-center justify-center">
                            <span class="text-6xl floating" style="animation-delay: 1s;">🚀</span>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-3">Top 5 Web Design Trends 2025</h3>
                            <p class="text-gray-300 mb-4">Stay ahead of the curve with the latest web design trends that will dominate the digital landscape...</p>
                            <span class="text-blue-300 text-sm">Web Design • 7 min read</span>
                        </div>
                    </article>
                    
                    <article class="bg-white bg-opacity-10 backdrop-blur-lg rounded-2xl overflow-hidden card-3d fade-in" style="animation-delay: 0.4s;">
                        <div class="h-48 bg-gradient-to-br from-green-500 to-yellow-500 flex items-center justify-center">
                            <span class="text-6xl floating" style="animation-delay: 2s;">🎨</span>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-3">The Psychology of Color in Branding</h3>
                            <p class="text-gray-300 mb-4">Learn how different colors influence customer behavior and how to choose the perfect palette...</p>
                            <span class="text-green-300 text-sm">Branding • 6 min read</span>
                        </div>
                    </article>
                </div>
            </div>
        </section>
    </div>

    <!-- Page 4: About -->
    <div id="about-page" class="hidden-page">
        <section class="min-h-screen bg-gradient-to-br from-gray-900 via-indigo-900 to-gray-900 pt-24 pb-12">
            <div class="container mx-auto px-6">
                <h1 class="text-5xl md:text-6xl font-bold text-center mb-16 fade-in">
                    Who We Are <span class="bounce-emoji">👥</span>
                </h1>
                
                <div class="max-w-4xl mx-auto">
                    <div class="bg-white bg-opacity-10 backdrop-blur-lg rounded-3xl p-8 md:p-12 card-3d fade-in">
                        <div class="text-center mb-8">
                            <div class="w-32 h-32 bg-gradient-to-br from-purple-500 to-pink-500 rounded-full mx-auto mb-6 flex items-center justify-center">
                                <span class="text-6xl floating">👨‍💼</span>
                            </div>
                            <h2 class="text-3xl font-bold mb-2">Jahangir Yousuf Kacher</h2>
                            <p class="text-purple-300 text-lg">Founder & Creative Director</p>
                        </div>
                        
                        <p class="text-lg text-center mb-8 leading-relaxed">
                            J ENTERPRICES is a design-forward company committed to helping brands stand out online. 
                            Founded by Jahangir Yousuf Kacher, our team specializes in bringing your vision to digital life 
                            through innovative design solutions and cutting-edge technology.
                        </p>
                        
                        <div class="grid md:grid-cols-3 gap-6 mt-12">
                            <div class="text-center fade-in" style="animation-delay: 0.2s;">
                                <div class="text-4xl mb-3 floating">🎯</div>
                                <h3 class="text-xl font-bold mb-2">Our Mission</h3>
                                <p class="text-gray-300">To empower businesses with exceptional design that drives growth and success.</p>
                            </div>
                            
                            <div class="text-center fade-in" style="animation-delay: 0.4s;">
                                <div class="text-4xl mb-3 floating" style="animation-delay: 1s;">💡</div>
                                <h3 class="text-xl font-bold mb-2">Our Vision</h3>
                                <p class="text-gray-300">To be the leading creative agency that transforms ideas into digital masterpieces.</p>
                            </div>
                            
                            <div class="text-center fade-in" style="animation-delay: 0.6s;">
                                <div class="text-4xl mb-3 floating" style="animation-delay: 2s;">⭐</div>
                                <h3 class="text-xl font-bold mb-2">Our Values</h3>
                                <p class="text-gray-300">Creativity, innovation, and client satisfaction are at the heart of everything we do.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Page 5: Contact -->
    <div id="contact-page" class="hidden-page">
        <section class="min-h-screen bg-gradient-to-br from-gray-900 via-purple-900 to-gray-900 pt-24 pb-12">
            <div class="container mx-auto px-6">
                <h1 class="text-5xl md:text-6xl font-bold text-center mb-16 fade-in">
                    Get In Touch <span class="bounce-emoji">📞</span>
                </h1>
                
                <div class="grid lg:grid-cols-2 gap-12 max-w-6xl mx-auto">
                    <div class="fade-in">
                        <div class="bg-white bg-opacity-10 backdrop-blur-lg rounded-3xl p-8 card-3d">
                            <h2 class="text-3xl font-bold mb-8 text-center">Contact Information</h2>
                            
                            <div class="space-y-6">
                                <div class="flex items-center space-x-4">
                                    <div class="w-12 h-12 bg-gradient-to-br from-blue-500 to-purple-500 rounded-full flex items-center justify-center floating">
                                        📞
                                    </div>
                                    <div>
                                        <h3 class="font-semibold">Phone</h3>
                                        <p class="text-gray-300">+91 9622102381</p>
                                    </div>
                                </div>
                                
                                <div class="flex items-center space-x-4">
                                    <div class="w-12 h-12 bg-gradient-to-br from-green-500 to-teal-500 rounded-full flex items-center justify-center floating" style="animation-delay: 1s;">
                                        📧
                                    </div>
                                    <div>
                                        <h3 class="font-semibold">Email</h3>
                                        <p class="text-gray-300">jahangirahmedkacher@gmail.com</p>
                                    </div>
                                </div>
                                
                                <div class="flex items-center space-x-4">
                                    <div class="w-12 h-12 bg-gradient-to-br from-pink-500 to-red-500 rounded-full flex items-center justify-center floating" style="animation-delay: 2s;">
                                        🏠
                                    </div>
                                    <div>
                                        <h3 class="font-semibold">Address</h3>
                                        <p class="text-gray-300">Office Garkhal Akhnoor<br>Jammu, Jammu & Kashmir, India</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="fade-in" style="animation-delay: 0.3s;">
                        <div class="bg-white bg-opacity-10 backdrop-blur-lg rounded-3xl p-8 card-3d">
                            <h2 class="text-3xl font-bold mb-8 text-center">Send Us a Message</h2>
                            
                            <form class="space-y-6" onsubmit="handleFormSubmit(event)">
                                <div>
                                    <label class="block text-sm font-medium mb-2">Name</label>
                                    <input type="text" required class="w-full px-4 py-3 bg-white bg-opacity-20 rounded-lg border border-white border-opacity-30 focus:outline-none focus:ring-2 focus:ring-purple-500 text-white placeholder-gray-300" placeholder="Your Name">
                                </div>
                                
                                <div>
                                    <label class="block text-sm font-medium mb-2">Email</label>
                                    <input type="email" required class="w-full px-4 py-3 bg-white bg-opacity-20 rounded-lg border border-white border-opacity-30 focus:outline-none focus:ring-2 focus:ring-purple-500 text-white placeholder-gray-300" placeholder="your@email.com">
                                </div>
                                
                                <div>
                                    <label class="block text-sm font-medium mb-2">Message</label>
                                    <textarea rows="4" required class="w-full px-4 py-3 bg-white bg-opacity-20 rounded-lg border border-white border-opacity-30 focus:outline-none focus:ring-2 focus:ring-purple-500 text-white placeholder-gray-300" placeholder="Tell us about your project..."></textarea>
                                </div>
                                
                                <button type="submit" class="w-full bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 text-white font-bold py-4 px-8 rounded-lg transition-all duration-300 transform hover:scale-105 pulse-button">
                                    Drop Us a Message <span class="bounce-emoji ml-2">📬</span>
                                </button>
                            </form>
                        </div>
                    </div>
                </div>
                
                <!-- Map Section -->
                <div class="mt-16 fade-in" style="animation-delay: 0.6s;">
                    <div class="bg-white bg-opacity-10 backdrop-blur-lg rounded-3xl p-8 card-3d">
                        <h2 class="text-3xl font-bold mb-8 text-center">Find Us Here <span class="bounce-emoji">📍</span></h2>
                        <div class="h-64 bg-gradient-to-br from-blue-500 to-purple-500 rounded-2xl flex items-center justify-center">
                            <div class="text-center">
                                <div class="text-6xl mb-4 floating">🗺️</div>
                                <p class="text-white text-lg">Interactive Map Coming Soon</p>
                                <p class="text-gray-200">Office Garkhal Akhnoor, Jammu, J&K</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- AI Chatbot -->
    <div class="chatbot">
        <button onclick="toggleChatbot()" class="bg-gradient-to-r from-purple-600 to-pink-600 hover:from-purple-700 hover:to-pink-700 text-white p-4 rounded-full shadow-lg transition-all duration-300 transform hover:scale-110">
            <span class="text-2xl">🤖</span>
        </button>
    </div>

    <!-- Chatbot Modal -->
    <div id="chatbot-modal" class="fixed inset-0 bg-black bg-opacity-50 z-50 hidden flex items-center justify-center p-4">
        <div class="bg-white bg-opacity-10 backdrop-blur-lg rounded-3xl p-8 max-w-md w-full">
            <div class="flex justify-between items-center mb-6">
                <h3 class="text-2xl font-bold text-white">AI Assistant <span class="bounce-emoji">🤖</span></h3>
                <button onclick="toggleChatbot()" class="text-white hover:text-gray-300">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                    </svg>
                </button>
            </div>
            <div class="text-center text-white">
                <div class="text-6xl mb-4 floating">💬</div>
                <p class="mb-4">Hi! I'm your AI assistant. I'm here to help you with any questions about our services.</p>
                <p class="text-sm text-gray-300 mb-6">This is a demo version. For full AI integration, we can implement Chatbase, Kommunicate, or Botpress.</p>
                <button class="bg-purple-600 hover:bg-purple-700 text-white px-6 py-3 rounded-lg transition-colors">
                    Start Conversation ✨
                </button>
            </div>
        </div>
    </div>

    <script>
        // Page Navigation
        function showPage(pageId) {
            // Hide all pages
            const pages = ['home', 'services', 'articles', 'about', 'contact'];
            pages.forEach(page => {
                const element = document.getElementById(page + '-page');
                if (element) {
                    element.classList.remove('active-page');
                    element.classList.add('hidden-page');
                }
            });
            
            // Show selected page
            const targetPage = document.getElementById(pageId + '-page');
            if (targetPage) {
                targetPage.classList.remove('hidden-page');
                targetPage.classList.add('active-page');
            }
            
            // Close mobile menu
            document.getElementById('mobile-menu').classList.add('hidden');
            
            // Trigger fade-in animations
            setTimeout(() => {
                const fadeElements = targetPage.querySelectorAll('.fade-in');
                fadeElements.forEach(el => el.classList.add('visible'));
            }, 100);
        }

        // Mobile Menu Toggle
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        }

        // Chatbot Toggle
        function toggleChatbot() {
            const modal = document.getElementById('chatbot-modal');
            modal.classList.toggle('hidden');
        }

        // Form Submission
        function handleFormSubmit(event) {
            event.preventDefault();
            alert('Thank you for your message! This is a demo form. In the live version, this would send your message to J ENTERPRICES.');
        }

        // Initialize fade-in animations on page load
        document.addEventListener('DOMContentLoaded', function() {
            setTimeout(() => {
                const fadeElements = document.querySelectorAll('#home-page .fade-in');
                fadeElements.forEach(el => el.classList.add('visible'));
            }, 500);
        });

        // Scroll animations for other pages
        function observeElements() {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            });

            document.querySelectorAll('.fade-in').forEach(el => {
                observer.observe(el);
            });
        }

        // Initialize observers
        document.addEventListener('DOMContentLoaded', observeElements);
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'96ce0c1c74e081ea',t:'MTc1NDgxMzc0Ny4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
