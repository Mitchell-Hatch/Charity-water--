<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Charity: Water - Your Support is Their Future</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #7db4c7 0%, #5a9bb5 100%);
            min-height: 100vh;
            padding: 40px 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: linear-gradient(135deg, #7db4c7 0%, #5a9bb5 100%);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        .header {
            padding: 40px;
            color: white;
        }
        
        .logo {
            display: flex;
            align-items: center;
            margin-bottom: 30px;
            font-size: 28px;
            font-weight: 300;
            letter-spacing: 3px;
        }
        
        .logo-icon {
            background: #FFD700;
            width: 45px;
            height: 45px;
            margin-right: 15px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: #333;
            font-size: 24px;
        }
        
        .main-headline {
            font-size: 48px;
            font-weight: bold;
            color: #FFD700;
            line-height: 1.2;
            margin-bottom: 40px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }
        
        .content-section {
            display: flex;
            align-items: center;
            gap: 60px;
            padding: 0 40px 40px;
        }
        
        .text-content {
            flex: 1;
            color: white;
        }
        
        .quote-text {
            font-size: 32px;
            line-height: 1.4;
            margin-bottom: 40px;
            font-weight: 300;
            color: #2c5f72;
        }
        
        .cta-button {
            display: inline-block;
            background: transparent;
            color: #ff6b4a;
            font-size: 36px;
            font-weight: bold;
            text-decoration: underline;
            text-underline-offset: 8px;
            text-decoration-thickness: 4px;
            padding: 20px 0;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        
        .cta-button:hover {
            color: #ff4521;
            text-decoration-thickness: 6px;
            transform: translateY(-2px);
        }
        
        .image-content {
            flex: 1;
            position: relative;
        }
        
        .main-image {
            width: 100%;
            height: 400px;
            object-fit: cover;
            border-radius: 15px;
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        
        @media (max-width: 768px) {
            .content-section {
                flex-direction: column;
                gap: 30px;
            }
            
            .main-headline {
                font-size: 32px;
            }
            
            .quote-text {
                font-size: 24px;
            }
            
            .cta-button {
                font-size: 28px;
            }
            
            .header, .content-section {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <div class="logo">
                <div class="logo-icon">🚰</div>
                <span>charity: water</span>
            </div>
            
            <h1 class="main-headline">
                "Your Support is Their Future: Donate to Charity: Water to See Change You Can Track and Trust"
            </h1>
        </header>
        
        <div class="content-section">
            <div class="text-content">
                <p class="quote-text">
                    "Partner with Charity: Water, we provide clean water access—and show you the real-world impact of every donation."
                </p>
                
                <button class="cta-button" onclick="handleDonation()">
                    CLICK HERE TO<br>DONATE
                </button>
            </div>
            
            <div class="image-content">
                <img src="https://images.unsplash.com/photo-1578662996442-48f60103fc96?w=500&h=400&fit=crop&crop=faces" 
                     alt="Young person smiling while holding a glass of clean water" 
                     class="main-image">
            </div>
        </div>
    </div>
    
    <script>
        function handleDonation() {
            // In a real implementation, this would redirect to the donation page
            alert('Thank you for your interest in supporting clean water access! This would redirect to the donation page.');
            console.log('Donation button clicked - would redirect to donation form');
        }
        
        // Add some interactive hover effects
        document.addEventListener('DOMContentLoaded', function() {
            const button = document.querySelector('.cta-button');
            const image = document.querySelector('.main-image');
            
            // Add subtle animation to the image on load
            setTimeout(() => {
                image.style.transform = 'scale(1.02)';
                image.style.transition = 'transform 0.5s ease';
            }, 500);
            
            // Reset image scale on button hover
            button.addEventListener('mouseenter', () => {
                image.style.transform = 'scale(1)';
            });
            
            button.addEventListener('mouseleave', () => {
                image.style.transform = 'scale(1.02)';
            });
        });
    </script>
</body>
</html>
