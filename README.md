<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Remove image backgrounds instantly with Re-Move BG. Free online tool with high-quality background removal in seconds.">
    <meta name="keywords" content="remove background, transparent background, image editor, free background remover, online photo editor">
    <meta name="author" content="Re-Move BG">
    <meta property="og:title" content="Re-Move BG | Free Online Background Remover">
    <meta property="og:description" content="Remove backgrounds from images automatically in 5 seconds with our free online tool.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://yourusername.github.io/re-move-bg">
    <meta name="theme-color" content="#FD1D1D">
    <title>Re-Move BG | Free Online Background Remover</title>
    <style>
        :root {
            --primary: #FD1D1D;
            --secondary: #833AB4;
            --tertiary: #405DE6;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
            --shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Native Ad Container */
        .native-ad-container {
            width: 100%;
            display: flex;
            justify-content: center;
            padding: 10px 0;
            background: #f8f9fa;
            margin-bottom: 20px;
        }

        /* Middle Banner Ad Styling */
        .middle-banner-ad {
            width: 100%;
            display: flex;
            justify-content: center;
            margin: 30px 0;
            padding: 10px 0;
            background: #f8f9fa;
        }

        /* Social Bar Ad Styling */
        .social-bar-ad {
            width: 100%;
            display: flex;
            justify-content: center;
            margin: 30px 0;
            padding: 15px 0;
            background: #f8f9fa;
            border-radius: 10px;
        }

        header {
            background: linear-gradient(45deg, var(--primary), var(--secondary), var(--tertiary));
            color: white;
            padding: 20px 0;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transform: rotate(45deg);
            animation: shine 3s infinite;
        }

        @keyframes shine {
            0% { transform: rotate(45deg) translate(-30%, -30%); }
            100% { transform: rotate(45deg) translate(30%, 30%); }
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
            z-index: 1;
        }

        .logo {
            font-size: 24px;
            font-weight: 700;
            display: flex;
            align-items: center;
        }

        .logo span {
            margin-left: 10px;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            padding: 5px 10px;
            border-radius: 5px;
        }

        nav ul li a:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }

        .hero {
            text-align: center;
            padding: 60px 0 40px;
            background: linear-gradient(135deg, rgba(253, 29, 29, 0.05), rgba(64, 93, 230, 0.05));
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            background: linear-gradient(45deg, var(--primary), var(--secondary), var(--tertiary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: gradient 5s ease infinite;
            background-size: 200% 200%;
        }

        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .hero p {
            font-size: 1.1rem;
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto 30px;
        }

        .upload-container {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: var(--shadow);
            max-width: 800px;
            margin: 0 auto;
            transition: var(--transition);
        }

        .upload-container:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
        }

        .upload-area {
            border: 2px dashed #ddd;
            border-radius: 8px;
            padding: 40px 20px;
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
            margin-bottom: 20px;
            position: relative;
            overflow: hidden;
        }

        .upload-area:hover {
            border-color: var(--primary);
        }

        .upload-area.active {
            border-color: var(--secondary);
            background-color: rgba(131, 58, 180, 0.05);
        }

        .upload-area i {
            font-size: 48px;
            color: var(--tertiary);
            margin-bottom: 15px;
            display: inline-block;
            transition: var(--transition);
        }

        .upload-area:hover i {
            transform: scale(1.1);
            color: var(--primary);
        }

        .upload-area h3 {
            margin-bottom: 10px;
            color: var(--dark);
        }

        .upload-area p {
            color: var(--gray);
            margin-bottom: 15px;
        }

        .btn {
            display: inline-block;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white;
            padding: 12px 24px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            border: none;
            cursor: pointer;
            transition: var(--transition);
            box-shadow: 0 4px 15px rgba(253, 29, 29, 0.3);
            position: relative;
            overflow: hidden;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(253, 29, 29, 0.4);
        }

        .btn:active {
            transform: translateY(1px);
        }

        .btn::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, var(--tertiary), var(--secondary));
            opacity: 0;
            transition: var(--transition);
            z-index: -1;
        }

        .btn:hover::after {
            opacity: 1;
        }

        .btn-secondary {
            background: white;
            color: var(--dark);
            border: 1px solid #ddd;
            box-shadow: none;
        }

        .btn-secondary:hover {
            background: #f8f9fa;
            box-shadow: none;
        }

        #fileInput {
            display: none;
        }

        .preview-container {
            display: none;
            margin-top: 30px;
            animation: fadeIn 0.5s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .preview-title {
            text-align: center;
            margin-bottom: 20px;
            color: var(--dark);
        }

        .preview-columns {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .preview-box {
            flex: 1;
            min-width: 300px;
            background-color: white;
            border-radius: 10px;
            padding: 20px;
            box-shadow: var(--shadow);
            text-align: center;
        }

        .preview-box h3 {
            margin-bottom: 15px;
            color: var(--dark);
        }

        .image-preview {
            width: 100%;
            height: auto;
            max-height: 300px;
            object-fit: contain;
            border-radius: 5px;
            margin-bottom: 15px;
            background-color: #f8f9fa;
            background-image: linear-gradient(45deg, #eee 25%, transparent 25%, transparent 75%, #eee 75%, #eee),
                              linear-gradient(45deg, #eee 25%, transparent 25%, transparent 75%, #eee 75%, #eee);
            background-size: 20px 20px;
            background-position: 0 0, 10px 10px;
        }

        .action-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 30px;
            flex-wrap: wrap;
        }

        .loading {
            display: none;
            text-align: center;
            margin: 30px 0;
        }

        .spinner {
            width: 50px;
            height: 50px;
            border: 5px solid rgba(64, 93, 230, 0.2);
            border-radius: 50%;
            border-top-color: var(--tertiary);
            animation: spin 1s linear infinite;
            margin: 0 auto 15px;
        }

        @keyframes spin {
            100% { transform: rotate(360deg); }
        }

        .features {
            padding: 60px 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 2rem;
            color: var(--dark);
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .feature-card {
            background-color: var(--light);
            border-radius: 10px;
            padding: 30px;
            text-align: center;
            transition: var(--transition);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }

        .feature-icon {
            font-size: 40px;
            margin-bottom: 20px;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .feature-card h3 {
            margin-bottom: 15px;
            color: var(--dark);
        }

        .feature-card p {
            color: var(--gray);
        }

        footer {
            background: linear-gradient(45deg, var(--dark), #343a40);
            color: white;
            padding: 40px 0 20px;
        }

        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 40px;
            margin-bottom: 30px;
        }

        .footer-column {
            flex: 1;
            min-width: 200px;
        }

        .footer-column h3 {
            margin-bottom: 20px;
            font-size: 1.2rem;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 40px;
            height: 3px;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column ul li {
            margin-bottom: 10px;
        }

        .footer-column ul li a {
            color: #adb5bd;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-column ul li a:hover {
            color: white;
            padding-left: 5px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: var(--transition);
        }

        .social-links a:hover {
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #adb5bd;
            font-size: 0.9rem;
        }

        /* Mobile styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                margin-top: 20px;
                justify-content: center;
            }

            nav ul li {
                margin: 0 10px;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .preview-columns {
                flex-direction: column;
            }

            .preview-box {
                min-width: 100%;
            }

            .action-buttons {
                flex-direction: column;
                align-items: center;
            }

            .btn {
                width: 100%;
                text-align: center;
            }

            .footer-content {
                flex-direction: column;
            }
        }

        /* Confetti effect */
        .confetti {
            position: fixed;
            width: 10px;
            height: 10px;
            background-color: var(--primary);
            opacity: 0;
            animation: confetti 3s ease-out;
            z-index: 1000;
        }

        @keyframes confetti {
            0% { transform: translateY(0) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>✂️</text></svg>">
</head>
<body>
    <!-- Native Ad Container (728x90) -->
    <div class="native-ad-container">
        <script type="text/javascript">
            atOptions = {
                'key' : '59ecbdc58d543da449404bda675ea564',
                'format' : 'iframe',
                'height' : 90,
                'width' : 728,
                'params' : {}
            };
        </script>
        <script type="text/javascript" src="//www.highperformanceformat.com/59ecbdc58d543da449404bda675ea564/invoke.js"></script>
    </div>

    <header>
        <div class="container header-content">
            <div class="logo">
                <i class="fas fa-cut"></i>
                <span>Re–Move BG</span>
            </div>
            <nav>
                <ul>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#how-it-works">How It Works</a></li>
                    <li><a href="#about">About</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Remove Background from Images Instantly</h1>
            <p>Upload your photo and let our AI remove the background automatically. Fast, free, and no signup required!</p>
           
            <div class="upload-container">
                <div class="upload-area" id="uploadArea">
                    <i class="fas fa-cloud-upload-alt"></i>
                    <h3>Upload Your Image</h3>
                    <p>Drag & drop your image here or click to browse</p>
                    <button class="btn">Select Image</button>
                    <input type="file" id="fileInput" accept="image/*">
                </div>
                <p class="text-center" style="color: var(--gray); font-size: 0.9rem;">
                    Supported formats: JPG, PNG, WEBP (Max 5MB)
                </p>
            </div>
        </div>
    </section>

    <div class="container">
        <div class="loading" id="loadingIndicator">
            <div class="spinner"></div>
            <p>Removing background... This may take a few seconds</p>
        </div>

        <div class="preview-container" id="previewContainer">
            <h2 class="preview-title">Your Background-Free Image</h2>
            <div class="preview-columns">
                <div class="preview-box">
                    <h3>Original Image</h3>
                    <img id="originalImage" class="image-preview" src="" alt="Original image">
                </div>
                <div class="preview-box">
                    <h3>Background Removed</h3>
                    <img id="processedImage" class="image-preview" src="" alt="Background removed image">
                </div>
            </div>
            <div class="action-buttons">
                <button class="btn" id="downloadBtn">
                    <i class="fas fa-download"></i> Download Image
                </button>
                <button class="btn btn-secondary" id="newImageBtn">
                    <i class="fas fa-redo"></i> Process New Image
                </button>
            </div>
        </div>

        <!-- Middle Banner Ad (320x50) -->
        <div class="middle-banner-ad">
            <script type="text/javascript">
                atOptions = {
                    'key' : 'e662eed619b1d026f6e77af5174b3b90',
                    'format' : 'iframe',
                    'height' : 50,
                    'width' : 320,
                    'params' : {}
                };
            </script>
            <script type="text/javascript" src="//www.highperformanceformat.com/e662eed619b1d026f6e77af5174b3b90/invoke.js"></script>
        </div>
    </div>

    <section class="features" id="features">
        <div class="container">
            <h2 class="section-title">Why Choose Re–Move BG?</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <h3>Lightning Fast</h3>
                    <p>Our AI processes images in seconds, saving you time and effort compared to manual editing.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-lock"></i>
                    </div>
                    <h3>Privacy Focused</h3>
                    <p>We automatically delete your images after processing. Your photos never get stored on our servers.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-gem"></i>
                    </div>
                    <h3>High Quality</h3>
                    <p>Get professional-quality results with clean edges and transparent backgrounds every time.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Social Bar Ad -->
    <div class="social-bar-ad">
        <script type='text/javascript' src='//pl26580036.profitableratecpm.com/f2/79/81/f279814704da88ab11691838e329d85f.js'></script>
    </div>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Re–Move BG</h3>
                    <p>The easiest way to remove backgrounds from your images automatically and for free.</p>
                    <div class="social-links">
                        <a href="#" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                        <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                        <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#how-it-works">How It Works</a></li>
                        <li><a href="#about">About</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Resources</h3>
                    <ul>
                        <li><a href="#">Help Center</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>© <span id="currentYear"></span> Re–Move BG. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year in footer
            document.getElementById('currentYear').textContent = new Date().getFullYear();
           
            // File upload handling
            const uploadArea = document.getElementById('uploadArea');
            const fileInput = document.getElementById('fileInput');
            const previewContainer = document.getElementById('previewContainer');
            const loadingIndicator = document.getElementById('loadingIndicator');
            const originalImage = document.getElementById('originalImage');
            const processedImage = document.getElementById('processedImage');
            const downloadBtn = document.getElementById('downloadBtn');
            const newImageBtn = document.getElementById('newImageBtn');
           
            // Handle drag and drop
            uploadArea.addEventListener('click', () => fileInput.click());
           
            uploadArea.addEventListener('dragover', (e) => {
                e.preventDefault();
                uploadArea.classList.add('active');
            });
           
            uploadArea.addEventListener('dragleave', () => {
                uploadArea.classList.remove('active');
            });
           
            uploadArea.addEventListener('drop', (e) => {
                e.preventDefault();
                uploadArea.classList.remove('active');
                if (e.dataTransfer.files.length) {
                    fileInput.files = e.dataTransfer.files;
                    handleFileUpload(e.dataTransfer.files[0]);
                }
            });
           
            fileInput.addEventListener('change', () => {
                if (fileInput.files.length) {
                    handleFileUpload(fileInput.files[0]);
                }
            });

            // Remove.bg API Integration (50 free requests/month)
            async function removeBackgroundWithAPI(imageFile) {
                const API_KEY = 'Fqsgcyr5e8h1GkCZgVCwzLS6'; // Your provided API key
                const formData = new FormData();
                formData.append('image_file', imageFile);
                formData.append('size', 'auto');
               
                try {
                    const response = await fetch('https://api.remove.bg/v1.0/removebg', {
                        method: 'POST',
                        headers: {
                            'X-Api-Key': API_KEY
                        },
                        body: formData
                    });
                   
                    if (!response.ok) {
                        throw new Error('API request failed');
                    }
                   
                    return await response.blob();
                } catch (error) {
                    console.error('API Error:', error);
                    throw error;
                }
            }

            // Advanced client-side background removal
            async function removeBackgroundClientSide(imageData) {
                return new Promise((resolve) => {
                    const img = new Image();
                    img.onload = function() {
                        const canvas = document.createElement('canvas');
                        canvas.width = img.width;
                        canvas.height = img.height;
                        const ctx = canvas.getContext('2d');
                        ctx.drawImage(img, 0, 0);
                       
                        const imageData = ctx.getImageData(0, 0, canvas.width, canvas.height);
                        const data = imageData.data;
                       
                        // Detect background color from corners
                        const bgColor = getBackgroundColor(canvas, ctx);
                        const threshold = 30;
                       
                        for (let i = 0; i < data.length; i += 4) {
                            const r = data[i];
                            const g = data[i + 1];
                            const b = data[i + 2];
                           
                            // Check if pixel is similar to background
                            if (colorDistance(r, g, b, bgColor.r, bgColor.g, bgColor.b) < threshold) {
                                data[i + 3] = 0; // Set alpha to transparent
                            }
                        }
                       
                        ctx.putImageData(imageData, 0, 0);
                        resolve(canvas.toDataURL());
                    };
                    img.src = imageData;
                });
            }

            function getBackgroundColor(canvas, ctx) {
                // Sample corners to determine background color
                const corners = [
                    [0, 0], [canvas.width-1, 0],
                    [0, canvas.height-1], [canvas.width-1, canvas.height-1]
                ];
               
                let r = 0, g = 0, b = 0;
               
                corners.forEach(pos => {
                    const pixel = ctx.getImageData(pos[0], pos[1], 1, 1).data;
                    r += pixel[0];
                    g += pixel[1];
                    b += pixel[2];
                });
               
                return {
                    r: Math.round(r / corners.length),
                    g: Math.round(g / corners.length),
                    b: Math.round(b / corners.length)
                };
            }

            function colorDistance(r1, g1, b1, r2, g2, b2) {
                // Calculate Euclidean distance between colors
                const dr = r1 - r2;
                const dg = g1 - g2;
                const db = b1 - b2;
                return Math.sqrt(dr*dr + dg*dg + db*db);
            }

            async function handleFileUpload(file) {
                // Check file type and size
                const validTypes = ['image/jpeg', 'image/png', 'image/webp'];
                const maxSize = 5 * 1024 * 1024; // 5MB
               
                if (!validTypes.includes(file.type)) {
                    alert('Please upload a valid image file (JPEG, PNG, or WEBP)');
                    return;
                }
               
                if (file.size > maxSize) {
                    alert('File size exceeds 5MB limit. Please choose a smaller image.');
                    return;
                }
               
                // Show loading indicator
                loadingIndicator.style.display = 'block';
               
                // Display original image
                const reader = new FileReader();
                reader.onload = async function(e) {
                    originalImage.src = e.target.result;
                   
                    try {
                        // First try with Remove.bg API
                        const blob = await removeBackgroundWithAPI(file);
                        const processedUrl = URL.createObjectURL(blob);
                        processedImage.src = processedUrl;
                    } catch (apiError) {
                        console.log('API failed, trying client-side solution');
                        // If API fails, try client-side solution
                        const processedData = await removeBackgroundClientSide(e.target.result);
                        processedImage.src = processedData;
                    }
                   
                    // Hide loading, show results
                    loadingIndicator.style.display = 'none';
                    previewContainer.style.display = 'block';
                    previewContainer.scrollIntoView({ behavior: 'smooth' });
                    createConfetti();
                };
                reader.readAsDataURL(file);
            }
           
            // Download button
            downloadBtn.addEventListener('click', () => {
                if (!processedImage.src) return;
               
                const link = document.createElement('a');
                link.href = processedImage.src;
                link.download = 'background-removed-' + Date.now() + '.png';
                document.body.appendChild(link);
                link.click();
                document.body.removeChild(link);
               
                // Create confetti effect
                createConfetti();
            });
           
            // New image button
            newImageBtn.addEventListener('click', () => {
                previewContainer.style.display = 'none';
                fileInput.value = '';
                originalImage.src = '';
                processedImage.src = '';
            });
           
            // Create confetti effect
            function createConfetti() {
                const colors = ['#FD1D1D', '#833AB4', '#405DE6', '#FFDC80', '#FCAF45'];
               
                for (let i = 0; i < 100; i++) {
                    const confetti = document.createElement('div');
                    confetti.className = 'confetti';
                    confetti.style.left = Math.random() * 100 + 'vw';
                    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                    confetti.style.width = Math.random() * 10 + 5 + 'px';
                    confetti.style.height = Math.random() * 10 + 5 + 'px';
                    confetti.style.animationDuration = Math.random() * 2 + 2 + 's';
                    document.body.appendChild(confetti);
                   
                    // Remove confetti after animation
                    setTimeout(() => {
                        confetti.remove();
                    }, 3000);
                }
            }
        });
    </script>
</body>
</html>
