---
title: "Giới Thiệu"
url: "/about"
layout: "single"
---

<header class="luxury-header">
    <nav class="luxury-nav">
        <div class="luxury-logo">
            <a href="/">LÊ QUỐC TRỌNG</a>
        </div>
        <ul class="luxury-menu">
            <li><a href="/">TRANG CHỦ</a></li>
            <li><a href="/about" class="active">GIỚI THIỆU</a></li>
            <li><a href="/posts">BLOG</a></li>
            <li><a href="/contact">LIÊN HỆ</a></li>
        </ul>
    </nav>
</header>

<div class="luxury-split-screen">
    <div class="luxury-text-side">
        <div class="luxury-content-box">
            <p class="luxury-tag animated-item delay-1">LỜI TỰ BẠCH</p>
            <h1 class="luxury-title">
                <div class="hider"><span class="animated-item delay-2">GIỚI</span></div>
                <div class="hider"><span class="animated-item delay-3">THIỆU.</span></div>
            </h1>
            
            <div class="luxury-description animated-item delay-4">
                <h3 class="job-tag">LÊ QUỐC TRỌNG — HUTECH IT STUDENT</h3>
                <p>Chào bạn, mình hiện đang là sinh viên chuyên ngành <strong>Công Nghệ Thông Tin</strong>. Hành trình của mình được xây đắp từ những sự tò mò đơn sơ nhất về thế giới kỹ thuật số.</p>
                <p>Mình chọn đi sâu vào <strong>Lập trình mạng</strong> và <strong>Java</strong>. Những đêm thức trắng sửa lỗi đã giữ chân mình lại với nghề.</p>
            </div>

            <div class="luxury-quote animated-item delay-5">
                "Giữ tâm thế của người mới bắt đầu."
            </div>
        </div>
    </div>

    <div class="luxury-image-side">
        <div class="image-wrapper animated-image">
            <img src="anh3.jpg" alt="Lê Quốc Trọng" onerror="this.src='/LeQuocTrong_Blog/anh3.jpg'">
        </div>
    </div>
</div>

<style>
    /* 1. DIỆT RÁC THEME TRIỆT ĐỂ */
    footer, .footer, .nav, .header, .logo-switches, #top-link, header.page-header, .breadcrumbs, .post-header { 
        display: none !important; 
    }
    body, html { 
        background: #fff !important; margin: 0; padding: 0; overflow: hidden !important; 
    }

    /* 2. MENU ĐỒNG BỘ TRANG CHỦ */
    .luxury-header {
        position: fixed; top: 0; left: 0; width: 100%; z-index: 9999;
        background: #fff; padding: 25px 0; display: flex; justify-content: center;
    }
    .luxury-nav { 
        width: 100%; max-width: 1300px; display: flex; justify-content: space-between; 
        align-items: center; padding: 0 100px; 
    }
    .luxury-logo a { font-family: 'Montserrat', sans-serif; font-size: 20px; font-weight: 900; color: #000; text-decoration: none; letter-spacing: -1px; }
    .luxury-menu { display: flex !important; list-style: none !important; gap: 40px; margin: 0; padding: 0; }
    .luxury-menu a { color: #000; text-decoration: none; font-family: 'Montserrat', sans-serif; font-size: 13px; font-weight: 700; text-transform: uppercase; }
    .luxury-menu a.active { border-bottom: 2.5px solid #000; padding-bottom: 3px; }

    /* 3. LAYOUT CHIA ĐÔI */
    .luxury-split-screen { display: flex; width: 100vw; height: 100vh; background: #fff; }
    
    .luxury-text-side { 
        flex: 4.5; display: flex; justify-content: flex-end; align-items: center; 
        padding-right: 80px; background: #fff;
    }
    .luxury-content-box { max-width: 480px; width: 100%; }

    .luxury-title { 
        font-family: 'Montserrat', sans-serif !important; 
        font-size: 75px; font-weight: 900; line-height: 0.82; 
        margin: 0 0 35px 0; text-transform: uppercase; letter-spacing: -5px; color: #1a1a1a;
    }
    .hider { overflow: hidden; }

    .luxury-tag { font-family: 'Montserrat', sans-serif; font-size: 10px; font-weight: 600; color: #bbb; letter-spacing: 5px; margin-bottom: 15px; }
    .luxury-description { border-left: 5px solid #1a1a1a; padding-left: 25px; margin-top: 30px; }
    .job-tag { font-family: 'Montserrat', sans-serif; font-size: 14px; font-weight: 900; margin-bottom: 15px; color: #000; }
    .luxury-description p { font-family: 'Montserrat', sans-serif; font-size: 13px; line-height: 1.6; color: #666; margin-bottom: 10px; }
    .luxury-quote { margin-top: 25px; font-family: 'Montserrat', sans-serif; font-style: italic; font-size: 13px; font-weight: 600; color: #999; }

    /* 4. FIX LẤY THÂN NGƯỜI */
    .luxury-image-side { flex: 5.5; background: #f9f9f9; overflow: hidden; }
    .image-wrapper { width: 100%; height: 100%; }
    .image-wrapper img { 
        width: 100%; height: 100%; object-fit: cover; 
        object-position: center 15%; /* Lấy từ ngực trở lên */
        display: block; 
    }

    /* 5. ANIMATIONS */
    @keyframes revealUp { from { transform: translateY(110%); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
    .animated-item { display: inline-block; animation: revealUp 1s cubic-bezier(0.19, 1, 0.22, 1) forwards; opacity: 0; }
    .animated-image { opacity: 0; animation: fadeIn 1.5s ease forwards; animation-delay: 0.4s; }
    @keyframes fadeIn { to { opacity: 1; } }
    .delay-1 { animation-delay: 0.1s; } .delay-2 { animation-delay: 0.2s; }
    .delay-3 { animation-delay: 0.3s; } .delay-4 { animation-delay: 0.4s; }
    .delay-5 { animation-delay: 0.5s; }
</style>