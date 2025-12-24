---
title: "Giới Thiệu"
url: "/about"
layout: "single"
---

<div class="ultimate-about-wrapper">
    <header class="ultimate-nav-bar">
        <div class="nav-content">
            <a href="/" class="nav-logo">LÊ QUỐC TRỌNG</a>
            <ul class="nav-links">
                <li><a href="/">TRANG CHỦ</a></li>
                <li><a href="/about" class="active">GIỚI THIỆU</a></li>
                <li><a href="/posts">BLOG</a></li>
                <li><a href="/contact">LIÊN HỆ</a></li>
            </ul>
        </div>
    </header>

    <div class="split-screen">
        <div class="left-text">
            <div class="content-container">
                <p class="tag animated-up delay-1">LỜI TỰ BẠCH</p>
                <h1 class="hero-title">
                    <div class="mask"><span class="animated-up delay-2">GIỚI</span></div>
                    <div class="mask"><span class="animated-up delay-3">THIỆU.</span></div>
                </h1>
                
                <div class="desc-box animated-up delay-4">
                    <h3 class="job">LÊ QUỐC TRỌNG — HUTECH IT STUDENT</h3>
                    <p>Chào bạn, mình là sinh viên <strong>Công Nghệ Thông Tin</strong>. Hành trình của mình bắt đầu từ sự tò mò về thế giới số.</p>
                    <p>Mình đam mê <strong>Lập trình mạng</strong> và <strong>Java</strong>. Những đêm thức trắng đã giúp mình trưởng thành hơn với nghề.</p>
                </div>

                <div class="quote animated-up delay-5">
                    "Giữ tâm thế của người mới bắt đầu."
                </div>
            </div>
        </div>

        <div class="right-image">
            <div class="img-wrapper animated-fade">
                <img src="anh3.jpg" alt="Lê Quốc Trọng" onerror="this.src='/LeQuocTrong_Blog/anh3.jpg'">
            </div>
        </div>
    </div>
</div>

<style>
    /* 1. DIỆT SẠCH TAM GIÁC XANH VÀ RÁC THEME */
    header, footer, .header, .footer, .nav, #top-link, .top-link, .logo-switches, 
    .breadcrumbs, header.page-header, .post-header { 
        display: none !important; 
        visibility: hidden !important;
        opacity: 0 !important;
        height: 0 !important;
        width: 0 !important;
        pointer-events: none !important;
    }

    /* TRIỆT TIÊU SCROLL ĐỂ KHÔNG HIỆN TAM GIÁC */
    html, body { 
        background: #ffffff !important; 
        margin: 0 !important; 
        padding: 0 !important; 
        overflow: hidden !important; 
        height: 100vh !important;
    }

    /* 2. MENU ĐỒNG BỘ TRANG CHỦ */
    .ultimate-nav-bar {
        position: fixed !important; top: 0 !important; left: 0 !important; 
        width: 100% !important; z-index: 99999 !important;
        background: #fff !important; padding: 25px 0 !important; 
        display: flex !important; justify-content: center !important;
    }
    .nav-content { 
        width: 100% !important; max-width: 1300px !important; 
        display: flex !important; justify-content: space-between !important; 
        align-items: center !important; padding: 0 100px !important; 
    }
    .nav-logo { font-family: 'Montserrat', sans-serif !important; font-size: 20px !important; font-weight: 900 !important; color: #000 !important; text-decoration: none !important; letter-spacing: -1px !important; }
    .nav-links { display: flex !important; list-style: none !important; gap: 40px !important; margin: 0 !important; padding: 0 !important; }
    .nav-links a { color: #000 !important; text-decoration: none !important; font-family: 'Montserrat', sans-serif !important; font-size: 13px !important; font-weight: 700 !important; text-transform: uppercase !important; }
    .nav-links a.active { border-bottom: 2.5px solid #000 !important; padding-bottom: 3px !important; }

    /* 3. LAYOUT CHIA ĐÔI */
    .ultimate-about-wrapper { width: 100vw !important; height: 100vh !important; background: #fff !important; }
    .split-screen { display: flex !important; width: 100% !important; height: 100% !important; }
    
    .left-text { flex: 4.5 !important; display: flex !important; justify-content: flex-end !important; align-items: center !important; padding-right: 80px !important; }
    .content-container { max-width: 480px !important; width: 100% !important; }

    .hero-title { font-family: 'Montserrat', sans-serif !important; font-size: 75px !important; font-weight: 900 !important; line-height: 0.82 !important; margin: 0 0 35px 0 !important; text-transform: uppercase !important; letter-spacing: -5px !important; color: #1a1a1a !important; }
    .mask { overflow: hidden !important; }

    .tag { font-family: 'Montserrat', sans-serif !important; font-size: 10px !important; font-weight: 600 !important; color: #bbb !important; letter-spacing: 5px !important; margin-bottom: 15px !important; }
    .desc-box { border-left: 5px solid #1a1a1a !important; padding-left: 25px !important; margin-top: 30px !important; }
    .job { font-family: 'Montserrat', sans-serif !important; font-size: 14px !important; font-weight: 900 !important; margin-bottom: 15px !important; color: #000 !important; }
    .desc-box p { font-family: 'Montserrat', sans-serif !important; font-size: 13px !important; line-height: 1.6 !important; color: #666 !important; margin-bottom: 10px !important; }
    .quote { margin-top: 25px !important; font-family: 'Montserrat', sans-serif !important; font-style: italic !important; font-size: 13px !important; font-weight: 600 !important; color: #999 !important; }

    /* 4. FIX LẤY THÂN NGƯỜI */
    .right-image { flex: 5.5 !important; background: #f9f9f9 !important; overflow: hidden !important; }
    .img-wrapper { width: 100% !important; height: 100% !important; }
    .img-wrapper img { width: 100% !important; height: 100% !important; object-fit: cover !important; object-position: center 15% !important; display: block !important; }

    /* 5. ANIMATIONS */
    @keyframes revealUp { from { transform: translateY(110%); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
    .animated-up { display: inline-block !important; animation: revealUp 1s cubic-bezier(0.19, 1, 0.22, 1) forwards !important; opacity: 0 !important; }
    .animated-fade { opacity: 0 !important; animation: fadeIn 1.5s ease forwards !important; animation-delay: 0.4s !important; }
    @keyframes fadeIn { to { opacity: 1 !important; } }
    .delay-1 { animation-delay: 0.1s !important; } .delay-2 { animation-delay: 0.2s !important; }
    .delay-3 { animation-delay: 0.3s !important; } .delay-4 { animation-delay: 0.4s !important; }
    .delay-5 { animation-delay: 0.5s !important; }
</style>