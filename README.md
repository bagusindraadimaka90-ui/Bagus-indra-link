# Bagus-indra-link
Selamat datang di halaman kecil ku
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Social Links | BAGUS INDRA</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #0a0a0a;
            color: #f0f0f0;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(40, 40, 40, 0.1) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(60, 60, 60, 0.1) 0%, transparent 20%);
            overflow-x: hidden;
        }

        .container {
            max-width: 800px;
            width: 100%;
            text-align: center;
            padding: 40px;
            background: rgba(15, 15, 15, 0.9);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            border: 1px solid rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            animation: fadeIn 1s ease-out;
            position: relative;
        }

        .profile-section {
            margin-bottom: 40px;
        }

        .profile-image-container {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            margin: 0 auto 25px;
            border: 5px solid #333;
            background-color: #1a1a1a;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            transition: transform 0.5s ease, border-color 0.5s ease;
            position: relative;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .profile-image-container:hover {
            transform: scale(1.05);
            border-color: #555;
        }

        .profile-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }

        h1 {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 15px;
            letter-spacing: 2px;
            background: linear-gradient(to right, #fff, #ccc);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-transform: uppercase;
        }

        .tagline {
            color: #ccc;
            font-size: 1.3rem;
            font-weight: 300;
            margin-bottom: 40px;
            letter-spacing: 1px;
            line-height: 1.6;
            padding: 0 30px;
            font-style: italic;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            padding: 15px 0;
        }

        .button-container {
            display: flex;
            flex-direction: column;
            gap: 22px;
            margin-bottom: 40px;
        }

        .social-button {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 18px;
            padding: 20px 30px;
            background: linear-gradient(to right, #222, #111);
            color: #f0f0f0;
            border: none;
            border-radius: 15px;
            font-size: 1.3rem;
            font-weight: 500;
            text-decoration: none;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transform: translateZ(0);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .social-button:active {
            transform: translateY(5px) scale(0.98);
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
        }

        .social-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.5);
        }

        .social-button i {
            font-size: 1.6rem;
            transition: transform 0.3s ease;
            display: inline-block;
            width: 26px;
            text-align: center;
            backface-visibility: hidden;
        }

        .social-button:active i {
            transform: scale(0.9);
        }

        .social-button.youtube {
            background: linear-gradient(to right, #1a1a1a, #0a0a0a);
        }

        .social-button.youtube:hover {
            background: linear-gradient(to right, #ff0000, #cc0000);
        }

        .social-button.tiktok {
            background: linear-gradient(to right, #1a1a1a, #0a0a0a);
        }

        .social-button.tiktok:hover {
            background: linear-gradient(to right, #000000, #333333);
        }

        .social-button.tiktok:hover i {
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.4);
        }

        .social-button.instagram {
            background: linear-gradient(to right, #1a1a1a, #0a0a0a);
        }

        .social-button.instagram:hover {
            background: linear-gradient(to right, #e1306c, #833ab4);
        }

        .store-button {
            background: linear-gradient(to right, #2a2a2a, #1a1a1a);
            color: #fff;
            padding: 20px 30px;
            border: none;
            border-radius: 15px;
            font-size: 1.3rem;
            font-weight: 600;
            text-decoration: none;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 18px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
            border: 1px solid rgba(255, 255, 255, 0.05);
            transform: translateZ(0);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .store-button:active {
            transform: translateY(5px) scale(0.98);
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
        }

        .store-button:hover {
            transform: translateY(-3px);
            background: linear-gradient(to right, #3a3a3a, #2a2a2a);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.5);
        }

        .store-button i {
            font-size: 1.6rem;
            transition: transform 0.3s ease;
            display: inline-block;
            width: 26px;
            backface-visibility: hidden;
        }

        .store-button:active i {
            transform: scale(0.9);
        }

        .footer {
            margin-top: 40px;
            color: #777;
            font-size: 0.9rem;
            letter-spacing: 1.5px;
            text-align: center;
            padding-top: 25px;
            border-top: 1px solid rgba(255, 255, 255, 0.08);
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin-top: 25px;
        }

        .social-icon {
            color: #777;
            font-size: 1.4rem;
            transition: all 0.3s ease;
            width: 45px;
            height: 45px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.05);
            text-decoration: none;
        }

        .social-icon:hover {
            color: #fff;
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.1);
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Responsif */
        @media (max-width: 600px) {
            .container {
                padding: 30px 20px;
                margin: 10px;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .tagline {
                font-size: 1.1rem;
                padding: 12px 15px;
            }
            
            .profile-image-container {
                width: 150px;
                height: 150px;
            }
            
            .social-button, .store-button {
                padding: 18px 22px;
                font-size: 1.15rem;
                gap: 15px;
            }
            
            .social-button i, .store-button i {
                font-size: 1.4rem;
                width: 24px;
            }
            
            .social-links {
                gap: 20px;
            }
            
            .social-icon {
                font-size: 1.3rem;
                width: 40px;
                height: 40px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="profile-section">
            <div class="profile-image-container">
                <!-- FOTO PROFIL DARI YOUTUBE -->
                <img src="https://yt3.googleusercontent.com/ytc/AIdro_mAq9ww1zwYbTTBlpYvjtmI0QSRU6Xa4b-0rA5S8J8=s176-c-k-c0x00ffffff-no-rj" 
                     alt="BAGUS INDRA" 
                     class="profile-image"
                     onerror="this.style.display='none'; document.querySelector('.profile-fallback').style.display='flex';">
                <div class="profile-fallback" style="display: none; width: 100%; height: 100%; align-items: center; justify-content: center; background: linear-gradient(45deg, #222, #333);">
                    <i class="fas fa-user-circle" style="font-size: 70px; color: #666;"></i>
                </div>
            </div>
            
            <h1>BAGUS INDRA</h1>
            
            <p class="tagline">"Selamat datang di halaman kecil ku"</p>
        </div>

        <div class="button-container">
            <!-- LINK YOUTUBE -->
            <a href="https://youtube.com/@indraagantengbgt?si=Mp_7DTqAw6HyUc2A" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-button youtube">
                <i class="fab fa-youtube"></i>
                <span>Subscribe YouTube</span>
            </a>
            
            <!-- LINK TIKTOK -->
            <a href="https://www.tiktok.com/@indraagantengbgt?_r=1&_t=ZS-92D7fohwGDx" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-button tiktok">
                <i class="fab fa-tiktok"></i>
                <span>Follow TikTok</span>
            </a>
            
            <!-- LINK INSTAGRAM -->
            <a href="https://www.instagram.com/bgusinm?igsh=a293aGlmNDVtNXRy" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-button instagram">
                <i class="fab fa-instagram"></i>
                <span>Follow Instagram</span>
            </a>
            
            <!-- LINK TOKO -->
            <a href="https://lynk.id/inibagus" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="store-button">
                <i class="fas fa-store"></i>
                <span>TOKO KU</span>
            </a>
        </div>

        <div class="social-links">
            <a href="https://youtube.com/@indraagantengbgt?si=Mp_7DTqAw6HyUc2A" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-icon">
                <i class="fab fa-youtube"></i>
            </a>
            <a href="https://www.tiktok.com/@indraagantengbgt?_r=1&_t=ZS-92D7fohwGDx" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-icon">
                <i class="fab fa-tiktok"></i>
            </a>
            <a href="https://www.instagram.com/bgusinm?igsh=a293aGlmNDVtNXRy" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-icon">
                <i class="fab fa-instagram"></i>
            </a>
            <a href="https://lynk.id/inibagus" 
               target="_blank" 
               rel="noopener noreferrer" 
               class="social-icon">
                <i class="fas fa-store"></i>
            </a>
        </div>

        <div class="footer">
            <p>© 2024 BAGUS INDRA. All rights reserved.</p>
            <p style="margin-top: 10px; font-size: 0.85rem; color: #666;">"Selamat datang di halaman kecil ku"</p>
        </div>
    </div>

    <script>
        // SCRIPT SEDERHANA TANPA MENGANGGU LINK
        document.addEventListener('DOMContentLoaded', function() {
            const buttons = document.querySelectorAll('.social-button, .store-button, .social-icon');
            
            buttons.forEach(button => {
                // Efek tekan sederhana tanpa mencegah link
                button.addEventListener('mousedown', function() {
                    this.style.transform = 'translateY(5px) scale(0.98)';
                    this.style.boxShadow = '0 2px 6px rgba(0, 0, 0, 0.2)';
                    
                    const icon = this.querySelector('i');
                    if (icon) {
                        icon.style.transform = 'scale(0.9)';
                    }
                });
                
                button.addEventListener('mouseup', function() {
                    this.style.transform = '';
                    this.style.boxShadow = '';
                    
                    const icon = this.querySelector('i');
                    if (icon) {
                        icon.style.transform = '';
                    }
                });
                
                button.addEventListener('mouseleave', function() {
                    this.style.transform = '';
                    this.style.boxShadow = '';
                    
                    const icon = this.querySelector('i');
                    if (icon) {
                        icon.style.transform = '';
                    }
                });
                
                // Untuk touch devices - TANPA preventDefault()
                button.addEventListener('touchstart', function() {
                    this.style.transform = 'translateY(5px) scale(0.98)';
                    this.style.boxShadow = '0 2px 6px rgba(0, 0, 0, 0.2)';
                    
                    const icon = this.querySelector('i');
                    if (icon) {
                        icon.style.transform = 'scale(0.9)';
                    }
                });
                
                button.addEventListener('touchend', function() {
                    setTimeout(() => {
                        this.style.transform = '';
                        this.style.boxShadow = '';
                        
                        const icon = this.querySelector('i');
                        if (icon) {
                            icon.style.transform = '';
                        }
                    }, 150);
                });
            });
            
            // Animasi untuk profile image container
            const profileContainer = document.querySelector('.profile-image-container');
            setTimeout(() => {
                profileContainer.style.transition = 'transform 0.7s ease';
                profileContainer.style.transform = 'scale(1.08)';
                setTimeout(() => {
                    profileContainer.style.transform = 'scale(1)';
                }, 400);
            }, 500);
            
            // Animasi ikon sosial di footer
            const socialIcons = document.querySelectorAll('.social-icon');
            socialIcons.forEach((icon, index) => {
                setTimeout(() => {
                    icon.style.opacity = '0';
                    icon.style.transform = 'translateY(15px) scale(0.8)';
                    
                    setTimeout(() => {
                        icon.style.transition = 'all 0.6s ease';
                        icon.style.opacity = '1';
                        icon.style.transform = 'translateY(0) scale(1)';
                    }, 100);
                }, 800 + (index * 150));
            });
            
            // Preload gambar profil
            const profileImg = new Image();
            profileImg.src = 'https://yt3.googleusercontent.com/ytc/AIdro_mAq9ww1zwYbTTBlpYvjtmI0QSRU6Xa4b-0rA5S8J8=s176-c-k-c0x00ffffff-no-rj';
            profileImg.onload = function() {
                console.log('Foto profil berhasil dimuat');
            };
            profileImg.onerror = function() {
                console.log('Foto profil gagal dimuat, menggunakan fallback');
                document.querySelector('.profile-image').style.display = 'none';
                document.querySelector('.profile-fallback').style.display = 'flex';
            };
        });
    </script>
</body>
</html>
