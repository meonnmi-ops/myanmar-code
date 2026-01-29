<!DOCTYPE html>
<html lang="my">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="မြန်မာဘာသာဖြင့် ပရိုဂရမ်းမင်းရေးသားနိုင်သော ပလက်ဖောင်း - Myanmar Code Programming Language">
    <meta name="keywords" content="မြန်မာကုဒ်, Myanmar Code, programming, ပရိုဂရမ်းမင်း, programming language, Myanmar">
    <meta name="author" content="AMO MASTER 221922 Team">
    
    <title>မြန်မာကုဒ် - Myanmar Programming Language</title>
    
    <!-- Open Graph Meta Tags -->
    <meta property="og:title" content="မြန်မာကုဒ် - Myanmar Programming Language">
    <meta property="og:description" content="မြန်မာဘာသာဖြင့် ပရိုဂရမ်းမင်းရေးသားနိုင်သော ပလက်ဖောင်း">
    <meta property="og:image" content="https://myanmar-code.org/assets/og-image.png">
    <meta property="og:url" content="https://myanmar-code.org">
    <meta property="og:type" content="website">
    
    <!-- Twitter Card -->
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="မြန်မာကုဒ် - Myanmar Programming Language">
    <meta name="twitter:description" content="မြန်မာဘာသာဖြင့် ပရိုဂရမ်းမင်းရေးသားနိုင်သော ပလက်ဖောင်း">
    <meta name="twitter:image" content="https://myanmar-code.org/assets/twitter-card.png">
    
    <!-- Favicon -->
    <link rel="icon" type="image/x-icon" href="assets/favicon.ico">
    <link rel="apple-touch-icon" sizes="180x180" href="assets/apple-touch-icon.png">
    
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Myanmar:wght@300;400;500;600;700&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Styles -->
    <style>
        /* Base Styles */
        :root {
            --primary-color: #2563eb;
            --primary-dark: #1d4ed8;
            --secondary-color: #7c3aed;
            --accent-color: #10b981;
            --text-color: #1f2937;
            --text-light: #6b7280;
            --bg-color: #ffffff;
            --bg-light: #f9fafb;
            --bg-dark: #111827;
            --border-color: #e5e7eb;
            --shadow-sm: 0 1px 3px rgba(0,0,0,0.12);
            --shadow-md: 0 4px 6px -1px rgba(0,0,0,0.1);
            --shadow-lg: 0 10px 15px -3px rgba(0,0,0,0.1);
            --radius-sm: 0.375rem;
            --radius-md: 0.5rem;
            --radius-lg: 0.75rem;
            --radius-xl: 1rem;
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
            font-family: 'Inter', 'Noto Sans Myanmar', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--bg-color);
            overflow-x: hidden;
        }
        
        .myanmar-font {
            font-family: 'Noto Sans Myanmar', 'Inter', sans-serif;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1.5rem;
        }
        
        .section {
            padding: 5rem 0;
        }
        
        .section-title {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 1rem;
            color: var(--text-color);
        }
        
        .section-subtitle {
            font-size: 1.125rem;
            text-align: center;
            color: var(--text-light);
            max-width: 600px;
            margin: 0 auto 3rem;
        }
        
        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 0.75rem 1.5rem;
            font-size: 1rem;
            font-weight: 600;
            text-decoration: none;
            border-radius: var(--radius-md);
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
            outline: none;
        }
        
        .btn-primary {
            background-color: var(--primary-color);
            color: white;
        }
        
        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: var(--shadow-md);
        }
        
        .btn-secondary {
            background-color: white;
            color: var(--text-color);
            border: 2px solid var(--border-color);
        }
        
        .btn-secondary:hover {
            border-color: var(--primary-color);
            color: var(--primary-color);
        }
        
        .btn-lg {
            padding: 1rem 2rem;
            font-size: 1.125rem;
        }
        
        .btn-icon {
            margin-right: 0.5rem;
        }
        
        /* Header & Navigation */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            box-shadow: var(--shadow-sm);
        }
        
        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            text-decoration: none;
        }
        
        .logo-icon {
            font-size: 1.75rem;
            color: var(--primary-color);
        }
        
        .logo-text {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--text-color);
        }
        
        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }
        
        .nav-link {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            padding: 0.5rem 0;
            position: relative;
            transition: color 0.3s ease;
        }
        
        .nav-link:hover {
            color: var(--primary-color);
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--primary-color);
            transition: width 0.3s ease;
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .nav-link.active {
            color: var(--primary-color);
        }
        
        .nav-link.active::after {
            width: 100%;
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--text-color);
            cursor: pointer;
        }
        
        /* Hero Section */
        .hero {
            padding-top: 8rem;
            padding-bottom: 5rem;
            background: linear-gradient(135deg, #f6f9ff 0%, #f0f4ff 100%);
            position: relative;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 50%;
            height: 100%;
            background: linear-gradient(45deg, transparent 70%, rgba(37, 99, 235, 0.05) 100%);
        }
        
        .hero-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }
        
        .hero-text {
            max-width: 600px;
        }
        
        .hero-title {
            font-size: 3.5rem;
            font-weight: 800;
            line-height: 1.2;
            margin-bottom: 1.5rem;
            color: var(--text-color);
        }
        
        .hero-title .highlight {
            color: var(--primary-color);
            position: relative;
            display: inline-block;
        }
        
        .hero-title .highlight::after {
            content: '';
            position: absolute;
            bottom: 0.25rem;
            left: 0;
            width: 100%;
            height: 0.5rem;
            background-color: rgba(37, 99, 235, 0.2);
            z-index: -1;
        }
        
        .hero-description {
            font-size: 1.25rem;
            color: var(--text-light);
            margin-bottom: 2rem;
            line-height: 1.8;
        }
        
        .hero-buttons {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }
        
        .hero-code {
            background-color: var(--bg-dark);
            border-radius: var(--radius-xl);
            padding: 2rem;
            box-shadow: var(--shadow-lg);
            position: relative;
            overflow: hidden;
        }
        
        .code-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
        }
        
        .code-title {
            color: #9ca3af;
            font-size: 0.875rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.05em;
        }
        
        .code-actions {
            display: flex;
            gap: 0.5rem;
        }
        
        .code-btn {
            width: 0.75rem;
            height: 0.75rem;
            border-radius: 50%;
            border: none;
            cursor: pointer;
        }
        
        .code-btn.close {
            background-color: #ef4444;
        }
        
        .code-btn.minimize {
            background-color: #f59e0b;
        }
        
        .code-btn.maximize {
            background-color: #10b981;
        }
        
        .code-content {
            font-family: 'Courier New', monospace;
            font-size: 0.875rem;
            line-height: 1.8;
        }
        
        .code-line {
            display: flex;
            align-items: flex-start;
            margin-bottom: 0.5rem;
        }
        
        .line-number {
            color: #6b7280;
            min-width: 2.5rem;
            text-align: right;
            padding-right: 1rem;
            user-select: none;
        }
        
        .code-keyword {
            color: #3b82f6;
        }
        
        .code-string {
            color: #10b981;
        }
        
        .code-comment {
            color: #6b7280;
        }
        
        .code-number {
            color: #f59e0b;
        }
        
        /* Features Section */
        .features {
            background-color: var(--bg-color);
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }
        
        .feature-card {
            background-color: white;
            padding: 2rem;
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow-sm);
            transition: all 0.3s ease;
            border: 1px solid var(--border-color);
        }
        
        .feature-card:hover {
            transform: translateY(-4px);
            box-shadow: var(--shadow-lg);
            border-color: var(--primary-color);
        }
        
        .feature-icon {
            width: 3rem;
            height: 3rem;
            background-color: rgba(37, 99, 235, 0.1);
            border-radius: var(--radius-md);
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 1.5rem;
        }
        
        .feature-icon i {
            font-size: 1.5rem;
            color: var(--primary-color);
        }
        
        .feature-title {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 0.75rem;
            color: var(--text-color);
        }
        
        .feature-description {
            color: var(--text-light);
            line-height: 1.7;
        }
        
        /* Examples Section */
        .examples {
            background-color: var(--bg-light);
        }
        
        .examples-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }
        
        .example-card {
            background-color: white;
            border-radius: var(--radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow-sm);
            transition: all 0.3s ease;
        }
        
        .example-card:hover {
            transform: translateY(-4px);
            box-shadow: var(--shadow-lg);
        }
        
        .example-header {
            background-color: var(--bg-dark);
            padding: 1rem 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .example-title {
            color: white;
            font-size: 1rem;
            font-weight: 600;
        }
        
        .example-difficulty {
            padding: 0.25rem 0.75rem;
            border-radius: var(--radius-sm);
            font-size: 0.75rem;
            font-weight: 600;
            text-transform: uppercase;
        }
        
        .difficulty-beginner {
            background-color: rgba(34, 197, 94, 0.2);
            color: #10b981;
        }
        
        .difficulty-intermediate {
            background-color: rgba(249, 115, 22, 0.2);
            color: #f97316;
        }
        
        .difficulty-advanced {
            background-color: rgba(239, 68, 68, 0.2);
            color: #ef4444;
        }
        
        .example-content {
            padding: 1.5rem;
            font-family: 'Courier New', monospace;
            font-size: 0.875rem;
            line-height: 1.8;
            background-color: #f8fafc;
            max-height: 300px;
            overflow-y: auto;
        }
        
        .example-actions {
            padding: 1rem 1.5rem;
            background-color: white;
            border-top: 1px solid var(--border-color);
            display: flex;
            gap: 0.75rem;
        }
        
        /* Installation Section */
        .installation {
            background-color: var(--bg-color);
        }
        
        .installation-steps {
            max-width: 800px;
            margin: 3rem auto 0;
        }
        
        .step {
            display: flex;
            align-items: flex-start;
            gap: 2rem;
            margin-bottom: 3rem;
            padding: 2rem;
            background-color: white;
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow-sm);
            border: 1px solid var(--border-color);
            transition: all 0.3s ease;
        }
        
        .step:hover {
            border-color: var(--primary-color);
            box-shadow: var(--shadow-md);
        }
        
        .step-number {
            width: 3rem;
            height: 3rem;
            background-color: var(--primary-color);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.25rem;
            font-weight: 700;
            flex-shrink: 0;
        }
        
        .step-content {
            flex: 1;
        }
        
        .step-title {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--text-color);
        }
        
        .step-description {
            color: var(--text-light);
            margin-bottom: 1rem;
        }
        
        .step-code {
            background-color: var(--bg-dark);
            border-radius: var(--radius-md);
            padding: 1rem;
            font-family: 'Courier New', monospace;
            font-size: 0.875rem;
            color: #e5e7eb;
            overflow-x: auto;
        }
        
        .step-code .prompt {
            color: #10b981;
        }
        
        /* Community Section */
        .community {
            background-color: var(--bg-light);
        }
        
        .community-content {
            text-align: center;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .community-stats {
            display: flex;
            justify-content: center;
            gap: 3rem;
            margin: 3rem 0;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }
        
        .stat-label {
            color: var(--text-light);
            font-size: 0.875rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
        }
        
        .community-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
        }
        
        .community-link {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.75rem 1.5rem;
            background-color: white;
            border-radius: var(--radius-md);
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            box-shadow: var(--shadow-sm);
            transition: all 0.3s ease;
            border: 1px solid var(--border-color);
        }
        
        .community-link:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-md);
            border-color: var(--primary-color);
            color: var(--primary-color);
        }
        
        .community-link i {
            font-size: 1.25rem;
        }
        
        /* Footer */
        .footer {
            background-color: var(--bg-dark);
            color: white;
            padding: 4rem 0 2rem;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-bottom: 3rem;
        }
        
        .footer-logo {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            margin-bottom: 1rem;
            text-decoration: none;
        }
        
        .footer-logo-icon {
            font-size: 1.5rem;
            color: var(--primary-color);
        }
        
        .footer-logo-text {
            font-size: 1.25rem;
            font-weight: 700;
            color: white;
        }
        
        .footer-description {
            color: #9ca3af;
            line-height: 1.7;
            margin-bottom: 1.5rem;
        }
        
        .footer-heading {
            font-size: 1.125rem;
            font-weight: 600;
            margin-bottom: 1.5rem;
            color: white;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-link {
            margin-bottom: 0.75rem;
        }
        
        .footer-link a {
            color: #9ca3af;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-link a:hover {
            color: var(--primary-color);
        }
        
        .footer-bottom {
            padding-top: 2rem;
            border-top: 1px solid #374151;
            text-align: center;
            color: #9ca3af;
            font-size: 0.875rem;
        }
        
        .footer-bottom a {
            color: var(--primary-color);
            text-decoration: none;
        }
        
        .footer-bottom a:hover {
            text-decoration: underline;
        }
        
        /* Responsive Design */
        @media (max-width: 1024px) {
            .hero-title {
                font-size: 2.75rem;
            }
            
            .section-title {
                font-size: 2.25rem;
            }
        }
        
        @media (max-width: 768px) {
            .hero-content {
                grid-template-columns: 1fr;
                gap: 3rem;
            }
            
            .hero-title {
                font-size: 2.25rem;
            }
            
            .hero-description {
                font-size: 1.125rem;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 4rem;
                left: 0;
                right: 0;
                background-color: white;
                flex-direction: column;
                padding: 1.5rem;
                box-shadow: var(--shadow-lg);
                transform: translateY(-100%);
                opacity: 0;
                visibility: hidden;
                transition: all 0.3s ease;
            }
            
            .nav-links.active {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }
            
            .section {
                padding: 3rem 0;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .step {
                flex-direction: column;
                gap: 1rem;
                padding: 1.5rem;
            }
            
            .step-number {
                width: 2.5rem;
                height: 2.5rem;
                font-size: 1rem;
            }
            
            .community-stats {
                flex-direction: column;
                gap: 2rem;
            }
        }
        
        @media (max-width: 480px) {
            .hero {
                padding-top: 6rem;
                padding-bottom: 3rem;
            }
            
            .hero-title {
                font-size: 1.75rem;
            }
            
            .hero-description {
                font-size: 1rem;
            }
            
            .hero-buttons {
                flex-direction: column;
            }
            
            .btn {
                width: 100%;
                text-align: center;
            }
            
            .section-title {
                font-size: 1.75rem;
            }
            
            .examples-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Header & Navigation -->
    <header class="header">
        <div class="container">
            <nav class="nav">
                <a href="/" class="logo">
                    <span class="logo-icon myanmar-font">🇲🇲</span>
                    <span class="logo-text myanmar-font">မြန်မာကုဒ်</span>
                </a>
                
                <button class="mobile-menu-btn" id="mobileMenuBtn">
                    <i class="fas fa-bars"></i>
                </button>
                
                <ul class="nav-links" id="navLinks">
                    <li><a href="#home" class="nav-link active">ပင်မစာမျက်နှာ</a></li>
                    <li><a href="#features" class="nav-link">အင်္ဂါရပ်များ</a></li>
                    <li><a href="#examples" class="nav-link">နမူနာများ</a></li>
                    <li><a href="#installation" class="nav-link">ထည့်သွင်းခြင်း</a></li>
                    <li><a href="#community" class="nav-link">အသိုင်းအဝိုင်း</a></li>
                    <li><a href="https://github.com/amo-master-221922/myanmar-code" class="nav-link" target="_blank">GitHub</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <div class="hero-text">
                    <h1 class="hero-title myanmar-font">
                        မြန်မာဘာသာဖြင့်
                        <span class="highlight myanmar-font">ပရိုဂရမ်းမင်း</span>
                        ရေးသားပါ
                    </h1>
                    <p class="hero-description myanmar-font">
                        မြန်မာကုဒ်သည် မြန်မာဘာသာစကားဖြင့် ပရိုဂရမ်းမင်းရေးသားနိုင်သော ပထမဆုံးအကြိမ် 
                        ပြည့်စုံသည့် Interpreter ဖြစ်သည်။ eval() လုံးဝမသုံးဘဲ လုံခြုံပြီး မြန်ဆန်သော 
                        execution ကို ပေးစွမ်းနိုင်သည်။
                    </p>
                    <div class="hero-buttons">
                        <a href="#installation" class="btn btn-primary btn-lg">
                            <i class="fas fa-download btn-icon"></i>
                            စတင်အသုံးပြုရန်
                        </a>
                        <a href="#examples" class="btn btn-secondary btn-lg">
                            <i class="fas fa-code btn-icon"></i>
                            နမူနာများကြည့်ရန်
                        </a>
                    </div>
                </div>
                
                <div class="hero-code">
                    <div class="code-header">
                        <div class="code-title">program.mmr</div>
                        <div class="code-actions">
                            <button class="code-btn close"></button>
                            <button class="code-btn minimize"></button>
                            <button class="code-btn maximize"></button>
                        </div>
                    </div>
                    <div class="code-content">
                        <div class="code-line">
                            <span class="line-number">1</span>
                            <span class="code-comment"># မြန်မာကုဒ်ဖြင့် ပရိုဂရမ်းမင်း</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">2</span>
                            <span class="code-keyword myanmar-font">နေရာ</span>
                            <span> </span>
                            <span>နာမည် = </span>
                            <span class="code-string">"ကိုကိုနတ်"</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">3</span>
                            <span class="code-keyword myanmar-font">နေရာ</span>
                            <span> </span>
                            <span>အသက် = </span>
                            <span class="code-number">၂၅</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">4</span>
                            <span></span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">5</span>
                            <span class="code-keyword myanmar-font">အကယ်၍</span>
                            <span> </span>
                            <span>အသက် >= </span>
                            <span class="code-number">၁၈</span>
                            <span> </span>
                            <span class="code-keyword myanmar-font">ဒါဆို</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">6</span>
                            <span>    </span>
                            <span class="code-keyword myanmar-font">ပုံနှိပ်</span>
                            <span> </span>
                            <span class="code-string">"မင်္ဂလာပါ "</span>
                            <span> + နာမည်</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">7</span>
                            <span class="code-keyword myanmar-font">မဟုတ်ရင်</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">8</span>
                            <span>    </span>
                            <span class="code-keyword myanmar-font">ပုံနှိပ်</span>
                            <span> </span>
                            <span class="code-string">"အရွယ်မရောက်သေးပါ"</span>
                        </div>
                        <div class="code-line">
                            <span class="line-number">9</span>
                            <span class="code-keyword myanmar-font">အဆုံး</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="section features" id="features">
        <div class="container">
            <h2 class="section-title myanmar-font">ထူးခြားချက်များ</h2>
            <p class="section-subtitle myanmar-font">
                မြန်မာကုဒ်၏ ထူးခြားသော အင်္ဂါရပ်များကို လေ့လာပါ
            </p>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-language"></i>
                    </div>
                    <h3 class="feature-title myanmar-font">မြန်မာစစ်စစ်</h3>
                    <p class="feature-description myanmar-font">
                        မြန်မာဘာသာစကားဖြင့် ပရိုဂရမ်းမင်းရေးသားနိုင်သည်။ 
                        မြန်မာစာလုံးများ၊ မြန်မာဂဏန်းများနှင့် မြန်မာဝါကျဖွဲ့စည်းပုံကို ထောက်ပံ့ပေးသည်။
                    </p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3 class="feature-title myanmar-font">လုံခြုံသည်</h3>
                    <p class="feature-description myanmar-font">
                        eval() လုံးဝမသုံးဘဲ ကိုယ်ပိုင် evaluation engine ဖြင့် 
                        လုံခြုံသော execution ကို ပေးစွမ်းနိုင်သည်။ Code injection 
                        အန္တရာယ်မှ ကင်းရှင်းသည်။
                    </p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <h3 class="feature-title myanmar-font">မြန်ဆန်သည်</h3>
                    <p class="feature-description myanmar-font">
                        Optimized interpreter ဖြင့် မြန်ဆန်သော execution speed ရှိသည်။ 
                        Lexer, Parser, Evaluator အားလုံး performance optimization 
                        ပြုလုပ်ထားသည်။
                    </p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-book"></i>
                    </div>
                    <h3 class="feature-title myanmar-font">လေ့လာရလွယ်သည်</h3>
                    <p class="feature-description myanmar-font">
                        မြန်မာလို documentation နှင့် နမူနာများ ပါဝင်သည်။ 
                        စတင်သူများအတွက် လွယ်ကူသော syntax နှင့် ရှင်းလင်းသော error messages များ ပေးစွမ်းနိုင်သည်။
                    </p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-cogs"></i>
                    </div>
                    <h3 class="feature-title myanmar-font">ပြည့်စုံသည်</h3>
                    <p class="feature-description myanmar-font">
                        Built-in functions 30+၊ File I/O operations၊ Standard library modules၊ 
                        Error handling system နှင့် Testing framework များ ပါဝင်သည်။
                    </p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3 class="feature-title myanmar-font">အသိုင်းအဝိုင်း</h3>
                    <p class="feature-description myanmar-font">
                        ကြီးထွားလာသော အသိုင်းအဝိုင်းနှင့် ပြည့်စုံသော support system ရှိသည်။ 
                        Community forum၊ GitHub discussions နှင့် နမူနာများ များစွာရှိသည်။
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Examples Section -->
    <section class="section examples" id="examples">
        <div class="container">
            <h2 class="section-title myanmar-font">နမူနာများ</h2>
            <p class="section-subtitle myanmar-font">
                မြန်မာကုဒ်ဖြင့် ရေးသားထားသော နမူနာပရိုဂရမ်များ
            </p>
            
            <div class="examples-grid">
                <div class="example-card">
                    <div class="example-header">
                        <div class="example-title">Hello World</div>
                        <div class="example-difficulty difficulty-beginner">အစပြုသူ</div>
                    </div>
                    <div class="example-content">
                        <pre class="myanmar-font"># hello_world.mmr
ပုံနှိပ် "မင်္ဂလာပါ ကမ္ဘာကြီး"
ပုံနှိပ် "မြန်မာကုဒ် စမ်းသပ်ခြင်း"</pre>
                    </div>
                    <div class="example-actions">
                        <button class="btn btn-primary" onclick="copyCode('hello_world')">
                            <i class="fas fa-copy"></i> Copy
                        </button>
                        <button class="btn btn-secondary" onclick="runExample('hello_world')">
                            <i class="fas fa-play"></i> Run
                        </button>
                    </div>
                </div>
                
                <div class="example-card">
                    <div class="example-header">
                        <div class="example-title">Calculator</div>
                        <div class="example-difficulty difficulty-intermediate">အလယ်အလတ်</div>
                    </div>
                    <div class="example-content">
                        <pre class="myanmar-font"># calculator.mmr
လုပ်ဆောင်ချက် ပေါင်းပါ(a, b)
    ပြန်ပို့ a + b
အဆုံး

နေရာ result = ပေါင်းပါ(၁၀, ၅)
ပုံနှိပ် "ပေါင်းလဒ်: " + result</pre>
                    </div>
                    <div class="example-actions">
                        <button class="btn btn-primary" onclick="copyCode('calculator')">
                            <i class="fas fa-copy"></i> Copy
                        </button>
                        <button class="btn btn-secondary" onclick="runExample('calculator')">
                            <i class="fas fa-play"></i> Run
                        </button>
                    </div>
                </div>
                
                <div class="example-card">
                    <div class="example-header">
                        <div class="example-title">Fibonacci</div>
                        <div class="example-difficulty difficulty-advanced">အဆင့်မြင့်</div>
                    </div>
                    <div class="example-content">
                        <pre class="myanmar-font"># fibonacci.mmr
လုပ်ဆောင်ချက် ဖီဘိုနာချီ(n)
    အကယ်၍ n <= ၁ ဒါဆို
        ပြန်ပို့ n
    မဟုတ်ရင်
        ပြန်ပို့ ဖီဘိုနာချီ(n-၁) + ဖီဘိုနာချီ(n-၂)
    အဆုံး
အဆုံး

ပုံနှိပ် "ဖီဘိုနာချီကိန်းများ:"
အတွက် i ကို ၀ မှ ၁၀ အထိ လုပ်ပါ
    ပုံနှိပ် ဖီဘိုနာချီ(i)
အဆုံး</pre>
                    </div>
                    <div class="example-actions">
                        <button class="btn btn-primary" onclick="copyCode('fibonacci')">
                            <i class="fas fa-copy"></i> Copy
                        </button>
                        <button class="btn btn-secondary" onclick="runExample('fibonacci')">
                            <i class="fas fa-play"></i> Run
                        </button>
                    </div>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 3rem;">
                <a href="https://github.com/amo-master-221922/myanmar-code/tree/main/examples" 
                   class="btn btn-primary" target="_blank">
                    <i class="fas fa-external-link-alt btn-icon"></i>
                    နမူနာပိုမိုကြည့်ရန်
                </a>
            </div>
        </div>
    </section>

    <!-- Installation Section -->
    <section class="section installation" id="installation">
        <div class="container">
            <h2 class="section-title myanmar-font">ထည့်သွင်းခြင်း</h2>
            <p class="section-subtitle myanmar-font">
                မြန်မာကုဒ်ကို ၄ ဆင့်အတွင်း ထည့်သွင်းအသုံးပြုနိုင်သည်
            </p>
            
            <div class="installation-steps">
                <div class="step">
                    <div class="step-number">၁</div>
                    <div class="step-content">
                        <h3 class="step-title myanmar-font">Python စစ်ဆေးပါ</h3>
                        <p class="step-description myanmar-font">
                            Python 3.6 သို့မဟုတ် အထက်ရှိရန် လိုအပ်ပါသည်။
                        </p>
                        <div class="step-code">
                            <span class="prompt">$</span> python --version<br>
                            <span class="prompt">$</span> python3 --version
                        </div>
                    </div>
                </div>
                
                <div class="step">
                    <div class="step-number">၂</div>
                    <div class="step-content">
                        <h3 class="step-title myanmar-font">မြန်မာကုဒ် ထည့်သွင်းပါ</h3>
                        <p class="step-description myanmar-font">
                            PIP ကိုသုံး၍ မြန်မာကုဒ်ကို ထည့်သွင်းပါ။
                        </p>
                        <div class="step-code">
                            <span class="prompt">$</span> pip install myanmar-code
                        </div>
                    </div>
                </div>
                
                <div class="step">
                    <div class="step-number">၃</div>
                    <div class="step-content">
                        <h3 class="step-title myanmar-font">ထည့်သွင်းမှု စစ်ဆေးပါ</h3>
                        <p class="step-description myanmar-font">
                            ထည့်သွင်းမှု အောင်မြင်ကြောင်း စစ်ဆေးပါ။
                        </p>
                        <div class="step-code">
                            <span class="prompt">$</span> myanmar-code --version<br>
                            Myanmar Code v1.0.0
                        </div>
                    </div>
                </div>
                
                <div class="step">
                    <div class="step-number">၄</div>
                    <div class="step-content">
                        <h3 class="step-title myanmar-font">မြန်မာကုဒ် စတင်အသုံးပြုပါ</h3>
                        <p class="step-description myanmar-font">
                            မြန်မာကုဒ်ကို စတင်အသုံးပြုပါ။
                        </p>
                        <div class="step-code">
                            <span class="prompt">$</span> myanmar-code<br>
                            >>> ပုံနှိပ် "မင်္ဂလာပါ"<br>
                            မင်္ဂလာပါ
                        </div>
                    </div>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 3rem;">
                <a href="https://github.com/amo-master-221922/myanmar-code#installation" 
                   class="btn btn-primary btn-lg" target="_blank">
                    <i class="fas fa-book btn-icon"></i>
                    အသေးစိတ် Installation Guide
                </a>
            </div>
        </div>
    </section>

    <!-- Community Section -->
    <section class="section community" id="community">
        <div class="container">
            <h2 class="section-title myanmar-font">အသိုင်းအဝိုင်း</h2>
            <p class="section-subtitle myanmar-font">
                မြန်မာကုဒ် အသိုင်းအဝိုင်းတွင် ပါဝင်ပြီး အခြားပရိုဂရမ်းမင်းများနှင့် ချိတ်ဆက်ပါ
            </p>
            
            <div class="community-content">
                <div class="community-stats">
                    <div class="stat">
                        <div class="stat-number">100+</div>
                        <div class="stat-label">အသုံးပြုသူများ</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">30+</div>
                        <div class="stat-label">Built-in Functions</div>
                    </div>
                    <div class="stat">
                        <div class="stat-number">50+</div>
                        <div class="stat-label">နမူနာများ</div>
                    </div>
                </div>
                
                <div class="community-links">
                    <a href="https://github.com/amo-master-221922/myanmar-code" class="community-link" target="_blank">
                        <i class="fab fa-github"></i>
                        GitHub
                    </a>
                    <a href="https://github.com/amo-master-221922/myanmar-code/discussions" class="community-link" target="_blank">
                        <i class="fas fa-comments"></i>
                        Discussions
                    </a>
                    <a href="https://github.com/amo-master-221922/myanmar-code/issues" class="community-link" target="_blank">
                        <i class="fas fa-bug"></i>
                        Issues
                    </a>
                    <a href="https://github.com/amo-master-221922/myanmar-code/wiki" class="community-link" target="_blank">
                        <i class="fas fa-book"></i>
                        Wiki
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <a href="/" class="footer-logo">
                        <span class="footer-logo-icon myanmar-font">🇲🇲</span>
                        <span class="footer-logo-text myanmar-font">မြန်မာကုဒ်</span>
                    </a>
                    <p class="footer-description myanmar-font">
                        မြန်မာဘာသာဖြင့် ပရိုဂရမ်းမင်းရေးသားနိုင်သော ပလက်ဖောင်း။ 
                        eval() လုံးဝမသုံးဘဲ လုံခြုံပြီး မြန်ဆန်သော execution ကို ပေးစွမ်းနိုင်သည်။
                    </p>
                </div>
                
                <div class="footer-links-section">
                    <h3 class="footer-heading myanmar-font">လင့်ခ်များ</h3>
                    <ul class="footer-links">
                        <li class="footer-link"><a href="#home">ပင်မစာမျက်နှာ</a></li>
                        <li class="footer-link"><a href="#features">အင်္ဂါရပ်များ</a></li>
                        <li class="footer-link"><a href="#examples">နမူနာများ</a></li>
                        <li class="footer-link"><a href="#installation">ထည့်သွင်းခြင်း</a></li>
                        <li class="footer-link"><a href="#community">အသိုင်းအဝိုင်း</a></li>
                    </ul>
                </div>
                
                <div class="footer-links-section">
                    <h3 class="footer-heading myanmar-font">အရင်းအမြစ်များ</h3>
                    <ul class="footer-links">
                        <li class="footer-link"><a href="https://github.com/amo-master-221922/myanmar-code" target="_blank">GitHub Repository</a></li>
                        <li class="footer-link"><a href="https://github.com/amo-master-221922/myanmar-code/wiki" target="_blank">Documentation</a></li>
                        <li class="footer-link"><a href="https://github.com/amo-master-221922/myanmar-code/tree/main/examples" target="_blank">Examples</a></li>
                        <li class="footer-link"><a href="https://github.com/amo-master-221922/myanmar-code/issues" target="_blank">Issue Tracker</a></li>
                        <li class="footer-link"><a href="https://github.com/amo-master-221922/myanmar-code/releases" target="_blank">Releases</a></li>
                    </ul>
                </div>
                
                <div class="footer-links-section">
                    <h3 class="footer-heading myanmar-font">ဆက်သွယ်ရန်</h3>
                    <ul class="footer-links">
                        <li class="footer-link"><a href="https://github.com/amo-master-221922/myanmar-code/discussions" target="_blank">Community Discussions</a></li>
                        <li class="footer-link"><a href="https://github.com/amo-master-221922" target="_blank">AMO MASTER 221922</a></li>
                        <li class="footer-link"><a href="mailto:support@myanmar-code.org">Email Support</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p class="myanmar-font">
                    &copy; 2023 မြန်မာကုဒ် - AMO MASTER 221922 Team. All rights reserved.
                    <br>
                    <a href="https://github.com/amo-master-221922/myanmar-code/blob/main/LICENSE" target="_blank">MIT License</a>
                </p>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const navLinks = document.getElementById('navLinks');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.classList.toggle('active');
            mobileMenuBtn.innerHTML = navLinks.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Close mobile menu when clicking on a link
        document.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
                mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Active navigation link on scroll
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('section[id]');
            const scrollPosition = window.scrollY + 100;
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.offsetHeight;
                const sectionId = section.getAttribute('id');
                
                if (scrollPosition >= sectionTop && scrollPosition < sectionTop + sectionHeight) {
                    document.querySelectorAll('.nav-link').forEach(link => {
                        link.classList.remove('active');
                        if (link.getAttribute('href') === `#${sectionId}`) {
                            link.classList.add('active');
                        }
                    });
                }
            });
        });
        
        // Copy code examples
        function copyCode(exampleName) {
            const examples = {
                'hello_world': `# hello_world.mmr
ပုံနှိပ် "မင်္ဂလာပါ ကမ္ဘာကြီး"
ပုံနှိပ် "မြန်မာကုဒ် စမ်းသပ်ခြင်း"`,
                
                'calculator': `# calculator.mmr
လုပ်ဆောင်ချက် ပေါင်းပါ(a, b)
    ပြန်ပို့ a + b
အဆုံး

နေရာ result = ပေါင်းပါ(၁၀, ၅)
ပုံနှိပ် "ပေါင်းလဒ်: " + result`,
                
                'fibonacci': `# fibonacci.mmr
လုပ်ဆောင်ချက် ဖီဘိုနာချီ(n)
    အကယ်၍ n <= ၁ ဒါဆို
        ပြန်ပို့ n
    မဟုတ်ရင်
        ပြန်ပို့ ဖီဘိုနာချီ(n-၁) + ဖီဘိုနာချီ(n-၂)
    အဆုံး
အဆုံး

ပုံနှိပ် "ဖီဘိုနာချီကိန်းများ:"
အတွက် i ကို ၀ မှ ၁၀ အထိ လုပ်ပါ
    ပုံနှိပ် ဖီဘိုနာချီ(i)
အဆုံး`
            };
            
            if (examples[exampleName]) {
                navigator.clipboard.writeText(examples[exampleName])
                    .then(() => {
                        alert('Code copied to clipboard!');
                    })
                    .catch(err => {
                        console.error('Failed to copy: ', err);
                        alert('Failed to copy code. Please try again.');
                    });
            }
        }
        
        // Run example (placeholder)
        function runExample(exampleName) {
            alert(`Running ${exampleName} example...\n\nIn a real environment, this would execute the Myanmar code.`);
        }
        
        // Initialize
        document.addEventListener('DOMContentLoaded', () => {
            // Set current year in footer
            const yearElement = document.querySelector('.footer-bottom p');
            if (yearElement) {
                yearElement.innerHTML = yearElement.innerHTML.replace('2023', new Date().getFullYear());
            }
            
            // Add active class to home link by default
            if (window.location.hash === '' || window.location.hash === '#') {
                document.querySelector('.nav-link[href="#home"]').classList.add('active');
            }
        });
    </script>
</body>
</html>
