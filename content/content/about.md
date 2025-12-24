---
title: "About Me"
layout: "page"
url: "/about"
summary: "Professional Profile"
showToc: false
showPostNavLinks: false
showSocial: false
showBreadcrumbs: false
showReadingTime: false
showAuthor: false
showDate: false
editPost:
  disabled: true
---

<div class="story-container">
  
  <div class="visual-side">
    <div class="photo-frame animated-element delay-1">
      <img src="anh3.jpg" alt="Lê Quốc Trọng" onerror="this.src='/LeQuocTrong_Blog/anh3.jpg'">
    </div>
  </div>

  <div class="text-side">
    <div class="text-wrapper">
      <h4 class="intro-label animated-element delay-2">LỜI TỰ BẠCH</h4>
      <h1 class="main-title animated-element delay-3">Lê Quốc Trọng</h1>
      <p class="subtitle animated-element delay-4">Một sinh viên IT bình thường tại HUTECH</p>
      
      <div class="separator animated-element delay-5"></div>

      <div class="narrative-content">
        <p class="animated-element delay-6">Chào bạn, cảm ơn vì đã ghé thăm góc nhỏ này. Mình tên là Lê Quốc Trọng, hiện đang là sinh viên chuyên ngành <strong>Công Nghệ Thông Tin</strong>. Thú thật, mình không phải là một "ngôi sao" trong lớp, cũng chẳng phải thiên tài có thể viết code nhoay nhoáy từ năm cấp hai. Hành trình của mình bắt đầu khá muộn và chậm rãi, được xây đắp từ những sự tò mò đơn sơ nhất về thế giới kỹ thuật số.</p>

        <p class="animated-element delay-7">Mình chọn đi sâu vào <strong>Lập trình mạng (Network Programming)</strong> và <strong>Java&JavaScript</strong> - những mảng kiến thức khô khan nhưng đầy tính logic. Có những đêm thức trắng chỉ để sửa một lỗi Socket ngớ ngẩn, hay những lúc muốn bỏ cuộc vì sự phức tạp của các luồng dữ liệu. Nhưng chính những khoảnh khắc "vỡ lẽ" sau khi sửa được lỗi đã giữ chân mình lại với nghề.</p>

        <p class="animated-element delay-8">Trang blog này ra đời không mang tham vọng dạy dỗ ai cả. Nó đơn thuần là cuốn nhật ký ghi chép lại những gì mình may mắn học được, và cả những sai lầm ngớ ngẩn mình đã mắc phải. Mình tin rằng, thừa nhận sự thiếu sót của bản thân chính là cách nhanh nhất để trưởng thành.</p>
      </div>

      <div class="signature-quote animated-element delay-9">
        "Giữ tâm thế của người mới bắt đầu, để luôn khao khát học hỏi."
      </div>
    </div>
  </div>

</div>

<style>
/* 1. XÓA NỀN XÁM CỦA MENU MẶC ĐỊNH THEME */
.nav, header, .header, nav, body, .main, main {
    background-color: #ffffff !important; 
    background: #ffffff !important;
}

/* Import Font */
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,400&family=Mulish:wght@300;400;600&display=swap');

/* XÓA CÁC THÀNH PHẦN THỪA CỦA PAPERMOD TRÊN TRANG NÀY */
header.page-header, .post-title, .post-meta, .post-footer, .breadcrumbs, .share-buttons, .toc, footer.page-footer { 
  display: none !important; 
}

/* 2. KHUNG BAO NGOÀI */
.story-container {
  width: 100vw;
  position: relative;
  left: 50%;
  right: 50%;
  margin-left: -50vw;
  margin-right: -50vw;
  display: flex;
  min-height: 100vh;
  background: #fff;
  overflow: hidden;
  /* Đẩy nội dung xuống dưới thanh Menu ngang */
  padding-top: 80px; 
}

/* 3. CỘT ẢNH */
.visual-side {
  flex: 5; 
  background-color: #f8f9fa;
  display: flex;
  justify-content: flex-end; 
  align-items: flex-start; 
  padding-top: 60px; 
  padding-right: 60px;
}

.photo-frame {
  width: 100%; 
  max-width: 380px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.08);
  border-radius: 4px;
  background: #fff;
  padding: 10px;
}

.photo-frame img {
  width: 100%;
  height: auto;
  display: block;
  filter: grayscale(20%);
  transition: 0.5s;
}

.photo-frame:hover img {
    filter: grayscale(0%);
}

/* 4. CỘT CHỮ */
.text-side {
  flex: 6; 
  display: flex;
  padding: 60px 80px; 
  background: #fff;
}

.text-wrapper { max-width: 700px; }

.main-title {
  font-family: 'Playfair Display', serif;
  font-size: 3.5rem;
  color: #222;
  margin-bottom: 10px;
}

/* ANIMATION - GIỮ NGUYÊN FORM CỦA MÀY */
@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
}

.animated-element {
    opacity: 0;
    animation: fadeInUp 0.8s ease-out forwards;
}

.delay-1 { animation-delay: 0.1s; }
.delay-2 { animation-delay: 0.2s; }
.delay-3 { animation-delay: 0.3s; }
.delay-4 { animation-delay: 0.4s; }
.delay-5 { animation-delay: 0.5s; }
.delay-6 { animation-delay: 0.6s; }
.delay-7 { animation-delay: 0.7s; }
.delay-8 { animation-delay: 0.8s; }
.delay-9 { animation-delay: 0.9s; }

@media (max-width: 900px) {
  .story-container { flex-direction: column-reverse; height: auto; }
  .visual-side, .text-side { padding: 40px 20px; }
}
</style>