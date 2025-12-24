---
title: "Liên Hệ"
layout: "page"
url: "/contact"
---

<script>
    document.addEventListener("DOMContentLoaded", function() {
        const trash = document.querySelectorAll('header:not(.ultimate-nav-bar), footer, .top-link, #top-link, .logo-switches, .breadcrumbs, .page-header');
        trash.forEach(el => el.remove());
        document.body.style.overflow = 'hidden';
    });
</script>

<div class="ultimate-contact-wrapper">
    <header class="ultimate-nav-bar">
        <div class="nav-content">
            <a href="/" class="nav-logo">LÊ QUỐC TRỌNG</a>
            <ul class="nav-links">
                <li><a href="/">TRANG CHỦ</a></li>
                <li><a href="/about">GIỚI THIỆU</a></li>
                <li><a href="/posts">BLOG</a></li>
                <li><a href="/contact" class="active">LIÊN HỆ</a></li>
            </ul>
        </div>
    </header>

    <div class="split-screen">
        <div class="left-text">
            <div class="content-container">
                <p class="tag animated-up delay-1">GET IN TOUCH</p>
                <h1 class="hero-title">
                    <div class="mask"><span class="animated-up delay-2">LIÊN</span></div>
                    <div class="mask"><span class="animated-up delay-3">HỆ.</span></div>
                </h1>
                
                <div class="contact-methods-list animated-up delay-4">
                    <div class="method-box">
                        <span class="method-label">EMAIL</span>
                        <a href="mailto:qctrong136@gmail.com" class="method-value">qctrong136@gmail.com</a>
                    </div>
                    <div class="method-box">
                        <span class="method-label">PHONE</span>
                        <span class="method-value">+84 36 773 8269</span>
                    </div>
                    <div class="method-box">
                        <span class="method-label">SOCIAL</span>
                        <div class="social-flex">
                            <a href="https://www.facebook.com/qctrongikbao" target="_blank">FACEBOOK</a>
                            <a href="https://www.instagram.com/leequoctronggg.136/" target="_blank">INSTAGRAM</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="right-form-side">
            <div class="form-container animated-fade">
                <form action="https://formspree.io/f/xvzpylgw" method="POST" class="luxury-form">
                    <div class="input-group">
                        <input type="text" name="name" placeholder="TÊN CỦA BẠN" required>
                    </div>
                    <div class="input-group">
                        <input type="email" name="email" placeholder="EMAIL" required>
                    </div>
                    <div class="input-group">
                        <textarea name="message" rows="4" placeholder="NỘI DUNG TIN NHẮN" required></textarea>
                    </div>
                    <button type="submit" class="submit-btn">GỬI NGAY —</button>
                </form>
            </div>
        </div>
    </div>
</div>

<style>
    /* 1. DIỆT RÁC THEME */
    html, body { 
        background: #ffffff !important; 
        margin: 0 !important; padding: 0 !important; 
        overflow: hidden !important; height: 100vh !important;
    }

    /* 2. MENU ĐỒNG BỘ */
    .ultimate-nav-bar {
        position: fixed !important; top: 0 !important; left: 0 !important; width: 100% !important; z-index: 99999 !important;
        background: #fff !important; padding: 25px 0 !important; display: flex !important; justify-content: center !important;
    }
    .nav-content { 
        width: 100% !important; max-width: 1300px !important; display: flex !important; justify-content: space-between !important; 
        align-items: center !important; padding: 0 100px !important; 
    }
    .nav-logo { font-family: 'Montserrat', sans-serif !important; font-size: 20px !important; font-weight: 900 !important; color: #000 !important; text-decoration: none !important; letter-spacing: -1px !important; }
    .nav-links { display: flex !important; list-style: none !important; gap: 40px !important; margin: 0 !important; padding: 0 !important; }
    .nav-links a { color: #000 !important; text-decoration: none !important; font-family: 'Montserrat', sans-serif !important; font-size: 13px !important; font-weight: 700 !important; text-transform: uppercase !important; }
    .nav-links a.active { border-bottom: 2.5px solid #000 !important; padding-bottom: 3px !important; }

    /* 3. LAYOUT CHIA ĐÔI */
    .ultimate-contact-wrapper { width: 100vw !important; height: 100vh !important; background: #fff !important; }
    .split-screen { display: flex !important; width: 100% !important; height: 100% !important; }
    
    .left-text { flex: 4.5 !important; display: flex !important; justify-content: flex-end !important; align-items: center !important; padding-right: 80px !important; }
    .content-container { max-width: 480px !important; width: 100% !important; }

    .hero-title { font-family: 'Montserrat', sans-serif !important; font-size: 75px !important; font-weight: 900 !important; line-height: 0.82 !important; margin: 0 0 45px 0 !important; text-transform: uppercase !important; letter-spacing: -5px !important; color: #1a1a1a !important; }
    .mask { overflow: hidden !important; }
    .tag { font-family: 'Montserrat', sans-serif !important; font-size: 10px !important; font-weight: 600 !important; color: #bbb !important; letter-spacing: 5px !important; margin-bottom: 15px !important; }

    /* CONTACT INFO */
    .method-box { margin-bottom: 30px; }
    .method-label { display: block; font-family: 'Montserrat', sans-serif; font-size: 10px; font-weight: 900; color: #111; margin-bottom: 8px; letter-spacing: 2px; }
    .method-value, .social-flex a { font-family: 'Montserrat', sans-serif; font-size: 14px; font-weight: 500; color: #666; text-decoration: none; transition: 0.3s; }
    .method-value:hover, .social-flex a:hover { color: #000; }
    .social-flex { display: flex; gap: 20px; }

    /* 4. FORM SIDE ĐẲNG CẤP */
    .right-form-side { flex: 5.5 !important; background: #f9f9f9 !important; display: flex; justify-content: center; align-items: center; }
    .form-container { width: 100%; max-width: 500px; padding: 40px; }
    
    .luxury-form .input-group { margin-bottom: 30px; border-bottom: 1px solid #ddd; }
    .luxury-form input, .luxury-form textarea { 
        width: 100%; background: transparent; border: none; padding: 15px 0;
        font-family: 'Montserrat', sans-serif; font-size: 12px; font-weight: 600; outline: none; text-transform: uppercase;
    }
    .luxury-form textarea { resize: none; text-transform: none; }
    .submit-btn { 
        background: #111; color: #fff; border: none; padding: 18px 40px; 
        font-family: 'Montserrat', sans-serif; font-size: 12px; font-weight: 900; 
        cursor: pointer; transition: 0.4s; letter-spacing: 2px; 
    }
    .submit-btn:hover { background: #000; transform: translateX(10px); }

    /* 5. ANIMATIONS */
    @keyframes revealUp { from { transform: translateY(110%); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
    .animated-up { display: inline-block !important; animation: revealUp 1s cubic-bezier(0.19, 1, 0.22, 1) forwards !important; opacity: 0 !important; }
    .animated-fade { opacity: 0 !important; animation: fadeIn 1.5s ease forwards !important; animation-delay: 0.4s !important; }
    @keyframes fadeIn { to { opacity: 1 !important; } }
    .delay-1 { animation-delay: 0.1s !important; } .delay-2 { animation-delay: 0.2s !important; }
    .delay-3 { animation-delay: 0.3s !important; } .delay-4 { animation-delay: 0.4s !important; }
    .delay-5 { animation-delay: 0.5s !important; }
</style>