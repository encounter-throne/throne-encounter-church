<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Throne Encounter Church | Raising a Generation of Encounter</title>
    <meta name="description" content="A revival-driven church in Abuja, Nigeria raising men and women who carry the presence and power of God. Led by Apostle Praizx Oragba.">
    
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Tailwind Config -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        royal: {
                            900: '#0a0e27',
                            800: '#0f172a',
                            700: '#1e3a8a',
                            600: '#1e40af',
                        },
                        gold: {
                            400: '#fbbf24',
                            500: '#f59e0b',
                            600: '#d97706',
                        }
                    },
                    fontFamily: {
                        serif: ['Cinzel', 'serif'],
                        sans: ['Inter', 'sans-serif'],
                    },
                    animation: {
                        'float': 'float 6s ease-in-out infinite',
                        'shimmer': 'shimmer 2s linear infinite',
                        'fade-in-up': 'fadeInUp 0.8s ease-out forwards',
                        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-20px)' },
                        },
                        shimmer: {
                            '0%': { backgroundPosition: '-200% 0' },
                            '100%': backgroundPosition: '200% 0' },
                        fadeInUp: {
                            '0%': { opacity: '0', transform: 'translateY(30px)' },
                            '100%': { opacity: '1', transform: 'translateY(0)' },
                        }
                    }
                }
            }
        }
    </script>

    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>

    <style>
        /* Custom Styles */
        .text-gradient {
            background: linear-gradient(135deg, #fbbf24 0%, #f59e0b 50%, #d97706 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .gold-glow {
            box-shadow: 0 0 30px rgba(251, 191, 36, 0.3);
        }
        
        .hero-overlay {
            background: linear-gradient(135deg, rgba(10, 14, 39, 0.95) 0%, rgba(15, 23, 42, 0.8) 50%, rgba(30, 58, 138, 0.6) 100%);
        }
        
        .glass-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(251, 191, 36, 0.1);
        }
        
        .nav-scrolled {
            background: rgba(10, 14, 39, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(251, 191, 36, 0.2);
        }
        
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(251, 191, 36, 0.15);
        }
        
        .btn-primary {
            background: linear-gradient(135deg, #fbbf24 0%, #f59e0b 100%);
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(251, 191, 36, 0.4);
        }
        
        .section-reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease-out;
        }
        
        .section-reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 10px;
        }
        
        ::-webkit-scrollbar-track {
            background: #0a0e27;
        }
        
        ::-webkit-scrollbar-thumb {
            background: #f59e0b;
            border-radius: 5px;
        }
        
        .testimonial-card {
            background: linear-gradient(135deg, rgba(30, 58, 138, 0.1) 0%, rgba(251, 191, 36, 0.05) 100%);
        }
        
        /* Logo Animation */
        .logo-spin {
            animation: spin-slow 20s linear infinite;
        }
        
        @keyframes spin-slow {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .pastor-image-container {
            position: relative;
            overflow: hidden;
        }
        
        .pastor-image-container::before {
            content: '';
            position: absolute;
            inset: -10px;
            background: linear-gradient(135deg, #fbbf24 0%, #f59e0b 100%);
            opacity: 0.3;
            filter: blur(30px);
            z-index: -1;
            border-radius: 2rem;
        }
        
        .logo-glow {
            filter: drop-shadow(0 0 20px rgba(251, 191, 36, 0.5));
        }
    </style>
</head>
<body class="font-sans bg-white text-gray-800 overflow-x-hidden">

    <!-- Navigation -->
    <nav id="navbar" class="fixed w-full z-50 transition-all duration-300 bg-transparent py-4">
        <div class="container mx-auto px-6 flex justify-between items-center">
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-12 h-12 relative">
                    <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="The Throne Encounter Church Logo" class="w-full h-full object-contain logo-glow">
                </div>
                <div class="flex flex-col">
                    <span class="font-serif font-bold text-white text-lg leading-tight">The Throne</span>
                    <span class="text-gold-400 text-xs tracking-widest uppercase">Encounter Church</span>
                </div>
            </a>
            
            <div class="hidden md:flex items-center gap-8">
                <a href="#home" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Home</a>
                <a href="#about" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">About</a>
                <a href="#services" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Services</a>
                <a href="#sermons" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Sermons</a>
                <a href="#leadership" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Leadership</a>
                <a href="#events" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Events</a>
                <a href="#give" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Give</a>
                <a href="#contact" class="text-white hover:text-gold-400 transition-colors text-sm font-medium uppercase tracking-wider">Contact</a>
            </div>
            
            <button id="mobile-menu-btn" class="md:hidden text-white hover:text-gold-400 transition-colors">
                <i data-lucide="menu" class="w-8 h-8"></i>
            </button>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-royal-900 border-t border-gold-400/20 absolute w-full">
            <div class="flex flex-col p-6 gap-4">
                <a href="#home" class="text-white hover:text-gold-400 transition-colors py-2">Home</a>
                <a href="#about" class="text-white hover:text-gold-400 transition-colors py-2">About</a>
                <a href="#services" class="text-white hover:text-gold-400 transition-colors py-2">Services</a>
                <a href="#sermons" class="text-white hover:text-gold-400 transition-colors py-2">Sermons</a>
                <a href="#leadership" class="text-white hover:text-gold-400 transition-colors py-2">Leadership</a>
                <a href="#events" class="text-white hover:text-gold-400 transition-colors py-2">Events</a>
                <a href="#give" class="text-white hover:text-gold-400 transition-colors py-2">Give</a>
                <a href="#contact" class="text-white hover:text-gold-400 transition-colors py-2">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="relative min-h-screen flex items-center justify-center overflow-hidden">
        <!-- Background Image with Overlay -->
        <div class="absolute inset-0 z-0">
            <img src="https://images.unsplash.com/photo-1516450360452-9312f5e86fc7?w=1920&h=1080&fit=crop" alt="Worship Atmosphere" class="w-full h-full object-cover">
            <div class="hero-overlay absolute inset-0"></div>
        </div>
        
        <!-- Animated Particles -->
        <div class="absolute inset-0 z-0 opacity-30">
            <div class="absolute top-20 left-10 w-2 h-2 bg-gold-400 rounded-full animate-float"></div>
            <div class="absolute top-40 right-20 w-3 h-3 bg-gold-400 rounded-full animate-float" style="animation-delay: 1s;"></div>
            <div class="absolute bottom-32 left-1/4 w-2 h-2 bg-gold-400 rounded-full animate-float" style="animation-delay: 2s;"></div>
        </div>
        
        <div class="container mx-auto px-6 relative z-10 text-center pt-20">
            <div class="max-w-5xl mx-auto">
                <!-- Logo in Hero -->
                <div class="mb-8 flex justify-center section-reveal">
                    <div class="w-24 h-24 md:w-32 md:h-32 relative animate-pulse-slow">
                        <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="The Throne Encounter Church Logo" class="w-full h-full object-contain logo-glow">
                    </div>
                </div>
                
                <div class="inline-block mb-6 px-6 py-2 border border-gold-400/30 rounded-full bg-white/5 backdrop-blur-sm animate-fade-in-up">
                    <span class="text-gold-400 text-sm font-medium tracking-widest uppercase">Welcome to The Throne</span>
                </div>
                
                <h1 class="font-serif text-5xl md:text-7xl lg:text-8xl font-bold text-white mb-6 leading-tight animate-fade-in-up" style="animation-delay: 0.2s;">
                    ENCOUNTER GOD.<br>
                    <span class="text-gradient">DISCOVER PURPOSE.</span><br>
                    WALK IN POWER.
                </h1>
                
                <p class="text-xl md:text-2xl text-gray-300 mb-10 max-w-3xl mx-auto font-light animate-fade-in-up" style="animation-delay: 0.4s;">
                    A revival-driven church raising men and women who carry the presence and power of God.
                </p>
                
                <div class="flex flex-col sm:flex-row gap-4 justify-center items-center animate-fade-in-up" style="animation-delay: 0.6s;">
                    <a href="#services" class="btn-primary px-8 py-4 rounded-full text-royal-900 font-bold text-lg flex items-center gap-2 group">
                        Join Us This Sunday
                        <i data-lucide="arrow-right" class="w-5 h-5 group-hover:translate-x-1 transition-transform"></i>
                    </a>
                    <a href="#sermons" class="px-8 py-4 rounded-full border-2 border-white text-white font-bold text-lg hover:bg-white hover:text-royal-900 transition-all flex items-center gap-2">
                        <i data-lucide="play-circle" class="w-5 h-5"></i>
                        Watch Live
                    </a>
                    <a href="#give" class="px-8 py-4 rounded-full border-2 border-gold-400 text-gold-400 font-bold text-lg hover:bg-gold-400 hover:text-royal-900 transition-all flex items-center gap-2">
                        <i data-lucide="heart" class="w-5 h-5"></i>
                        Give Online
                    </a>
                </div>
            </div>
            
            <!-- Scroll Indicator -->
            <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
                <i data-lucide="chevron-down" class="w-8 h-8 text-gold-400"></i>
            </div>
        </div>
    </section>

    <!-- About Preview Section -->
    <section id="about" class="py-24 bg-white relative overflow-hidden">
        <div class="absolute top-0 right-0 w-96 h-96 bg-royal-900/5 rounded-full blur-3xl -translate-y-1/2 translate-x-1/2"></div>
        
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div class="section-reveal">
                    <div class="inline-block px-4 py-2 bg-royal-900/5 rounded-full mb-6">
                        <span class="text-royal-700 font-semibold text-sm uppercase tracking-wider">About Us</span>
                    </div>
                    <h2 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mb-6 leading-tight">
                        Not Just a Church,<br>
                        <span class="text-gradient">A Movement of Revival</span>
                    </h2>
                    <p class="text-gray-600 text-lg leading-relaxed mb-6">
                        The Throne Encounter Church is a prophetic and revival-centered ministry headquartered in Abuja, Nigeria. Our mission is to raise kingdom ambassadors through divine encounters, sound teaching, and supernatural empowerment.
                    </p>
                    <p class="text-gray-600 text-lg leading-relaxed mb-8">
                        We are committed to raising a generation that encounters God deeply and walks in kingdom authority, transforming lives and nations through the power of the Holy Spirit.
                    </p>
                    
                    <div class="grid grid-cols-2 gap-6 mb-8">
                        <div class="flex items-start gap-3">
                            <div class="w-10 h-10 rounded-full bg-gold-400/20 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="flame" class="w-5 h-5 text-gold-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-royal-900">Revival</h4>
                                <p class="text-sm text-gray-600">Spirit-filled atmosphere</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-10 h-10 rounded-full bg-gold-400/20 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="crown" class="w-5 h-5 text-gold-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-royal-900">Authority</h4>
                                <p class="text-sm text-gray-600">Kingdom dominion</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-10 h-10 rounded-full bg-gold-400/20 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="book-open" class="w-5 h-5 text-gold-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-royal-900">Truth</h4>
                                <p class="text-sm text-gray-600">Sound doctrine</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-3">
                            <div class="w-10 h-10 rounded-full bg-gold-400/20 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="users" class="w-5 h-5 text-gold-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-royal-900">Community</h4>
                                <p class="text-sm text-gray-600">Family of faith</p>
                            </div>
                        </div>
                    </div>
                    
                    <a href="#vision" class="inline-flex items-center gap-2 text-royal-700 font-bold hover:text-gold-600 transition-colors group">
                        Learn More About Our Vision
                        <i data-lucide="arrow-right" class="w-5 h-5 group-hover:translate-x-1 transition-transform"></i>
                    </a>
                </div>
                
                <div class="section-reveal relative">
                    <div class="relative rounded-2xl overflow-hidden shadow-2xl">
                        <img src="https://images.unsplash.com/photo-1548625149-fc4a29cf7092?w=800&h=1000&fit=crop" alt="Church Community" class="w-full h-auto object-cover">
                        <div class="absolute inset-0 bg-gradient-to-t from-royal-900/80 to-transparent"></div>
                        <div class="absolute bottom-8 left-8 right-8">
                            <div class="glass-card p-6 rounded-xl flex items-center gap-4">
                                <div class="w-16 h-16 rounded-full overflow-hidden border-2 border-gold-400 flex-shrink-0">
                                    <img src="/mnt/kimi/upload/RED SUIT 1.png" alt="Apostle Praizx Oragba" class="w-full h-full object-cover">
                                </div>
                                <div>
                                    <p class="text-white font-serif text-lg italic">"Raising a Generation of Encounter"</p>
                                    <p class="text-gold-400 text-sm mt-1">— Apostle Praizx Oragba</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- Decorative Element -->
                    <div class="absolute -z-10 -bottom-10 -right-10 w-64 h-64 border-2 border-gold-400/30 rounded-2xl"></div>
                    
                    <!-- Floating Logo Element -->
                    <div class="absolute -top-6 -right-6 w-20 h-20 bg-white rounded-full shadow-xl p-3 animate-float">
                        <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="Logo" class="w-full h-full object-contain">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Weekly Services Section -->
    <section id="services" class="py-24 bg-royal-900 relative overflow-hidden">
        <div class="absolute inset-0 opacity-10">
            <div class="absolute inset-0" style="background-image: radial-gradient(circle at 2px 2px, rgba(251,191,36,0.3) 1px, transparent 0); background-size: 40px 40px;"></div>
        </div>
        
        <div class="container mx-auto px-6 relative z-10">
            <div class="text-center mb-16 section-reveal">
                <span class="text-gold-400 font-semibold text-sm uppercase tracking-widest">Join Us</span>
                <h2 class="font-serif text-4xl md:text-5xl font-bold text-white mt-4 mb-6">Weekly Services</h2>
                <p class="text-gray-400 text-lg max-w-2xl mx-auto">Experience the power of God's presence in our transformative weekly gatherings</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Sunday Morning -->
                <div class="service-card glass-card p-8 rounded-2xl transition-all duration-300 section-reveal">
                    <div class="w-14 h-14 bg-gold-400/20 rounded-full flex items-center justify-center mb-6">
                        <i data-lucide="sun" class="w-7 h-7 text-gold-400"></i>
                    </div>
                    <h3 class="font-serif text-2xl font-bold text-white mb-2">Sunday Worship</h3>
                    <p class="text-gold-400 font-semibold mb-4">School of the Spirit</p>
                    <div class="space-y-3 text-gray-300">
                        <div class="flex items-center gap-3">
                            <i data-lucide="clock" class="w-5 h-5 text-gold-400"></i>
                            <span>9:00 AM</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <i data-lucide="map-pin" class="w-5 h-5 text-gold-400"></i>
                            <span>Main Sanctuary</span>
                        </div>
                    </div>
                    <div class="mt-6 pt-6 border-t border-white/10">
                        <span class="text-sm text-gray-400">Deep biblical teaching and spiritual formation</span>
                    </div>
                </div>
                
                <!-- Sunday Evening -->
                <div class="service-card glass-card p-8 rounded-2xl transition-all duration-300 section-reveal border-2 border-gold-400/30 relative">
                    <div class="absolute -top-4 left-1/2 transform -translate-x-1/2 bg-gold-400 text-royal-900 px-4 py-1 rounded-full text-sm font-bold flex items-center gap-2">
                        <i data-lucide="star" class="w-4 h-4 fill-current"></i>
                        Popular
                    </div>
                    <div class="w-14 h-14 bg-gold-400/20 rounded-full flex items-center justify-center mb-6">
                        <i data-lucide="sparkles" class="w-7 h-7 text-gold-400"></i>
                    </div>
                    <h3 class="font-serif text-2xl font-bold text-white mb-2">Sunday Evening</h3>
                    <p class="text-gold-400 font-semibold mb-4">Worship & Prophetic</p>
                    <div class="space-y-3 text-gray-300">
                        <div class="flex items-center gap-3">
                            <i data-lucide="clock" class="w-5 h-5 text-gold-400"></i>
                            <span>4:00 PM</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <i data-lucide="map-pin" class="w-5 h-5 text-gold-400"></i>
                            <span>Main Sanctuary</span>
                        </div>
                    </div>
                    <div class="mt-6 pt-6 border-t border-white/10">
                        <span class="text-sm text-gray-400">Intense worship and prophetic ministry</span>
                    </div>
                </div>
                
                <!-- Thursday Midweek -->
                <div class="service-card glass-card p-8 rounded-2xl transition-all duration-300 section-reveal">
                    <div class="w-14 h-14 bg-gold-400/20 rounded-full flex items-center justify-center mb-6">
                        <i data-lucide="flame" class="w-7 h-7 text-gold-400"></i>
                    </div>
                    <h3 class="font-serif text-2xl font-bold text-white mb-2">Thursday Encounter</h3>
                    <p class="text-gold-400 font-semibold mb-4">Moment of Encounter</p>
                    <div class="space-y-3 text-gray-300">
                        <div class="flex items-center gap-3">
                            <i data-lucide="clock" class="w-5 h-5 text-gold-400"></i>
                            <span>5:00 PM</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <i data-lucide="map-pin" class="w-5 h-5 text-gold-400"></i>
                            <span>Prayer Arena</span>
                        </div>
                    </div>
                    <div class="mt-6 pt-6 border-t border-white/10">
                        <span class="text-sm text-gray-400">Midweek spiritual refreshing and prayer</span>
                    </div>
                </div>
                
                <!-- Night of Theophany -->
                <div class="service-card glass-card p-8 rounded-2xl transition-all duration-300 section-reveal lg:col-span-2">
                    <div class="flex flex-col md:flex-row md:items-center gap-6">
                        <div class="w-14 h-14 bg-gold-400/20 rounded-full flex items-center justify-center flex-shrink-0">
                            <i data-lucide="moon" class="w-7 h-7 text-gold-400"></i>
                        </div>
                        <div class="flex-1">
                            <h3 class="font-serif text-2xl font-bold text-white mb-2">Night of Theophany</h3>
                            <p class="text-gold-400 font-semibold mb-2">Special Prophetic Night</p>
                            <p class="text-gray-400 text-sm mb-4">Last Friday of every month - Experience the manifest presence of God</p>
                        </div>
                        <div class="flex items-center gap-3 text-gray-300 bg-white/5 px-6 py-3 rounded-full">
                            <i data-lucide="clock" class="w-5 h-5 text-gold-400"></i>
                            <span class="font-semibold">9:00 PM</span>
                        </div>
                    </div>
                </div>
                
                <!-- Prayer & Fasting -->
                <div class="service-card glass-card p-8 rounded-2xl transition-all duration-300 section-reveal">
                    <div class="w-14 h-14 bg-gold-400/20 rounded-full flex items-center justify-center mb-6">
                        <i data-lucide="shield" class="w-7 h-7 text-gold-400"></i>
                    </div>
                    <h3 class="font-serif text-2xl font-bold text-white mb-2">Prayer & Fasting</h3>
                    <p class="text-gold-400 font-semibold mb-4">Weekly & Quarterly</p>
                    <div class="space-y-3 text-gray-300">
                        <div class="flex items-center gap-3">
                            <i data-lucide="calendar" class="w-5 h-5 text-gold-400"></i>
                            <span>Every Wednesday</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <i data-lucide="calendar" class="w-5 h-5 text-gold-400"></i>
                            <span>Quarterly Retreats</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 text-center section-reveal">
                <div class="inline-flex items-center gap-2 text-gold-400 bg-gold-400/10 px-6 py-3 rounded-full">
                    <i data-lucide="map-pin" class="w-5 h-5"></i>
                    <span class="font-semibold">Before FCT Unity Home, By Gwako U-Turn, Gwako Gwagwalada-Abuja, Nigeria</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Latest Sermons Section -->
    <section id="sermons" class="py-24 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between items-end mb-16 section-reveal">
                <div>
                    <span class="text-royal-700 font-semibold text-sm uppercase tracking-widest">Media</span>
                    <h2 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mt-4">Experience the Word<br>with Power</h2>
                </div>
                <a href="#" class="mt-6 md:mt-0 inline-flex items-center gap-2 text-royal-700 font-bold hover:text-gold-600 transition-colors">
                    View All Messages
                    <i data-lucide="arrow-right" class="w-5 h-5"></i>
                </a>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Sermon 1 -->
                <div class="group bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition-all duration-300 section-reveal">
                    <div class="relative aspect-video overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1445445290350-18a3b86e0b5a?w=800&h=450&fit=crop" alt="Sermon" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-black/40 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity">
                            <button class="w-16 h-16 bg-gold-400 rounded-full flex items-center justify-center text-royal-900 hover:scale-110 transition-transform">
                                <i data-lucide="play" class="w-8 h-8 fill-current"></i>
                            </button>
                        </div>
                        <div class="absolute bottom-4 right-4 bg-black/70 text-white px-3 py-1 rounded-full text-sm">
                            45:32
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center gap-2 text-sm text-gray-500 mb-3">
                            <span class="px-3 py-1 bg-royal-900/5 rounded-full text-royal-700 font-medium">Revival Series</span>
                            <span>Mar 2, 2026</span>
                        </div>
                        <h3 class="font-serif text-xl font-bold text-royal-900 mb-2 group-hover:text-gold-600 transition-colors">The Throne Room Authority</h3>
                        <p class="text-gray-600 text-sm mb-4">Discovering your seat of authority in Christ and walking in kingdom dominion.</p>
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 rounded-full overflow-hidden border-2 border-gold-400">
                                <img src="/mnt/kimi/upload/RED SUIT 1.png" alt="Apostle Praizx Oragba" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <p class="font-semibold text-royal-900 text-sm">Apostle Praizx Oragba</p>
                                <p class="text-xs text-gray-500">Global Lead Pastor</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Sermon 2 -->
                <div class="group bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition-all duration-300 section-reveal">
                    <div class="relative aspect-video overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1504052434569-70ad5836ab65?w=800&h=450&fit=crop" alt="Sermon" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-black/40 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity">
                            <button class="w-16 h-16 bg-gold-400 rounded-full flex items-center justify-center text-royal-900 hover:scale-110 transition-transform">
                                <i data-lucide="play" class="w-8 h-8 fill-current"></i>
                            </button>
                        </div>
                        <div class="absolute bottom-4 right-4 bg-black/70 text-white px-3 py-1 rounded-full text-sm">
                            52:15
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center gap-2 text-sm text-gray-500 mb-3">
                            <span class="px-3 py-1 bg-royal-900/5 rounded-full text-royal-700 font-medium">Financial Breakthrough</span>
                            <span>Feb 28, 2026</span>
                        </div>
                        <h3 class="font-serif text-xl font-bold text-royal-900 mb-2 group-hover:text-gold-600 transition-colors">Keys to Kingdom Prosperity</h3>
                        <p class="text-gray-600 text-sm mb-4">Understanding biblical principles for financial breakthrough and wealth creation.</p>
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 rounded-full overflow-hidden border-2 border-gold-400">
                                <img src="/mnt/kimi/upload/RED SUIT 1.png" alt="Apostle Praizx Oragba" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <p class="font-semibold text-royal-900 text-sm">Apostle Praizx Oragba</p>
                                <p class="text-xs text-gray-500">Global Lead Pastor</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Sermon 3 -->
                <div class="group bg-white rounded-2xl overflow-hidden shadow-lg hover:shadow-2xl transition-all duration-300 section-reveal">
                    <div class="relative aspect-video overflow-hidden">
                        <img src="https://images.unsplash.com/photo-1519834785169-98be25ec3f84?w=800&h=450&fit=crop" alt="Sermon" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-black/40 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity">
                            <button class="w-16 h-16 bg-gold-400 rounded-full flex items-center justify-center text-royal-900 hover:scale-110 transition-transform">
                                <i data-lucide="play" class="w-8 h-8 fill-current"></i>
                            </button>
                        </div>
                        <div class="absolute bottom-4 right-4 bg-black/70 text-white px-3 py-1 rounded-full text-sm">
                            38:45
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex items-center gap-2 text-sm text-gray-500 mb-3">
                            <span class="px-3 py-1 bg-royal-900/5 rounded-full text-royal-700 font-medium">Prophetic</span>
                            <span>Feb 23, 2026</span>
                        </div>
                        <h3 class="font-serif text-xl font-bold text-royal-900 mb-2 group-hover:text-gold-600 transition-colors">Hearing God's Voice Clearly</h3>
                        <p class="text-gray-600 text-sm mb-4">Developing sensitivity to the Holy Spirit and walking in prophetic accuracy.</p>
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 rounded-full overflow-hidden border-2 border-gold-400">
                                <img src="/mnt/kimi/upload/RED SUIT 1.png" alt="Apostle Praizx Oragba" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <p class="font-semibold text-royal-900 text-sm">Apostle Praizx Oragba</p>
                                <p class="text-xs text-gray-500">Global Lead Pastor</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Live Stream Banner -->
            <div class="mt-16 bg-royal-900 rounded-3xl p-8 md:p-12 relative overflow-hidden section-reveal">
                <div class="absolute inset-0 opacity-20">
                    <img src="https://images.unsplash.com/photo-1516450360452-9312f5e86fc7?w=1200&h=400&fit=crop" class="w-full h-full object-cover">
                </div>
                <div class="relative z-10 flex flex-col md:flex-row items-center justify-between gap-8">
                    <div class="text-center md:text-left">
                        <div class="inline-flex items-center gap-2 text-red-400 font-bold mb-4 animate-pulse">
                            <span class="w-3 h-3 bg-red-500 rounded-full"></span>
                            LIVE EVERY SUNDAY
                        </div>
                        <h3 class="font-serif text-3xl md:text-4xl font-bold text-white mb-2">Join Our Live Stream</h3>
                        <p class="text-gray-300">Can't make it in person? Experience the power online</p>
                    </div>
                    <div class="flex gap-4">
                        <button class="btn-primary px-8 py-4 rounded-full text-royal-900 font-bold flex items-center gap-2">
                            <i data-lucide="youtube" class="w-5 h-5"></i>
                            YouTube
                        </button>
                        <button class="px-8 py-4 rounded-full border-2 border-white text-white font-bold hover:bg-white hover:text-royal-900 transition-all flex items-center gap-2">
                            <i data-lucide="facebook" class="w-5 h-5"></i>
                            Facebook
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Leadership Section -->
    <section id="leadership" class="py-24 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16 section-reveal">
                <span class="text-royal-700 font-semibold text-sm uppercase tracking-widest">Leadership</span>
                <h2 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mt-4">Apostolic Leadership</h2>
            </div>
            
            <div class="max-w-6xl mx-auto">
                <div class="grid md:grid-cols-2 gap-16 items-center section-reveal">
                    <div class="relative pastor-image-container">
                        <div class="aspect-[3/4] rounded-2xl overflow-hidden shadow-2xl border-4 border-gold-400/30">
                            <img src="/mnt/kimi/upload/RED SUIT 1.png" alt="Apostle Praizx Oragba - Global Lead Pastor of The Throne Encounter Church" class="w-full h-full object-cover object-top hover:scale-105 transition-transform duration-700">
                        </div>
                        
                        <!-- Decorative Elements -->
                        <div class="absolute -bottom-6 -right-6 w-48 h-48 bg-gold-400/20 rounded-full blur-3xl"></div>
                        <div class="absolute -top-6 -left-6 w-32 h-32 border-2 border-gold-400/30 rounded-2xl"></div>
                        <div class="absolute -bottom-4 -left-4 w-24 h-24 bg-royal-900 rounded-full flex items-center justify-center shadow-xl">
                            <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="Logo" class="w-16 h-16 object-contain">
                        </div>
                        
                        <!-- Badge -->
                        <div class="absolute top-6 right-6 bg-gold-400 text-royal-900 px-4 py-2 rounded-full font-bold text-sm shadow-lg flex items-center gap-2">
                            <i data-lucide="crown" class="w-4 h-4"></i>
                            Global Lead Pastor
                        </div>
                    </div>
                    
                    <div>
                        <div class="inline-block px-4 py-2 bg-gold-400/10 rounded-full mb-6">
                            <span class="text-gold-600 font-bold text-sm uppercase tracking-wider">Global Lead Pastor</span>
                        </div>
                        <h3 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mb-4">Apostle Praizx Oragba</h3>
                        <p class="text-xl text-gray-600 mb-6 italic font-light border-l-4 border-gold-400 pl-6">"Raising a generation that encounters God deeply and walks in kingdom authority."</p>
                        
                        <div class="space-y-4 text-gray-600 mb-8 text-lg leading-relaxed">
                            <p>Apostle Praizx Oragba is a prophetic voice and revivalist with a mandate to raise a generation that encounters God deeply. With a strong emphasis on spiritual intelligence, kingdom authority, and supernatural empowerment, he leads The Throne Encounter Church with vision and passion.</p>
                            <p>His ministry is characterized by powerful teaching, prophetic insight, and a demonstration of the Holy Spirit's power. He is committed to raising kingdom ambassadors who will influence every sphere of society.</p>
                            <p>Apostle Praizx is happily married and blessed with children, and together with his family, they exemplify kingdom values and excellence.</p>
                        </div>
                        
                        <div class="flex flex-wrap gap-4 mb-8">
                            <div class="flex items-center gap-2 px-4 py-2 bg-royal-900/5 rounded-full">
                                <i data-lucide="book-open" class="w-5 h-5 text-gold-600"></i>
                                <span class="text-royal-900 font-semibold">Teacher</span>
                            </div>
                            <div class="flex items-center gap-2 px-4 py-2 bg-royal-900/5 rounded-full">
                                <i data-lucide="flame" class="w-5 h-5 text-gold-600"></i>
                                <span class="text-royal-900 font-semibold">Revivalist</span>
                            </div>
                            <div class="flex items-center gap-2 px-4 py-2 bg-royal-900/5 rounded-full">
                                <i data-lucide="eye" class="w-5 h-5 text-gold-600"></i>
                                <span class="text-royal-900 font-semibold">Prophetic Voice</span>
                            </div>
                        </div>
                        
                        <div class="flex gap-4">
                            <a href="#" class="w-12 h-12 rounded-full bg-royal-900 text-white flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all transform hover:scale-110">
                                <i data-lucide="facebook" class="w-5 h-5"></i>
                            </a>
                            <a href="#" class="w-12 h-12 rounded-full bg-royal-900 text-white flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all transform hover:scale-110">
                                <i data-lucide="instagram" class="w-5 h-5"></i>
                            </a>
                            <a href="#" class="w-12 h-12 rounded-full bg-royal-900 text-white flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all transform hover:scale-110">
                                <i data-lucide="twitter" class="w-5 h-5"></i>
                            </a>
                            <a href="#" class="w-12 h-12 rounded-full bg-royal-900 text-white flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all transform hover:scale-110">
                                <i data-lucide="youtube" class="w-5 h-5"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Ministries Section -->
    <section class="py-24 bg-royal-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16 section-reveal">
                <span class="text-royal-700 font-semibold text-sm uppercase tracking-widest">Get Involved</span>
                <h2 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mt-4">Our Ministries</h2>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">Find your place in our community and grow in your calling</p>
            </div>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="users" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Youth & Young Adults</h3>
                    <p class="text-gray-600 text-sm">Raising fiery young leaders equipped for kingdom impact</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="hand" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Prayer & Intercession</h3>
                    <p class="text-gray-600 text-sm">Maintaining the fire on the altar through continuous prayer</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="video" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Media & Creative</h3>
                    <p class="text-gray-600 text-sm">Excellence in multimedia, design, and creative arts</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="globe" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Outreach & Missions</h3>
                    <p class="text-gray-600 text-sm">Taking the gospel to the ends of the earth</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="smile" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Children's Church</h3>
                    <p class="text-gray-600 text-sm">Nurturing the next generation in God's ways</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="mic" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Technical & Sound</h3>
                    <p class="text-gray-600 text-sm">Excellence in audio, lighting, and technical production</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="shield" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Men of Encounter</h3>
                    <p class="text-gray-600 text-sm">Building mighty men of valor and integrity</p>
                </div>
                
                <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:-translate-y-2 section-reveal">
                    <div class="w-14 h-14 bg-royal-900 rounded-2xl flex items-center justify-center text-gold-400 mb-6 group-hover:scale-110 transition-transform">
                        <i data-lucide="heart" class="w-7 h-7"></i>
                    </div>
                    <h3 class="font-serif text-xl font-bold text-royal-900 mb-2">Women of Destiny</h3>
                    <p class="text-gray-600 text-sm">Empowering women to fulfill their divine calling</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonies Section -->
    <section class="py-24 bg-royal-900 relative overflow-hidden">
        <div class="absolute inset-0 opacity-20">
            <div class="absolute inset-0" style="background-image: radial-gradient(circle at 2px 2px, rgba(251,191,36,0.3) 1px, transparent 0); background-size: 40px 40px;"></div>
        </div>
        
        <div class="container mx-auto px-6 relative z-10">
            <div class="text-center mb-16 section-reveal">
                <span class="text-gold-400 font-semibold text-sm uppercase tracking-widest">Testimonies</span>
                <h2 class="font-serif text-4xl md:text-5xl font-bold text-white mt-4">Real Encounters.<br>Real Transformations.</h2>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="testimonial-card p-8 rounded-2xl border border-gold-400/20 section-reveal">
                    <div class="flex gap-1 mb-6">
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                    </div>
                    <p class="text-gray-300 mb-6 italic">"I came to The Throne Encounter Church broken and depressed. Through the powerful teachings and prayers, I encountered God's healing power. Today, I am completely restored and serving in the Media team!"</p>
                    <div class="flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-gold-400/20 flex items-center justify-center text-gold-400 font-bold">SC</div>
                        <div>
                            <p class="text-white font-semibold">Sister Chioma</p>
                            <p class="text-gold-400 text-sm">Healing & Restoration</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card p-8 rounded-2xl border border-gold-400/20 section-reveal">
                    <div class="flex gap-1 mb-6">
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                    </div>
                    <p class="text-gray-300 mb-6 italic">"After applying the kingdom prosperity principles taught here, my business that was struggling experienced a supernatural turnaround. I went from debt to financial abundance in 6 months!"</p>
                    <div class="flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-gold-400/20 flex items-center justify-center text-gold-400 font-bold">BE</div>
                        <div>
                            <p class="text-white font-semibold">Brother Emmanuel</p>
                            <p class="text-gold-400 text-sm">Financial Breakthrough</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card p-8 rounded-2xl border border-gold-400/20 section-reveal">
                    <div class="flex gap-1 mb-6">
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                        <i data-lucide="star" class="w-5 h-5 text-gold-400 fill-current"></i>
                    </div>
                    <p class="text-gray-300 mb-6 italic">"The Night of Theophany changed my life completely. I received a clear prophetic word about my career direction. Within three months, everything the man of God said came to pass. God is faithful!"</p>
                    <div class="flex items-center gap-4">
                        <div class="w-12 h-12 rounded-full bg-gold-400/20 flex items-center justify-center text-gold-400 font-bold">SA</div>
                        <div>
                            <p class="text-white font-semibold">Sister Ada</p>
                            <p class="text-gold-400 text-sm">Prophetic Direction</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Events Section -->
    <section id="events" class="py-24 bg-white">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between items-end mb-16 section-reveal">
                <div>
                    <span class="text-royal-700 font-semibold text-sm uppercase tracking-widest">Upcoming</span>
                    <h2 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mt-4">Events & Conferences</h2>
                </div>
                <a href="#" class="mt-6 md:mt-0 inline-flex items-center gap-2 text-royal-700 font-bold hover:text-gold-600 transition-colors">
                    View All Events
                    <i data-lucide="arrow-right" class="w-5 h-5"></i>
                </a>
            </div>
            
            <div class="space-y-6">
                <div class="group bg-gray-50 rounded-2xl p-6 md:p-8 flex flex-col md:flex-row gap-8 items-center hover:shadow-xl transition-all duration-300 section-reveal">
                    <div class="flex-shrink-0 text-center md:text-left">
                        <div class="w-20 h-20 bg-royal-900 rounded-2xl flex flex-col items-center justify-center text-white relative overflow-hidden">
                            <div class="absolute inset-0 opacity-20">
                                <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" class="w-full h-full object-contain">
                            </div>
                            <span class="text-2xl font-bold relative z-10">15</span>
                            <span class="text-xs uppercase relative z-10">MAR</span>
                        </div>
                    </div>
                    <div class="flex-1 text-center md:text-left">
                        <div class="flex flex-wrap gap-2 mb-3 justify-center md:justify-start">
                            <span class="px-3 py-1 bg-gold-400/20 text-gold-600 rounded-full text-sm font-semibold">Conference</span>
                            <span class="px-3 py-1 bg-royal-900/10 text-royal-700 rounded-full text-sm">9:00 AM</span>
                        </div>
                        <h3 class="font-serif text-2xl font-bold text-royal-900 mb-2 group-hover:text-gold-600 transition-colors">Kingdom Financial Summit 2026</h3>
                        <p class="text-gray-600 mb-4">A 3-day intensive on biblical wealth creation, financial intelligence, and kingdom prosperity.</p>
                        <div class="flex items-center gap-6 text-sm text-gray-500 justify-center md:justify-start">
                            <span class="flex items-center gap-2">
                                <i data-lucide="map-pin" class="w-4 h-4"></i>
                                Main Auditorium
                            </span>
                            <span class="flex items-center gap-2">
                                <i data-lucide="users" class="w-4 h-4"></i>
                                500+ Registered
                            </span>
                        </div>
                    </div>
                    <div class="flex-shrink-0">
                        <button class="px-6 py-3 bg-royal-900 text-white rounded-full font-semibold hover:bg-gold-400 hover:text-royal-900 transition-all">
                            Register Now
                        </button>
                    </div>
                </div>
                
                <div class="group bg-gray-50 rounded-2xl p-6 md:p-8 flex flex-col md:flex-row gap-8 items-center hover:shadow-xl transition-all duration-300 section-reveal">
                    <div class="flex-shrink-0 text-center md:text-left">
                        <div class="w-20 h-20 bg-royal-900 rounded-2xl flex flex-col items-center justify-center text-white relative overflow-hidden">
                            <div class="absolute inset-0 opacity-20">
                                <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" class="w-full h-full object-contain">
                            </div>
                            <span class="text-2xl font-bold relative z-10">28</span>
                            <span class="text-xs uppercase relative z-10">MAR</span>
                        </div>
                    </div>
                    <div class="flex-1 text-center md:text-left">
                        <div class="flex flex-wrap gap-2 mb-3 justify-center md:justify-start">
                            <span class="px-3 py-1 bg-gold-400/20 text-gold-600 rounded-full text-sm font-semibold">Special Service</span>
                            <span class="px-3 py-1 bg-royal-900/10 text-royal-700 rounded-full text-sm">9:00 PM</span>
                        </div>
                        <h3 class="font-serif text-2xl font-bold text-royal-900 mb-2 group-hover:text-gold-600 transition-colors">Night of Theophany</h3>
                        <p class="text-gray-600 mb-4">Monthly prophetic night of divine encounter, worship, and supernatural manifestations.</p>
                        <div class="flex items-center gap-6 text-sm text-gray-500 justify-center md:justify-start">
                            <span class="flex items-center gap-2">
                                <i data-lucide="map-pin" class="w-4 h-4"></i>
                                Prayer Arena
                            </span>
                            <span class="flex items-center gap-2">
                                <i data-lucide="clock" class="w-4 h-4"></i>
                                All Night
                            </span>
                        </div>
                    </div>
                    <div class="flex-shrink-0">
                        <button class="px-6 py-3 bg-royal-900 text-white rounded-full font-semibold hover:bg-gold-400 hover:text-royal-900 transition-all">
                            Register Now
                        </button>
                    </div>
                </div>
                
                <div class="group bg-gray-50 rounded-2xl p-6 md:p-8 flex flex-col md:flex-row gap-8 items-center hover:shadow-xl transition-all duration-300 section-reveal">
                    <div class="flex-shrink-0 text-center md:text-left">
                        <div class="w-20 h-20 bg-royal-900 rounded-2xl flex flex-col items-center justify-center text-white relative overflow-hidden">
                            <div class="absolute inset-0 opacity-20">
                                <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" class="w-full h-full object-contain">
                            </div>
                            <span class="text-2xl font-bold relative z-10">10</span>
                            <span class="text-xs uppercase relative z-10">APR</span>
                        </div>
                    </div>
                    <div class="flex-1 text-center md:text-left">
                        <div class="flex flex-wrap gap-2 mb-3 justify-center md:justify-start">
                            <span class="px-3 py-1 bg-gold-400/20 text-gold-600 rounded-full text-sm font-semibold">Retreat</span>
                            <span class="px-3 py-1 bg-royal-900/10 text-royal-700 rounded-full text-sm">3 Days</span>
                        </div>
                        <h3 class="font-serif text-2xl font-bold text-royal-900 mb-2 group-hover:text-gold-600 transition-colors">Q1 Encounter Retreat</h3>
                        <p class="text-gray-600 mb-4">Quarterly retreat for deep spiritual refreshing, fasting, and intensive prayer.</p>
                        <div class="flex items-center gap-6 text-sm text-gray-500 justify-center md:justify-start">
                            <span class="flex items-center gap-2">
                                <i data-lucide="map-pin" class="w-4 h-4"></i>
                                Retreat Center
                            </span>
                            <span class="flex items-center gap-2">
                                <i data-lucide="users" class="w-4 h-4"></i>
                                Registration Open
                            </span>
                        </div>
                    </div>
                    <div class="flex-shrink-0">
                        <button class="px-6 py-3 bg-royal-900 text-white rounded-full font-semibold hover:bg-gold-400 hover:text-royal-900 transition-all">
                            Register Now
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Give Section -->
    <section id="give" class="py-24 bg-royal-900 relative overflow-hidden">
        <div class="absolute inset-0">
            <img src="https://images.unsplash.com/photo-1532629345422-7515f3d16bb6?w=1920&h=1080&fit=crop" class="w-full h-full object-cover opacity-10">
        </div>
        
        <div class="container mx-auto px-6 relative z-10">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="section-reveal">
                    <div class="w-16 h-16 mb-6 opacity-50">
                        <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="Logo" class="w-full h-full object-contain">
                    </div>
                    <span class="text-gold-400 font-semibold text-sm uppercase tracking-widest">Partnership</span>
                    <h2 class="font-serif text-4xl md:text-5xl font-bold text-white mt-4 mb-6">Partner With<br>the Vision</h2>
                    <p class="text-gray-300 text-lg mb-8">Your giving enables us to spread the gospel, support community outreach, and build a place where lives are transformed by the power of God.</p>
                    
                    <div class="bg-white/5 backdrop-blur-sm rounded-2xl p-8 border border-gold-400/20 mb-8">
                        <i data-lucide="quote" class="w-10 h-10 text-gold-400 mb-4"></i>
                        <p class="text-white text-xl italic font-serif mb-4">"Give, and it shall be given unto you; good measure, pressed down, and shaken together, and running over..."</p>
                        <p class="text-gold-400">— Luke 6:38 (KJV)</p>
                    </div>
                    
                    <div class="space-y-4">
                        <div class="flex items-start gap-4">
                            <div class="w-6 h-6 rounded-full bg-gold-400 flex items-center justify-center flex-shrink-0 mt-1">
                                <i data-lucide="check" class="w-4 h-4 text-royal-900"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-bold">Secure Payments</h4>
                                <p class="text-gray-400 text-sm">Protected by industry-standard encryption</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-4">
                            <div class="w-6 h-6 rounded-full bg-gold-400 flex items-center justify-center flex-shrink-0 mt-1">
                                <i data-lucide="check" class="w-4 h-4 text-royal-900"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-bold">International Giving</h4>
                                <p class="text-gray-400 text-sm">Support from anywhere in the world</p>
                            </div>
                        </div>
                        <div class="flex items-start gap-4">
                            <div class="w-6 h-6 rounded-full bg-gold-400 flex items-center justify-center flex-shrink-0 mt-1">
                                <i data-lucide="check" class="w-4 h-4 text-royal-900"></i>
                            </div>
                            <div>
                                <h4 class="text-white font-bold">Tax Deductible</h4>
                                <p class="text-gray-400 text-sm">Receive receipts for your records</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="section-reveal">
                    <div class="bg-white rounded-3xl p-8 md:p-10 shadow-2xl">
                        <div class="flex items-center gap-4 mb-6">
                            <div class="w-12 h-12">
                                <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="Logo" class="w-full h-full object-contain">
                            </div>
                            <h3 class="font-serif text-2xl font-bold text-royal-900">Give Online</h3>
                        </div>
                        
                        <div class="grid grid-cols-2 gap-4 mb-8">
                            <button class="give-type-btn active px-4 py-3 rounded-xl border-2 border-royal-900 bg-royal-900 text-white font-semibold transition-all" data-type="tithe">
                                Tithes
                            </button>
                            <button class="give-type-btn px-4 py-3 rounded-xl border-2 border-gray-200 text-gray-600 font-semibold hover:border-royal-900 hover:text-royal-900 transition-all" data-type="offering">
                                Offerings
                            </button>
                            <button class="give-type-btn px-4 py-3 rounded-xl border-2 border-gray-200 text-gray-600 font-semibold hover:border-royal-900 hover:text-royal-900 transition-all" data-type="partnership">
                                Partnership
                            </button>
                            <button class="give-type-btn px-4 py-3 rounded-xl border-2 border-gray-200 text-gray-600 font-semibold hover:border-royal-900 hover:text-royal-900 transition-all" data-type="project">
                                Building Project
                            </button>
                        </div>
                        
                        <div class="mb-8">
                            <label class="block text-gray-700 font-semibold mb-3">Select Amount</label>
                            <div class="grid grid-cols-3 gap-3 mb-4">
                                <button class="amount-btn px-4 py-3 rounded-lg border-2 border-gray-200 hover:border-gold-400 hover:bg-gold-50 transition-all font-semibold text-royal-900">₦5,000</button>
                                <button class="amount-btn px-4 py-3 rounded-lg border-2 border-gray-200 hover:border-gold-400 hover:bg-gold-50 transition-all font-semibold text-royal-900">₦10,000</button>
                                <button class="amount-btn px-4 py-3 rounded-lg border-2 border-gray-200 hover:border-gold-400 hover:bg-gold-50 transition-all font-semibold text-royal-900">₦50,000</button>
                                <button class="amount-btn px-4 py-3 rounded-lg border-2 border-gray-200 hover:border-gold-400 hover:bg-gold-50 transition-all font-semibold text-royal-900">$50</button>
                                <button class="amount-btn px-4 py-3 rounded-lg border-2 border-gray-200 hover:border-gold-400 hover:bg-gold-50 transition-all font-semibold text-royal-900">$100</button>
                                <button class="amount-btn px-4 py-3 rounded-lg border-2 border-gray-200 hover:border-gold-400 hover:bg-gold-50 transition-all font-semibold text-royal-900">$500</button>
                            </div>
                            <input type="text" placeholder="Enter custom amount" class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors">
                        </div>
                        
                        <div class="space-y-4 mb-8">
                            <div class="flex items-center gap-3 p-4 rounded-xl border-2 border-gray-200 hover:border-gold-400 cursor-pointer transition-all">
                                <div class="w-20 h-8 bg-blue-600 rounded flex items-center justify-center text-white font-bold text-xs">Paystack</div>
                                <span class="font-semibold text-gray-700 flex-1">Pay with Paystack</span>
                                <div class="w-5 h-5 rounded-full border-2 border-gray-300"></div>
                            </div>
                            <div class="flex items-center gap-3 p-4 rounded-xl border-2 border-gray-200 hover:border-gold-400 cursor-pointer transition-all">
                                <div class="w-20 h-8 bg-orange-500 rounded flex items-center justify-center text-white font-bold text-xs">Flutterwave</div>
                                <span class="font-semibold text-gray-700 flex-1">Pay with Flutterwave</span>
                                <div class="w-5 h-5 rounded-full border-2 border-gray-300"></div>
                            </div>
                            <div class="flex items-center gap-3 p-4 rounded-xl border-2 border-gray-200 hover:border-gold-400 cursor-pointer transition-all">
                                <i data-lucide="credit-card" class="w-8 h-8 text-royal-900"></i>
                                <span class="font-semibold text-gray-700 flex-1">Credit/Debit Card</span>
                                <div class="w-5 h-5 rounded-full border-2 border-gray-300"></div>
                            </div>
                        </div>
                        
                        <button class="w-full btn-primary py-4 rounded-xl text-royal-900 font-bold text-lg flex items-center justify-center gap-2">
                            Proceed to Give
                            <i data-lucide="arrow-right" class="w-5 h-5"></i>
                        </button>
                        
                        <p class="text-center text-gray-500 text-sm mt-4">Secured by 256-bit SSL encryption</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16 section-reveal">
                <span class="text-royal-700 font-semibold text-sm uppercase tracking-widest">Connect</span>
                <h2 class="font-serif text-4xl md:text-5xl font-bold text-royal-900 mt-4">Get In Touch</h2>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">We'd love to hear from you. Send us a message or visit us this Sunday.</p>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-16">
                <div class="section-reveal">
                    <div class="bg-gray-50 rounded-3xl p-8 md:p-10">
                        <h3 class="font-serif text-2xl font-bold text-royal-900 mb-8">Send us a Message</h3>
                        
                        <form class="space-y-6">
                            <div class="grid md:grid-cols-2 gap-6">
                                <div>
                                    <label class="block text-gray-700 font-semibold mb-2">First Name</label>
                                    <input type="text" class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors" placeholder="John">
                                </div>
                                <div>
                                    <label class="block text-gray-700 font-semibold mb-2">Last Name</label>
                                    <input type="text" class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors" placeholder="Doe">
                                </div>
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 font-semibold mb-2">Email Address</label>
                                <input type="email" class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors" placeholder="john@example.com">
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 font-semibold mb-2">Phone Number</label>
                                <input type="tel" class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors" placeholder="+234 800 000 0000">
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 font-semibold mb-2">Message Type</label>
                                <select class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors">
                                    <option>General Inquiry</option>
                                    <option>Prayer Request</option>
                                    <option>Counseling</option>
                                    <option>Partnership</option>
                                    <option>Testimony</option>
                                </select>
                            </div>
                            
                            <div>
                                <label class="block text-gray-700 font-semibold mb-2">Your Message</label>
                                <textarea rows="4" class="w-full px-4 py-3 rounded-lg border-2 border-gray-200 focus:border-royal-900 focus:outline-none transition-colors" placeholder="How can we help you?"></textarea>
                            </div>
                            
                            <button type="submit" class="w-full bg-royal-900 text-white py-4 rounded-lg font-bold hover:bg-gold-400 hover:text-royal-900 transition-all flex items-center justify-center gap-2">
                                Send Message
                                <i data-lucide="send" class="w-5 h-5"></i>
                            </button>
                        </form>
                    </div>
                </div>
                
                <div class="section-reveal space-y-8">
                    <div class="bg-royal-900 rounded-3xl p-8 text-white relative overflow-hidden">
                        <div class="absolute top-0 right-0 w-32 h-32 opacity-10">
                            <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" class="w-full h-full object-contain">
                        </div>
                        
                        <h3 class="font-serif text-2xl font-bold mb-8 relative z-10">Contact Information</h3>
                        
                        <div class="space-y-6 relative z-10">
                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-gold-400/20 rounded-full flex items-center justify-center flex-shrink-0">
                                    <i data-lucide="map-pin" class="w-6 h-6 text-gold-400"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-lg mb-1">Location</h4>
                                    <p class="text-gray-300">Before FCT Unity Home,<br>By Gwako U-Turn,<br>Gwako Gwagwalada-Abuja, Nigeria</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-gold-400/20 rounded-full flex items-center justify-center flex-shrink-0">
                                    <i data-lucide="phone" class="w-6 h-6 text-gold-400"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-lg mb-1">Phone</h4>
                                    <p class="text-gray-300">+234 913 203 4550<br>+234 814 424 7545<br>+234 912 534 1755</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-gold-400/20 rounded-full flex items-center justify-center flex-shrink-0">
                                    <i data-lucide="mail" class="w-6 h-6 text-gold-400"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-lg mb-1">Email</h4>
                                    <p class="text-gray-300">info.tec@gmail.com</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-gold-400/20 rounded-full flex items-center justify-center flex-shrink-0">
                                    <i data-lucide="clock" class="w-6 h-6 text-gold-400"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold text-lg mb-1">Service Times</h4>
                                    <p class="text-gray-300">
                                        Sunday School: 9:00 AM<br>
                                        Sunday Worship: 4:00 PM<br>
                                        Thursday: 5:00 PM<br>
                                        Night of Theophany: Last Friday 9:00 PM
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Map Embed -->
                    <div class="rounded-3xl overflow-hidden h-64 bg-gray-200 relative">
                        <iframe 
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3933.9!2d7.08!3d8.94!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zOMKwNTYnMjQuMCJOIDfCsDA0JzQ4LjAiRQ!5e0!3m2!1sen!2sng!4v1234567890"
                            width="100%" 
                            height="100%" 
                            style="border:0;" 
                            allowfullscreen="" 
                            loading="lazy"
                            class="absolute inset-0">
                        </iframe>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="py-16 bg-royal-900 relative overflow-hidden">
        <div class="absolute inset-0 opacity-5">
            <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" class="w-full h-full object-contain">
        </div>
        
        <div class="container mx-auto px-6 relative z-10">
            <div class="max-w-4xl mx-auto text-center section-reveal">
                <div class="w-16 h-16 mx-auto mb-6 opacity-30">
                    <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="Logo" class="w-full h-full object-contain">
                </div>
                <h3 class="font-serif text-3xl font-bold text-white mb-4">Stay Connected</h3>
                <p class="text-gray-300 mb-8">Subscribe to receive updates on upcoming events, sermons, and prophetic insights.</p>
                
                <form class="flex flex-col md:flex-row gap-4 max-w-2xl mx-auto">
                    <input type="email" placeholder="Enter your email address" class="flex-1 px-6 py-4 rounded-full border-2 border-white/20 bg-white/10 text-white placeholder-gray-400 focus:outline-none focus:border-gold-400 transition-colors">
                    <button type="submit" class="btn-primary px-8 py-4 rounded-full text-royal-900 font-bold flex items-center justify-center gap-2 whitespace-nowrap">
                        Subscribe
                        <i data-lucide="arrow-right" class="w-5 h-5"></i>
                    </button>
                </form>
                
                <p class="text-gray-400 text-sm mt-4">Join 5,000+ subscribers receiving weekly inspiration</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-royal-950 text-white pt-20 pb-8 border-t border-gold-400/20">
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-12 mb-16">
                <div>
                    <div class="flex items-center gap-3 mb-6">
                        <div class="w-12 h-12 relative">
                            <img src="/mnt/kimi/upload/A New Design (7) - Made with PosterMyWall.png" alt="The Throne Encounter Church Logo" class="w-full h-full object-contain">
                        </div>
                        <div>
                            <span class="font-serif font-bold text-xl block">The Throne</span>
                            <span class="text-gold-400 text-xs tracking-widest uppercase">Encounter Church</span>
                        </div>
                    </div>
                    <p class="text-gray-400 mb-6">Raising a generation of encounter. Transforming lives through divine presence and kingdom authority.</p>
                    <div class="flex gap-4">
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all">
                            <i data-lucide="facebook" class="w-5 h-5"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all">
                            <i data-lucide="instagram" class="w-5 h-5"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all">
                            <i data-lucide="twitter" class="w-5 h-5"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center hover:bg-gold-400 hover:text-royal-900 transition-all">
                            <i data-lucide="youtube" class="w-5 h-5"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="font-serif text-xl font-bold mb-6 text-gold-400">Quick Links</h4>
                    <ul class="space-y-3">
                        <li><a href="#about" class="text-gray-400 hover:text-white transition-colors">About Us</a></li>
                        <li><a href="#services" class="text-gray-400 hover:text-white transition-colors">Services</a></li>
                        <li><a href="#sermons" class="text-gray-400 hover:text-white transition-colors">Sermons</a></li>
                        <li><a href="#events" class="text-gray-400 hover:text-white transition-colors">Events</a></li>
                        <li><a href="#give" class="text-gray-400 hover:text-white transition-colors">Give Online</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-serif text-xl font-bold mb-6 text-gold-400">Resources</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Daily Devotional</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Prayer Requests</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Testimonies</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Blog</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Media Downloads</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-serif text-xl font-bold mb-6 text-gold-400">Service Times</h4>
                    <ul class="space-y-3 text-gray-400">
                        <li class="flex justify-between">
                            <span>Sunday School</span>
                            <span class="text-white">9:00 AM</span>
                        </li>
                        <li class="flex justify-between">
                            <span>Sunday Worship</span>
                            <span class="text-white">4:00 PM</span>
                        </li>
                        <li class="flex justify-between">
                            <span>Thursday</span>
                            <span class="text-white">5:00 PM</span>
                        </li>
                        <li class="flex justify-between">
                            <span>Night of Theophany</span>
                            <span class="text-white">9:00 PM</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-white/10 pt-8 flex flex-col md:flex-row justify-between items-center gap-4">
                <p class="text-gray-500 text-sm">© 2026 The Throne Encounter Church. All rights reserved.</p>
                <div class="flex gap-6 text-sm text-gray-500">
                    <a href="#" class="hover:text-white transition-colors">Privacy Policy</a>
                    <a href="#" class="hover:text-white transition-colors">Terms of Service</a>
                    <a href="#" class="hover:text-white transition-colors">Cookie Policy</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Initialize Lucide Icons
        lucide.createIcons();
        
        // Navigation Scroll Effect
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                navbar.classList.add('nav-scrolled');
                navbar.classList.remove('py-4');
                navbar.classList.add('py-2');
            } else {
                navbar.classList.remove('nav-scrolled');
                navbar.classList.remove('py-2');
                navbar.classList.add('py-4');
            }
        });
        
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Close mobile menu when clicking a link
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
        
        // Smooth Scroll for Navigation Links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
        
        // Intersection Observer for Scroll Animations
        const observerOptions = {
            root: null,
            rootMargin: '0px',
            threshold: 0.1
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                    observer.unobserve(entry.target);
                }
            });
        }, observerOptions);
        
        document.querySelectorAll('.section-reveal').forEach((el) => {
            observer.observe(el);
        });
        
        // Give Section Interaction
        const giveTypeBtns = document.querySelectorAll('.give-type-btn');
        giveTypeBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                giveTypeBtns.forEach(b => {
                    b.classList.remove('active', 'bg-royal-900', 'text-white', 'border-royal-900');
                    b.classList.add('border-gray-200', 'text-gray-600');
                });
                btn.classList.add('active', 'bg-royal-900', 'text-white', 'border-royal-900');
                btn.classList.remove('border-gray-200', 'text-gray-600');
            });
        });
        
        const amountBtns = document.querySelectorAll('.amount-btn');
        amountBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                amountBtns.forEach(b => {
                    b.classList.remove('border-gold-400', 'bg-gold-50');
                    b.classList.add('border-gray-200');
                });
                btn.classList.remove('border-gray-200');
                btn.classList.add('border-gold-400', 'bg-gold-50');
            });
        });
        
        // Form Submissions (Prevent default for demo)
        document.querySelectorAll('form').forEach(form => {
            form.addEventListener('submit', (e) => {
                e.preventDefault();
                alert('Thank you for your submission! This is a demo form.');
            });
        });
        
        // Add loading animation for buttons
        document.querySelectorAll('button').forEach(btn => {
            if (!btn.type || btn.type !== 'submit') {
                btn.addEventListener('click', function(e) {
                    if (this.textContent.includes('Register') || this.textContent.includes('Proceed')) {
                        const originalText = this.innerHTML;
                        this.innerHTML = '<i data-lucide="loader-2" class="w-5 h-5 animate-spin"></i> Processing...';
                        lucide.createIcons();
                        setTimeout(() => {
                            this.innerHTML = originalText;
                            lucide.createIcons();
                        }, 2000);
                    }
                });
            }
        });
    </script>
</body>
</html>
