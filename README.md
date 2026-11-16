<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>nhatvu.com - CÔNG TY TNHH MỘT THÀNH VIÊN XD &amp; TM NHẤT VŨ</title>
  <meta name="description" content="CÔNG TY TNHH MỘT THÀNH VIÊN XD & TM NHẤT VŨ - Chuyên phân phối Sơn Jotun, Dulux, Thiết bị vệ sinh, Gạch men, Ngói lợp, Bồn nước, Bình nóng lạnh, Keo dán gạch chính hãng tại 65 Nguyễn Quang Diêu, Hòa Xuân, Đà Nẵng." />

  <!-- Open Graph Thumbnail là Logo trang web khi gửi link chia sẻ -->
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://nhatvu.com/" />
  <meta property="og:title" content="nhatvu.com - CÔNG TY TNHH MTV XD & TM NHẤT VŨ" />
  <meta property="og:description" content="Tổng kho Sơn, Gạch men, Thiết bị vệ sinh, Ngói lợp, Bồn nước, Bình nóng lạnh, Phụ gia chống thấm uy tín tại Đà Nẵng. Hotline: 0905.343.016 - 0905.327.257" />
  <meta property="og:image" content="https://placehold.co/1200x630/0b3b68/ffffff?text=LOGO+NHAT+VU+-+XD+%26+TM+NHATVU.COM" />

  <!-- Google Fonts: Inter & Montserrat chuẩn Flatsome -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet" />

  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              primary: '#0B3B68',    /* Xanh Navy đậm theo màu Logo Nhất Vũ */
              secondary: '#14558F',  /* Xanh dương trung */
              accent: '#E65100',     /* Cam Đỏ Xây Dựng nổi bật theo Logo */
              light: '#F4F7FA',      /* Nền xám xanh nhạt chuẩn Flatsome */
            }
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
          }
        }
      }
    }
  </script>

  <style>
    /* Khóa tràn viền ngang tuyệt đối, không lệch phải */
    *, *::before, *::after {
      box-sizing: border-box;
    }
    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      max-width: 100vw;
      overflow-x: hidden;
      font-family: 'Inter', sans-serif;
      background-color: #f5f7fa;
      color: #222;
      scroll-behavior: smooth;
    }

    /* Chiều ngang giao diện trên máy tính bằng 95% kích thước màn hình máy tính */
    .flatsome-container {
      width: 96%;
      max-width: 96%;
      margin-left: auto;
      margin-right: auto;
    }
    @media (min-width: 1024px) {
      .flatsome-container {
        width: 95%;
        max-width: 95%;
        margin-left: auto;
        margin-right: auto;
      }
    }

    /* Tối ưu Menu Danh mục trên máy tính: chữ nhỏ gọn, viết liền trên 1 hàng, không gãy dòng tên danh mục */
    .desktop-cat-nav {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: flex-start;
      gap: 2px 6px;
    }
    .desktop-cat-link {
      white-space: nowrap;
      font-size: 12.5px;
      font-weight: 700;
      padding: 8px 10px;
      border-radius: 4px;
      transition: all 0.2s ease;
      display: inline-flex;
      align-items: center;
      gap: 5px;
      letter-spacing: -0.01em;
    }
    .desktop-cat-link:hover, .desktop-cat-link.active {
      background-color: #E65100;
      color: #ffffff;
    }

    /* Dropdown Submenu kiểu Flatsome */
    .has-dropdown {
      position: relative;
    }
    .nav-dropdown {
      position: absolute;
      top: 100%;
      left: 0;
      min-width: 210px;
      background: #ffffff;
      color: #1e293b;
      box-shadow: 0 10px 25px rgba(0,0,0,0.12);
      border-top: 3px solid #E65100;
      border-radius: 0 0 6px 6px;
      padding: 6px 0;
      opacity: 0;
      visibility: hidden;
      transform: translateY(8px);
      transition: all 0.2s ease;
      z-index: 60;
    }
    .has-dropdown:hover .nav-dropdown {
      opacity: 1;
      visibility: visible;
      transform: translateY(0);
    }
    .nav-dropdown a {
      display: block;
      padding: 7px 14px;
      font-size: 12.5px;
      font-weight: 500;
      color: #334155;
      white-space: nowrap;
      border-bottom: 1px solid #f1f5f9;
    }
    .nav-dropdown a:last-child {
      border-bottom: none;
    }
    .nav-dropdown a:hover {
      background-color: #f8fafc;
      color: #E65100;
      padding-left: 18px;
    }

    /* Bố cục ô sản phẩm chuẩn Flatsome */
    .product-small.box {
      background: #ffffff;
      border: 1px solid #e5e7eb;
      border-radius: 6px;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      height: 100%;
      position: relative;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }
    .product-small.box:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(11, 59, 104, 0.1);
      border-color: #cbd5e1;
    }

    /* Nút % giảm giá góc trên bên trái chuẩn Flatsome */
    .flatsome-discount-badge {
      position: absolute;
      top: 8px;
      left: 8px;
      z-index: 10;
      background-color: #E65100;
      color: #ffffff;
      font-weight: 700;
      font-size: 11.5px;
      width: 38px;
      height: 38px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 2px 6px rgba(230, 81, 0, 0.35);
      line-height: 1;
      pointer-events: none;
    }

    /* Tên sản phẩm hiển thị đầy đủ, không bị tràn hoặc cắt mất chữ */
    .product-title-full {
      font-size: 13px;
      line-height: 1.42;
      font-weight: 600;
      color: #1e293b;
      word-wrap: break-word;
      overflow-wrap: break-word;
      white-space: normal;
      display: block;
      margin-bottom: 6px;
    }
    @media (min-width: 768px) {
      .product-title-full {
        font-size: 13.5px;
      }
    }

    /* Chữ danh mục nhỏ gọn ở trang chủ, viết liền không gãy chữ */
    .cat-pill-compact {
      white-space: nowrap;
      font-size: 11.5px;
      font-weight: 600;
      padding: 4px 10px;
      border-radius: 4px;
      background: #f1f5f9;
      color: #334155;
      border: 1px solid #e2e8f0;
      transition: all 0.15s ease;
    }
    .cat-pill-compact:hover {
      background: #0B3B68;
      color: #ffffff;
      border-color: #0B3B68;
    }

    /* Banner Slider 2 ảnh kích thước bằng nhau tuyệt đối */
    .banner-viewport {
      position: relative;
      width: 100%;
      height: 250px;
      border-radius: 8px;
      overflow: hidden;
    }
    @media (min-width: 640px) {
      .banner-viewport {
        height: 310px;
      }
    }
    @media (min-width: 1024px) {
      .banner-viewport {
        height: 390px;
      }
    }
    .banner-slide {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.6s ease-in-out, visibility 0.6s ease-in-out;
    }
    .banner-slide.active {
      opacity: 1;
      visibility: visible;
      z-index: 5;
    }

    /* Hiệu ứng nút liên hệ nổi góc phải */
    @keyframes pulseRing {
      0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(230, 81, 0, 0.6); }
      70% { transform: scale(1); box-shadow: 0 0 0 10px rgba(230, 81, 0, 0); }
      100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(230, 81, 0, 0); }
    }
    .floating-pulse {
      animation: pulseRing 2s infinite;
    }
  </style>
</head>
<body>

  <!-- =========================================================================
       TOP BAR (ĐỊA CHỈ & THÔNG TIN CÔNG TY - ĐƠN GIẢN CHUẨN FLATSOME)
       ========================================================================= -->
  <div class="bg-[#082B4D] text-white text-xs py-1.5 border-b border-white/10">
    <div class="flatsome-container flex flex-wrap items-center justify-between gap-2">
      <div class="flex items-center gap-2 truncate">
        <i class="fa-solid fa-location-dot text-[#FF8A00]"></i>
        <span class="truncate">65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng</span>
      </div>
      <div class="hidden md:flex items-center gap-5 text-[12px] text-slate-200">
        <a href="#gioi-thieu-cua-hang" class="hover:text-[#FF8A00] transition">Giới thiệu cửa hàng</a>
        <a href="#tin-tuc-trang-chu" class="hover:text-[#FF8A00] transition">Tin tức xây dựng</a>
        <a href="#form-bao-gia" class="hover:text-[#FF8A00] transition">Yêu cầu báo giá</a>
        <a href="#lien-he-ban-do" class="hover:text-[#FF8A00] transition">Bản đồ chỉ đường</a>
      </div>
    </div>
  </div>

  <!-- =========================================================================
       HEADER CHÍNH (LOGO NHỎ GỌN, TÌM KIẾM, KHÔNG ĐỂ NÚT GỌI NGAY ĐỂ TRÁNH TRÀN VIỀN)
       ========================================================================= -->
  <header id="header" class="bg-white sticky top-0 z-50 shadow-sm border-b border-slate-200">
    <div class="flatsome-container py-2.5 flex items-center justify-between gap-3">
      
      <!-- Nút mở Menu trên Điện thoại -->
      <button id="mobileMenuBtn" type="button" aria-label="Mở danh mục" class="lg:hidden p-2 rounded border border-slate-200 text-brand-primary hover:bg-slate-100 shrink-0">
        <i class="fa-solid fa-bars text-lg"></i>
      </button>

      <!-- LOGO CÔNG TY CHUYÊN NGHIỆP - ĐÃ CHỈNH GỌN NHỎ LẠI -->
      <a href="#" class="flex items-center gap-2.5 shrink-0 group">
        <svg class="w-9 h-9 md:w-10 md:h-10 shrink-0" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
          <rect width="100" height="100" rx="16" fill="#0B3B68"/>
          <path d="M18 45L50 18L82 45" stroke="#E65100" stroke-width="8" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M28 80V46L50 74V46" stroke="#FFFFFF" stroke-width="7.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M56 46L67 80L78 46" stroke="#FF9800" stroke-width="7.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
        <div class="leading-tight">
          <div class="text-[13px] sm:text-[15px] font-extrabold text-brand-primary tracking-tight">
            NHẤT VŨ <span class="text-brand-accent font-bold text-[12px] sm:text-[13px]">nhatvu.com</span>
          </div>
          <div class="text-[10px] sm:text-[11px] font-semibold text-slate-500">
            CÔNG TY TNHH MTV XD &amp; TM NHẤT VŨ
          </div>
        </div>
      </a>

      <!-- Thanh tìm kiếm sản phẩm kiểu Flatsome -->
      <div class="hidden sm:flex flex-1 max-w-xl mx-2">
        <form onsubmit="handleSearch(event)" class="w-full flex border-2 border-brand-primary rounded overflow-hidden bg-white">
          <input id="searchInputDesktop" type="text" placeholder="Tìm kiếm sơn Jotun, gạch Đồng Tâm, thiết bị vệ sinh, bồn nước..." class="w-full px-3 py-1.5 text-xs md:text-sm focus:outline-none text-slate-700" />
          <button type="submit" class="bg-brand-primary hover:bg-brand-accent text-white px-4 text-xs md:text-sm font-semibold transition shrink-0">
            <i class="fa-solid fa-magnifying-glass"></i>
          </button>
        </form>
      </div>

      <!-- Liên kết nhanh sang Báo giá (nhỏ gọn, không để nút Gọi ngay tránh tràn viền) -->
      <div class="flex items-center gap-2 shrink-0">
        <a href="#form-bao-gia" class="text-xs font-semibold text-brand-primary bg-slate-100 hover:bg-brand-primary hover:text-white px-2.5 py-1.5 rounded border border-slate-200 transition whitespace-nowrap">
          <i class="fa-regular fa-file-lines mr-1 text-brand-accent"></i>Báo giá
        </a>
      </div>
    </div>

    <!-- Thanh tìm kiếm hiển thị gọn trên màn hình điện thoại -->
    <div class="sm:hidden flatsome-container pb-2">
      <form onsubmit="handleSearch(event)" class="w-full flex border border-brand-primary rounded overflow-hidden bg-white">
        <input id="searchInputMobile" type="text" placeholder="Tìm kiếm sản phẩm vật liệu xây dựng..." class="w-full px-3 py-1.5 text-xs focus:outline-none" />
        <button type="submit" class="bg-brand-primary text-white px-3 text-xs">
          <i class="fa-solid fa-magnifying-glass"></i>
        </button>
      </form>
    </div>

    <!-- =========================================================================
         THANH MENU DANH MỤC MÁY TÍNH (CHỮ NHỎ GỌN, VIẾT LIỀN TRÊN 1 HÀNG HOẶC XUỐNG HÀNG 2, KHÔNG ĐƯỢC GÃY DÒNG TÊN DANH MỤC)
         ========================================================================= -->
    <nav class="hidden lg:block bg-brand-primary text-white border-t border-white/10">
      <div class="flatsome-container py-1">
        <ul class="desktop-cat-nav">
          <li>
            <a href="#" class="desktop-cat-link active"><i class="fa-solid fa-house text-[11px]"></i>TRANG CHỦ</a>
          </li>
          <li class="has-dropdown">
            <a href="#sec-son" class="desktop-cat-link">SƠN <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-son">Sơn Jotun (Ngoại thất, Nội thất, Lót, Bột trét)</a>
              <a href="#sec-son">Sơn Dulux - Maxilite</a>
              <a href="#sec-son">Sơn Tito (Lót chống kiềm, Chống thấm, Sơn nhũ)</a>
              <a href="#sec-son">Chống thấm (Sika, Bestmix, Mapei)</a>
            </div>
          </li>
          <li class="has-dropdown">
            <a href="#sec-tbvs" class="desktop-cat-link">THIẾT BỊ VỆ SINH <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-tbvs">Bồn cầu chính hãng</a>
              <a href="#sec-tbvs">Sen vòi &amp; Sen cây nóng lạnh</a>
              <a href="#sec-tbvs">Chậu rửa Lavabo</a>
              <a href="#sec-tbvs">Gương phòng tắm</a>
              <a href="#sec-tbvs">Phụ kiện nhà tắm</a>
            </div>
          </li>
          <li class="has-dropdown">
            <a href="#sec-gach-men" class="desktop-cat-link">GẠCH MEN <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-gach-men">Gạch Đồng Tâm (80x80, 60x60, 40x80, 30x60)</a>
              <a href="#sec-gach-men">Gạch Kimgres cao cấp</a>
            </div>
          </li>
          <li class="has-dropdown">
            <a href="#sec-ngoi-lop" class="desktop-cat-link">NGÓI LỢP <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-ngoi-lop">Ngói màu DIC</a>
              <a href="#sec-ngoi-lop">Ngói Đất Việt</a>
            </div>
          </li>
          <li class="has-dropdown">
            <a href="#sec-bon-nuoc" class="desktop-cat-link">BỒN NƯỚC <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-bon-nuoc">Bồn nước Letton</a>
              <a href="#sec-bon-nuoc">Bồn nước Sơn Hà</a>
              <a href="#sec-bon-nuoc">Bồn nước Tân Á</a>
            </div>
          </li>
          <li class="has-dropdown">
            <a href="#sec-binh-nong-lanh" class="desktop-cat-link">BÌNH NÓNG LẠNH <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-binh-nong-lanh">Bình nóng lạnh Ariston</a>
              <a href="#sec-binh-nong-lanh">Bình nóng lạnh Ferroli</a>
            </div>
          </li>
          <li class="has-dropdown">
            <a href="#sec-keo-dan-gach" class="desktop-cat-link">DÁN GẠCH, CHÀ RON <i class="fa-solid fa-angle-down text-[10px] opacity-80"></i></a>
            <div class="nav-dropdown">
              <a href="#sec-keo-dan-gach">Phụ gia Bestmix</a>
              <a href="#sec-keo-dan-gach">Keo dán gạch Đồng Tâm</a>
              <a href="#sec-keo-dan-gach">Keo Cá Sấu (Crocodile)</a>
              <a href="#sec-keo-dan-gach">Keo dán gạch Sika</a>
            </div>
          </li>
          <li>
            <a href="#doi-tac-thuong-hieu" class="desktop-cat-link">ĐỐI TÁC</a>
          </li>
          <li>
            <a href="#tin-tuc-trang-chu" class="desktop-cat-link">BÀI VIẾT</a>
          </li>
          <li>
            <a href="#lien-he-ban-do" class="desktop-cat-link">LIÊN HỆ</a>
          </li>
        </ul>
      </div>
    </nav>
  </header>

  <!-- =========================================================================
       MENU DANH MỤC TRÊN ĐIỆN THOẠI (DRAWER GỌN ĐẸP CHUẨN FLATSOME)
       ========================================================================= -->
  <div id="mobileMenuOverlay" class="fixed inset-0 bg-black/50 z-50 hidden">
    <div class="bg-white w-72 max-w-[85vw] h-full overflow-y-auto shadow-xl flex flex-col">
      <div class="p-3.5 bg-brand-primary text-white flex items-center justify-between">
        <span class="font-bold text-sm">DANH MỤC SẢN PHẨM</span>
        <button id="closeMobileMenuBtn" type="button" class="w-7 h-7 rounded bg-white/10 flex items-center justify-center">
          <i class="fa-solid fa-xmark"></i>
        </button>
      </div>
      <div class="divide-y divide-slate-100 text-xs font-semibold text-slate-700">
        <a href="#" onclick="closeMobileMenu()" class="block px-4 py-3 text-brand-primary bg-slate-50">TRANG CHỦ</a>
        <a href="#sec-son" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">SƠN (Jotun, Dulux-Maxilite, Tito, Chống thấm)</a>
        <a href="#sec-tbvs" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">THIẾT BỊ VỆ SINH (Bồn cầu, Sen vòi, Lavabo, Gương)</a>
        <a href="#sec-gach-men" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">GẠCH MEN (Đồng Tâm, Kimgres)</a>
        <a href="#sec-ngoi-lop" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">NGÓI LỢP (DIC, Ngói Đất Việt)</a>
        <a href="#sec-bon-nuoc" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">BỒN NƯỚC (Letton, Sơn Hà, Tân Á)</a>
        <a href="#sec-binh-nong-lanh" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">BÌNH NÓNG LẠNH (Ariston, Ferroli)</a>
        <a href="#sec-keo-dan-gach" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">DÁN GẠCH, CHÀ RON (Bestmix, Đồng Tâm, Cá Sấu, Sika)</a>
        <a href="#doi-tac-thuong-hieu" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">ĐỐI TÁC PHÂN PHỐI</a>
        <a href="#tin-tuc-trang-chu" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">DANH MỤC BÀI VIẾT</a>
        <a href="#form-bao-gia" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">YÊU CẦU &amp; BÁO GIÁ</a>
        <a href="#lien-he-ban-do" onclick="closeMobileMenu()" class="block px-4 py-3 hover:text-brand-accent">LIÊN HỆ &amp; BẢN ĐỒ</a>
      </div>
    </div>
  </div>

  <!-- =========================================================================
       MAIN CONTENT (CHUẨN CẤU TRÚC SECTION > ROW > COL CỦA FLATSOME)
       ========================================================================= -->
  <main id="main" class="py-4 space-y-6">

    <!-- 1. SECTION: 2 ẢNH BANNER TỰ TRƯỢT CHUYÊN NGHIỆP KÍCH THƯỚC BẰNG NHAU
         Chữ & hình ảnh nằm gọn bên trong banner, cách xa viền ảnh, không bị thiếu chữ trên cả ĐT & Máy tính -->
    <section class="flatsome-container">
      <div class="banner-viewport shadow-sm">
        
        <!-- BANNER SLIDE 1 -->
        <div class="banner-slide active bg-gradient-to-r from-[#072644] via-[#0B3B68] to-[#14558F]">
          <div class="w-full h-full px-8 py-6 sm:px-14 sm:py-9 lg:px-20 lg:py-12 flex items-center justify-between gap-6">
            <div class="w-full md:w-7/12 text-white space-y-2 sm:space-y-3">
              <div class="text-[#FFB300] text-[11px] sm:text-xs md:text-sm font-bold uppercase tracking-wider">
                CÔNG TY TNHH MTV XD &amp; TM NHẤT VŨ - NHATVU.COM
              </div>
              <h1 class="text-base sm:text-2xl lg:text-3xl font-extrabold leading-snug">
                TỔNG KHO SƠN NƯỚC, GẠCH MEN &amp; THIẾT BỊ VỆ SINH CHÍNH HÃNG ĐÀ NẴNG
              </h1>
              <p class="text-[11px] sm:text-xs lg:text-sm text-slate-200 leading-relaxed">
                Phân phối Sơn Jotun, Dulux, Gạch Đồng Tâm, Kimgres, Thiết bị vệ sinh Inax, Viglacera, Bồn nước, Bình nóng lạnh &amp; Phụ gia chống thấm Sika.
              </p>
              <div class="pt-1 flex flex-wrap items-center gap-2 text-[11px] sm:text-xs font-semibold text-amber-300">
                <span><i class="fa-solid fa-location-dot mr-1"></i>65 Nguyễn Quang Diêu, Hòa Xuân, Đà Nẵng</span>
                <span class="hidden sm:inline">|</span>
                <span><i class="fa-solid fa-phone mr-1"></i>0905.343.016 - 0905.327.257</span>
              </div>
            </div>
            <!-- Hình minh họa thực tế nằm gọn bên trong banner -->
            <div class="hidden md:flex md:w-5/12 h-full items-center justify-center p-2">
              <div class="grid grid-cols-2 gap-2.5 w-full max-w-xs bg-white/10 p-3 rounded-lg border border-white/20">
                <img src="https://drive.google.com/thumbnail?id=1mDw0niLRcvL5Uo47G7Zkxguabu9fWm3d&sz=w600" onerror="handleDriveImgError(this, '1mDw0niLRcvL5Uo47G7Zkxguabu9fWm3d', 'Cua+Hang+Nhat+Vu')" alt="Cửa hàng Nhất Vũ" class="w-full h-28 object-cover rounded bg-white" />
                <img src="https://drive.google.com/thumbnail?id=1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY&sz=w600" onerror="handleDriveImgError(this, '1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY', 'San+Pham+Nhat+Vu')" alt="Sản phẩm Nhất Vũ" class="w-full h-28 object-cover rounded bg-white" />
              </div>
            </div>
          </div>
        </div>

        <!-- BANNER SLIDE 2 (Kích thước bằng nhau 100% với Slide 1) -->
        <div class="banner-slide bg-gradient-to-r from-[#0F385C] via-[#124B7A] to-[#8C3200]">
          <div class="w-full h-full px-8 py-6 sm:px-14 sm:py-9 lg:px-20 lg:py-12 flex items-center justify-between gap-6">
            <div class="w-full md:w-7/12 text-white space-y-2 sm:space-y-3">
              <div class="text-[#FFD54F] text-[11px] sm:text-xs md:text-sm font-bold uppercase tracking-wider">
                GIẢI PHÁP VẬT LIỆU XÂY DỰNG TOÀN DIỆN CHO MỌI CÔNG TRÌNH
              </div>
              <h2 class="text-base sm:text-2xl lg:text-3xl font-extrabold leading-snug">
                CHỐNG THẤM SIKA, KEO DÁN GẠCH, NGÓI LỢP &amp; BỒN NƯỚC GIÁ TỐT NHẤT
              </h2>
              <p class="text-[11px] sm:text-xs lg:text-sm text-slate-100 leading-relaxed">
                Cam kết hàng chính hãng 100%, chiết khấu cao cho nhà thầu và công trình dân dụng. Giao hàng tận chân công trình nhanh chóng tại Đà Nẵng &amp; Miền Trung.
              </p>
              <div class="pt-1 flex flex-wrap items-center gap-2 text-[11px] sm:text-xs font-semibold text-amber-200">
                <span><i class="fa-solid fa-truck-fast mr-1"></i>Giao hàng tận nơi</span>
                <span>•</span>
                <span><i class="fa-solid fa-Phone-volume mr-1"></i>Tư vấn báo giá: 0905.343.016 - 0905.327.257</span>
              </div>
            </div>
            <!-- Hình minh họa thực tế nằm gọn bên trong banner -->
            <div class="hidden md:flex md:w-5/12 h-full items-center justify-center p-2">
              <div class="grid grid-cols-2 gap-2.5 w-full max-w-xs bg-white/10 p-3 rounded-lg border border-white/20">
                <img src="https://drive.google.com/thumbnail?id=19JJuOMRdlzRtuwo-hfD7TsgqGqY3D849&sz=w600" onerror="handleDriveImgError(this, '19JJuOMRdlzRtuwo-hfD7TsgqGqY3D849', 'Showroom+Nhat+Vu')" alt="Kho hàng Nhất Vũ" class="w-full h-28 object-cover rounded bg-white" />
                <img src="https://drive.google.com/thumbnail?id=11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP&sz=w600" onerror="handleDriveImgError(this, '11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP', 'VLXD+Nhat+Vu')" alt="Vật liệu xây dựng Nhất Vũ" class="w-full h-28 object-cover rounded bg-white" />
              </div>
            </div>
          </div>
        </div>

        <!-- Nút điều hướng Trái / Phải của Banner -->
        <button type="button" onclick="changeBanner(-1)" aria-label="Banner trước" class="absolute left-2 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-8 sm:h-8 rounded-full bg-black/35 hover:bg-black/60 text-white flex items-center justify-center text-xs">
          <i class="fa-solid fa-chevron-left"></i>
        </button>
        <button type="button" onclick="changeBanner(1)" aria-label="Banner kế tiếp" class="absolute right-2 top-1/2 -translate-y-1/2 z-20 w-7 h-7 sm:w-8 sm:h-8 rounded-full bg-black/35 hover:bg-black/60 text-white flex items-center justify-center text-xs">
          <i class="fa-solid fa-chevron-right"></i>
        </button>

        <!-- Chấm tròn chuyển slide -->
        <div class="absolute bottom-2.5 left-1/2 -translate-x-1/2 z-20 flex items-center gap-2">
          <button type="button" onclick="goToBanner(0)" class="banner-dot w-2.5 h-2.5 rounded-full bg-white transition"></button>
          <button type="button" onclick="goToBanner(1)" class="banner-dot w-2.5 h-2.5 rounded-full bg-white/40 transition"></button>
        </div>
      </div>
    </section>

    <!-- 2. SECTION: DANH MỤC SẢN PHẨM TRANG CHỦ (CHỮ NHỎ GỌN, ĐẸP TRÊN CẢ MÁY TÍNH & ĐIỆN THOẠI) -->
    <section class="flatsome-container">
      <div class="bg-white rounded-lg border border-slate-200 p-3.5 shadow-sm">
        <div class="flex items-center justify-between border-b border-slate-200 pb-2.5 mb-3">
          <h2 class="text-sm sm:text-base font-extrabold text-brand-primary uppercase tracking-tight">
            DANH MỤC SẢN PHẨM
          </h2>
          <span class="text-[11px] text-slate-500">Chọn nhanh danh mục</span>
        </div>

        <!-- Lưới danh mục thiết kế gọn gàng, chữ danh mục không bị gãy dòng -->
        <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-7 gap-2.5">
          <a href="#sec-son" class="flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-fill-drip text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">SƠN NƯỚC</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">Jotun • Dulux • Tito</span>
          </a>

          <a href="#sec-tbvs" class="flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-shower text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">THIẾT BỊ VỆ SINH</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">Bồn cầu • Sen vòi</span>
          </a>

          <a href="#sec-gach-men" class="flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-border-all text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">GẠCH MEN</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">Đồng Tâm • Kimgres</span>
          </a>

          <a href="#sec-ngoi-lop" class="flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-house-chimney text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">NGÓI LỢP</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">DIC • Ngói Đất Việt</span>
          </a>

          <a href="#sec-bon-nuoc" class="flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-database text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">BỒN NƯỚC</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">Letton • Sơn Hà • Tân Á</span>
          </a>

          <a href="#sec-binh-nong-lanh" class="flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-temperature-arrow-up text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">BÌNH NÓNG LẠNH</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">Ariston • Ferroli</span>
          </a>

          <a href="#sec-keo-dan-gach" class="col-span-2 sm:col-span-1 flex flex-col items-center justify-center p-2.5 rounded border border-slate-200 hover:border-brand-accent hover:bg-orange-50/40 transition text-center">
            <div class="w-9 h-9 rounded-full bg-blue-50 text-brand-primary flex items-center justify-center mb-1.5">
              <i class="fa-solid fa-trowel-bricks text-sm"></i>
            </div>
            <span class="text-xs font-bold text-slate-800 whitespace-nowrap">DÁN GẠCH, CHÀ RON</span>
            <span class="text-[10px] text-slate-500 whitespace-nowrap">Sika • Cá Sấu • Bestmix</span>
          </a>
        </div>
      </div>
    </section>

    <!-- =========================================================================
         CÁC SECTION SẢN PHẨM THEO DANH MỤC MẪU NOITHATNGONGUYEN.COM + 19 ẢNH THỰC TẾ GOOGLE DRIVE
         (2 cột trên điện thoại, 5 cột trên máy tính, % giảm giá góc trên bên trái, không nhãn dán thừa)
         ========================================================================= -->
    <div id="catalogContainer" class="space-y-6"></div>

    <!-- =========================================================================
         3. SECTION: BỘ SƯU TẬP 19 ẢNH SẢN PHẨM THỰC TẾ TẠI KHO & CỬA HÀNG NHẤT VŨ
         (Giúp đối chiếu toàn bộ 19 file ảnh thực tế từ Google Drive để đưa vào UX Builder dễ dàng)
         ========================================================================= -->
    <section id="anh-thuc-te-kho" class="flatsome-container">
      <div class="bg-white rounded-lg border border-slate-200 p-4 shadow-sm">
        <div class="flex flex-wrap items-center justify-between gap-2 border-b-2 border-brand-primary pb-2.5 mb-4">
          <h2 class="text-sm sm:text-base font-extrabold text-brand-primary uppercase">
            HÌNH ẢNH SẢN PHẨM THỰC TẾ TẠI CỬA HÀNG NHẤT VŨ
          </h2>
          <span class="text-xs text-slate-500">19 mẫu sản phẩm thực tế tại 65 Nguyễn Quang Diêu</span>
        </div>
        <div id="allRealPhotosGrid" class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-3"></div>
      </div>
    </section>

    <!-- =========================================================================
         4. SECTION: HÌNH ẢNH CỬA HÀNG THỰC TẾ + KẾT NỐI FACEBOOK + GOOGLE MAP NGOÀI TRANG CHỦ
         ========================================================================= -->
    <section id="gioi-thieu-cua-hang" class="flatsome-container">
      <div class="bg-white rounded-lg border border-slate-200 p-4 shadow-sm">
        <div class="border-b-2 border-brand-primary pb-2.5 mb-4 flex flex-wrap items-center justify-between gap-2">
          <h2 class="text-sm sm:text-base font-extrabold text-brand-primary uppercase">
            HÌNH ẢNH CỬA HÀNG, FACEBOOK &amp; BẢN ĐỒ CHỈ ĐƯỜNG
          </h2>
          <span class="text-xs font-semibold text-brand-accent">65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng</span>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-4 items-stretch">
          <!-- Cột 1: 2 Ảnh Cửa Hàng Thực Tế từ Google Drive (5/12) -->
          <div class="lg:col-span-5 flex flex-col justify-between bg-slate-50 p-3 rounded border border-slate-200">
            <div>
              <h3 class="text-xs sm:text-sm font-bold text-brand-primary mb-2">
                <i class="fa-solid fa-store text-brand-accent mr-1.5"></i>Hình Ảnh Thực Tế Cửa Hàng Nhất Vũ
              </h3>
              <div class="grid grid-cols-2 gap-2.5">
                <div class="rounded overflow-hidden border border-slate-200 bg-white">
                  <img src="https://drive.google.com/thumbnail?id=1mDw0niLRcvL5Uo47G7Zkxguabu9fWm3d&sz=w800" onerror="handleDriveImgError(this, '1mDw0niLRcvL5Uo47G7Zkxguabu9fWm3d', 'Cua+Hang+Nhat+Vu+1')" alt="Ảnh cửa hàng Nhất Vũ 1" class="w-full h-40 sm:h-48 object-cover" />
                  <div class="p-2 text-[11px] font-semibold text-center text-slate-700">Mặt tiền &amp; Kho bãi Nhất Vũ</div>
                </div>
                <div class="rounded overflow-hidden border border-slate-200 bg-white">
                  <img src="https://drive.google.com/thumbnail?id=19JJuOMRdlzRtuwo-hfD7TsgqGqY3D849&sz=w800" onerror="handleDriveImgError(this, '19JJuOMRdlzRtuwo-hfD7TsgqGqY3D849', 'Cua+Hang+Nhat+Vu+2')" alt="Ảnh cửa hàng Nhất Vũ 2" class="w-full h-40 sm:h-48 object-cover" />
                  <div class="p-2 text-[11px] font-semibold text-center text-slate-700">Khu trưng bày sản phẩm thực tế</div>
                </div>
              </div>
            </div>
            <div class="mt-3 pt-2.5 border-t border-slate-200 text-xs text-slate-600 space-y-1">
              <p><strong>Đơn vị:</strong> CÔNG TY TNHH MỘT THÀNH VIÊN XD &amp; TM NHẤT VŨ</p>
              <p><strong>Địa chỉ:</strong> 65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng</p>
              <p><strong>Điện thoại:</strong> <a href="tel:0905343016" class="text-brand-accent font-bold">0905.343.016</a> - <a href="tel:0905327257" class="text-brand-accent font-bold">0905.327.257</a></p>
            </div>
          </div>

          <!-- Cột 2: Kết nối Facebook ngoài trang chủ (3/12) -->
          <div class="lg:col-span-3 flex flex-col justify-between bg-slate-50 p-3 rounded border border-slate-200">
            <div>
              <h3 class="text-xs sm:text-sm font-bold text-brand-primary mb-2">
                <i class="fa-brands fa-facebook text-[#1877F2] mr-1.5"></i>Kết Nối Facebook Chính Thức
              </h3>
              <div class="bg-white rounded border border-slate-200 overflow-hidden">
                <div class="h-20 bg-gradient-to-r from-[#0B3B68] to-[#1877F2] p-3 flex items-end">
                  <div class="flex items-center gap-2.5">
                    <div class="w-11 h-11 rounded-full bg-white p-1 shadow flex items-center justify-center text-brand-primary font-extrabold text-sm">
                      NV
                    </div>
                    <div class="text-white">
                      <div class="text-xs font-bold leading-tight">XD &amp; TM Nhất Vũ</div>
                      <div class="text-[10px] text-blue-100">nhatvu.com • Đà Nẵng</div>
                    </div>
                  </div>
                </div>
                <div class="p-3 space-y-2 text-xs text-slate-600">
                  <p class="leading-relaxed">
                    Cập nhật hình ảnh giao hàng thực tế, bảng giá sơn Jotun, Dulux, gạch men, thiết bị vệ sinh mới nhất trên Facebook của Nhất Vũ.
                  </p>
                  <a href="https://www.facebook.com/profile.php?id=100018933160246" target="_blank" rel="noopener noreferrer" class="w-full inline-flex items-center justify-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white font-semibold py-2 px-3 rounded text-xs transition">
                    <i class="fa-brands fa-facebook-f"></i> Xem Trang Facebook Nhất Vũ
                  </a>
                </div>
              </div>
            </div>
            <div class="mt-3 pt-2 border-t border-slate-200 text-[11px] text-slate-500">
              ID Facebook: <span class="font-mono text-slate-700">100018933160246</span>
            </div>
          </div>

          <!-- Cột 3: Bản đồ Google Maps ngoài trang chủ (4/12) -->
          <div id="lien-he-ban-do" class="lg:col-span-4 flex flex-col justify-between bg-slate-50 p-3 rounded border border-slate-200">
            <div>
              <div class="flex items-center justify-between mb-2">
                <h3 class="text-xs sm:text-sm font-bold text-brand-primary">
                  <i class="fa-solid fa-map-location-dot text-brand-accent mr-1.5"></i>Bản Đồ Google Map
                </h3>
                <a href="https://share.google/1XOj3LATI4UPCFgoy" target="_blank" rel="noopener noreferrer" class="text-[11px] font-bold text-brand-accent hover:underline">
                  Mở Google Map <i class="fa-solid fa-arrow-up-right-from-square text-[10px]"></i>
                </a>
              </div>
              <div class="rounded overflow-hidden border border-slate-300 bg-white h-52">
                <iframe
                  title="Bản đồ 65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng"
                  src="https://www.google.com/maps?q=65+Nguy%E1%BB%85n+Quang+Di%C3%AAu,+H%C3%B2a+Xu%C3%A2n,+%C4%90%C3%A0+N%E1%BA%B5ng&output=embed"
                  class="w-full h-full border-0"
                  loading="lazy"
                  referrerpolicy="no-referrer-when-downgrade">
                </iframe>
              </div>
            </div>
            <div class="mt-2.5 flex items-center justify-between gap-2">
              <span class="text-[11px] text-slate-600 truncate">65 Nguyễn Quang Diêu, P. Hòa Xuân, Đà Nẵng</span>
              <a href="https://share.google/1XOj3LATI4UPCFgoy" target="_blank" rel="noopener noreferrer" class="shrink-0 bg-brand-primary hover:bg-brand-accent text-white text-[11px] font-semibold px-2.5 py-1.5 rounded transition">
                <i class="fa-solid fa-diamond-turn-right mr-1"></i>Chỉ đường
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- =========================================================================
         5. SECTION: FORM YÊU CẦU VÀ BÁO GIÁ TRANG CHỦ
         ========================================================================= -->
    <section id="form-bao-gia" class="flatsome-container">
      <div class="bg-white rounded-lg border border-slate-200 p-4 sm:p-6 shadow-sm">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-center">
          <div class="lg:col-span-5 space-y-2.5">
            <h2 class="text-base sm:text-lg font-extrabold text-brand-primary uppercase">
              ĐĂNG KÝ YÊU CẦU TƯ VẤN &amp; NHẬN BÁO GIÁ SỈ / LẺ
            </h2>
            <p class="text-xs sm:text-sm text-slate-600 leading-relaxed">
              Quý khách hàng, nhà thầu xây dựng cần báo giá nhanh các hạng mục <strong>Sơn nước, Gạch ốp lát, Thiết bị vệ sinh, Ngói lợp, Bồn nước, Bình nóng lạnh, Chống thấm &amp; Keo dán gạch</strong> vui lòng điền thông tin bên cạnh.
            </p>
            <div class="p-3 rounded bg-slate-50 border border-slate-200 space-y-1.5 text-xs text-slate-700">
              <div><i class="fa-solid fa-check text-brand-accent mr-2"></i>Báo giá chiết khấu cao trực tiếp từ nhà phân phối Nhất Vũ</div>
              <div><i class="fa-solid fa-check text-brand-accent mr-2"></i>Hỗ trợ phối màu sơn 3D &amp; tính toán khối lượng vật tư miễn phí</div>
              <div><i class="fa-solid fa-check text-brand-accent mr-2"></i>Giao hàng nhanh tận công trình tại Đà Nẵng &amp; khu vực lân cận</div>
            </div>
          </div>

          <div class="lg:col-span-7">
            <form id="quoteForm" onsubmit="submitQuoteForm(event)" class="bg-slate-50 p-4 rounded-lg border border-slate-200 space-y-3">
              <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                <div>
                  <label class="block text-xs font-bold text-slate-700 mb-1">Họ và tên khách hàng *</label>
                  <input id="qName" type="text" required placeholder="Nhập họ và tên..." class="w-full px-3 py-2 text-xs sm:text-sm rounded border border-slate-300 bg-white focus:outline-none focus:border-brand-primary" />
                </div>
                <div>
                  <label class="block text-xs font-bold text-slate-700 mb-1">Số điện thoại / Zalo *</label>
                  <input id="qPhone" type="tel" required placeholder="Ví dụ: 0905343016" class="w-full px-3 py-2 text-xs sm:text-sm rounded border border-slate-300 bg-white focus:outline-none focus:border-brand-primary" />
                </div>
              </div>

              <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                <div>
                  <label class="block text-xs font-bold text-slate-700 mb-1">Danh mục sản phẩm cần báo giá</label>
                  <select id="qCategory" class="w-full px-3 py-2 text-xs sm:text-sm rounded border border-slate-300 bg-white focus:outline-none focus:border-brand-primary">
                    <option value="Sơn nước (Jotun, Dulux, Tito, Chống thấm)">Sơn nước (Jotun, Dulux, Tito, Chống thấm)</option>
                    <option value="Thiết bị vệ sinh (Bồn cầu, Sen vòi, Lavabo)">Thiết bị vệ sinh (Bồn cầu, Sen vòi, Lavabo)</option>
                    <option value="Gạch men ốp lát (Đồng Tâm, Kimgres)">Gạch men ốp lát (Đồng Tâm, Kimgres)</option>
                    <option value="Ngói lợp (DIC, Ngói Đất Việt)">Ngói lợp (DIC, Ngói Đất Việt)</option>
                    <option value="Bồn nước (Letton, Sơn Hà, Tân Á)">Bồn nước (Letton, Sơn Hà, Tân Á)</option>
                    <option value="Bình nóng lạnh (Ariston, Ferroli)">Bình nóng lạnh (Ariston, Ferroli)</option>
                    <option value="Keo dán gạch, Chà ron (Sika, Cá Sấu, Đồng Tâm)">Keo dán gạch, Chà ron (Sika, Cá Sấu, Đồng Tâm)</option>
                    <option value="Trọn gói Vật liệu xây dựng hoàn thiện">Trọn gói Vật liệu xây dựng hoàn thiện</option>
                  </select>
                </div>
                <div>
                  <label class="block text-xs font-bold text-slate-700 mb-1">Địa chỉ giao hàng / Công trình</label>
                  <input id="qAddress" type="text" placeholder="Ví dụ: Hòa Xuân, Cẩm Lệ, Đà Nẵng" class="w-full px-3 py-2 text-xs sm:text-sm rounded border border-slate-300 bg-white focus:outline-none focus:border-brand-primary" />
                </div>
              </div>

              <div>
                <label class="block text-xs font-bold text-slate-700 mb-1">Nội dung yêu cầu &amp; Khối lượng dự kiến</label>
                <textarea id="qNote" rows="2" placeholder="Nhập mã sản phẩm, số lượng hoặc yêu cầu tư vấn chi tiết..." class="w-full px-3 py-2 text-xs sm:text-sm rounded border border-slate-300 bg-white focus:outline-none focus:border-brand-primary"></textarea>
              </div>

              <div class="flex flex-wrap items-center justify-between gap-3 pt-1">
                <button type="submit" class="bg-brand-accent hover:bg-orange-700 text-white font-bold text-xs sm:text-sm px-5 py-2.5 rounded transition shadow-sm">
                  <i class="fa-solid fa-paper-plane mr-1.5"></i>GỬI YÊU CẦU BÁO GIÁ
                </button>
                <span class="text-xs text-slate-500">Hoặc liên hệ trực tiếp: <strong>0905.343.016 - 0905.327.257</strong></span>
              </div>

              <div id="quoteSuccessMsg" class="hidden p-3 rounded bg-emerald-50 border border-emerald-200 text-emerald-800 text-xs font-semibold"></div>
            </form>
          </div>
        </div>
      </div>
    </section>

    <!-- =========================================================================
         6. SECTION: DANH MỤC CÁC BÀI VIẾT TRANG CHỦ (TIN TỨC & KINH NGHIỆM XÂY DỰNG)
         ========================================================================= -->
    <section id="tin-tuc-trang-chu" class="flatsome-container">
      <div class="bg-white rounded-lg border border-slate-200 p-4 shadow-sm">
        <div class="flex items-center justify-between border-b-2 border-brand-primary pb-2.5 mb-4">
          <h2 class="text-sm sm:text-base font-extrabold text-brand-primary uppercase">
            DANH MỤC BÀI VIẾT &amp; KINH NGHIỆM XÂY DỰNG
          </h2>
          <span class="text-xs text-brand-primary font-semibold">Tin tức nhatvu.com</span>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-3.5">
          <article class="border border-slate-200 rounded overflow-hidden flex flex-col bg-white hover:shadow-md transition">
            <img src="https://drive.google.com/thumbnail?id=171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O&sz=w600" onerror="handleDriveImgError(this, '171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O', 'Kinh+Nghiem+Chon+Son')" alt="Kinh nghiệm chọn sơn" class="w-full h-36 object-cover bg-slate-100" />
            <div class="p-3 flex-1 flex flex-col justify-between">
              <div>
                <h3 class="text-xs sm:text-sm font-bold text-slate-800 leading-snug mb-1.5">
                  Kinh Nghiệm Chọn Sơn Ngoại Thất Jotun &amp; Dulux Bền Màu Cho Khí Hậu Đà Nẵng
                </h3>
                <p class="text-[11.5px] text-slate-500 leading-relaxed">
                  Hướng dẫn quy trình thi công sơn lót chống kiềm và sơn phủ ngoại thất chống bám bẩn, chống thấm tối ưu cho nhà phố.
                </p>
              </div>
              <div class="mt-2 pt-2 border-t border-slate-100 text-[11px] text-brand-primary font-semibold">
                Tư vấn Sơn Nước • Nhất Vũ
              </div>
            </div>
          </article>

          <article class="border border-slate-200 rounded overflow-hidden flex flex-col bg-white hover:shadow-md transition">
            <img src="https://drive.google.com/thumbnail?id=1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN&sz=w600" onerror="handleDriveImgError(this, '1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN', 'Chon+Gach+Op+Lat')" alt="Cách chọn gạch Porcelain" class="w-full h-36 object-cover bg-slate-100" />
            <div class="p-3 flex-1 flex flex-col justify-between">
              <div>
                <h3 class="text-xs sm:text-sm font-bold text-slate-800 leading-snug mb-1.5">
                  Cách Phân Biệt Gạch Porcelain Kháng Khuẩn Đồng Tâm 80x80 &amp; Gạch Men Thường
                </h3>
                <p class="text-[11.5px] text-slate-500 leading-relaxed">
                  Tìm hiểu ưu điểm chịu lực, chống trầy xước và độ bền màu vượt trội của dòng gạch Porcelain 2 da Đồng Tâm và Kimgres.
                </p>
              </div>
              <div class="mt-2 pt-2 border-t border-slate-100 text-[11px] text-brand-primary font-semibold">
                Tư vấn Gạch Ốp Lát • Nhất Vũ
              </div>
            </div>
          </article>

          <article class="border border-slate-200 rounded overflow-hidden flex flex-col bg-white hover:shadow-md transition">
            <img src="https://drive.google.com/thumbnail?id=1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4&sz=w600" onerror="handleDriveImgError(this, '1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4', 'Thiet+Bi+Ve+Sinh')" alt="Chọn thiết bị vệ sinh" class="w-full h-36 object-cover bg-slate-100" />
            <div class="p-3 flex-1 flex flex-col justify-between">
              <div>
                <h3 class="text-xs sm:text-sm font-bold text-slate-800 leading-snug mb-1.5">
                  Trọn Bộ Thiết Bị Vệ Sinh Phòng Tắm Gồm Những Gì? Báo Giá Mới Nhất
                </h3>
                <p class="text-[11.5px] text-slate-500 leading-relaxed">
                  Tổng hợp combo Bồn cầu, Sen cây tắm nóng lạnh, Chậu rửa Lavabo, Gương &amp; Phụ kiện Inax, Viglacera tiết kiệm chi phí.
                </p>
              </div>
              <div class="mt-2 pt-2 border-t border-slate-100 text-[11px] text-brand-primary font-semibold">
                Thiết Bị Vệ Sinh • Nhất Vũ
              </div>
            </div>
          </article>

          <article class="border border-slate-200 rounded overflow-hidden flex flex-col bg-white hover:shadow-md transition">
            <img src="https://drive.google.com/thumbnail?id=15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_&sz=w600" onerror="handleDriveImgError(this, '15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_', 'Chong+Tham+Sika')" alt="Thi công keo dán gạch và chống thấm" class="w-full h-36 object-cover bg-slate-100" />
            <div class="p-3 flex-1 flex flex-col justify-between">
              <div>
                <h3 class="text-xs sm:text-sm font-bold text-slate-800 leading-snug mb-1.5">
                  Tại Sao Nên Dùng Keo Dán Gạch Sika, Cá Sấu Thay Cho Hồ Dầu Truyền Thống?
                </h3>
                <p class="text-[11.5px] text-slate-500 leading-relaxed">
                  Giải pháp chống bong tróc, bộp gạch khổ lớn 80x80cm bằng keo dán gạch chuyên dụng và keo chà ron chống thấm.
                </p>
              </div>
              <div class="mt-2 pt-2 border-t border-slate-100 text-[11px] text-brand-primary font-semibold">
                Phụ Gia Xây Dựng • Nhất Vũ
              </div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- =========================================================================
         7. SECTION: DANH MỤC CÁC ĐỐI TÁC & THƯƠNG HIỆU ĐỒNG HÀNH
         ========================================================================= -->
    <section id="doi-tac-thuong-hieu" class="flatsome-container">
      <div class="bg-white rounded-lg border border-slate-200 p-4 shadow-sm">
        <div class="flex items-center justify-between border-b border-slate-200 pb-2.5 mb-3">
          <h2 class="text-sm sm:text-base font-extrabold text-brand-primary uppercase">
            ĐỐI TÁC &amp; THƯƠNG HIỆU PHÂN PHỐI CHÍNH HÃNG
          </h2>
          <span class="text-xs text-slate-500">Cam kết chính hãng 100%</span>
        </div>

        <div class="grid grid-cols-3 sm:grid-cols-4 md:grid-cols-6 gap-2.5">
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#003366]">JOTUN</span>
            <span class="text-[10px] text-slate-500">Sơn Na Uy</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#1E40AF]">DULUX</span>
            <span class="text-[10px] text-slate-500">AkzoNobel</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#0284C7]">INAX</span>
            <span class="text-[10px] text-slate-500">Thiết bị vệ sinh</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#0F766E]">VIGLACERA</span>
            <span class="text-[10px] text-slate-500">Sứ vệ sinh &amp; Sen vòi</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#B91C1C]">ĐỒNG TÂM</span>
            <span class="text-[10px] text-slate-500">Gạch Porcelain</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#334155]">KIMGRES</span>
            <span class="text-[10px] text-slate-500">Gạch men cao cấp</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#D97706]">SIKA</span>
            <span class="text-[10px] text-slate-500">Chống thấm &amp; Keo</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#15803D]">BESTMIX</span>
            <span class="text-[10px] text-slate-500">Hóa chất xây dựng</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#DC2626]">ARISTON</span>
            <span class="text-[10px] text-slate-500">Bình nóng lạnh</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#EA580C]">FERROLI</span>
            <span class="text-[10px] text-slate-500">Máy nước nóng</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#1D4ED8]">SƠN HÀ</span>
            <span class="text-[10px] text-slate-500">Bồn nước Inox/Nhựa</span>
          </div>
          <div class="p-3 rounded border border-slate-200 bg-slate-50 flex flex-col items-center justify-center text-center">
            <span class="font-extrabold text-sm text-[#C2410C]">TÂN Á</span>
            <span class="text-[10px] text-slate-500">Bồn nước Đại Thành</span>
          </div>
        </div>
      </div>
    </section>

  </main>

  <!-- =========================================================================
       FOOTER CHUẨN FLATSOME
       ========================================================================= -->
  <footer class="bg-[#082B4D] text-slate-200 pt-8 pb-6 mt-6 border-t-4 border-brand-accent">
    <div class="flatsome-container grid grid-cols-1 md:grid-cols-3 gap-6 pb-6 border-b border-white/10 text-xs">
      
      <!-- Thông tin công ty -->
      <div class="space-y-2.5">
        <div class="flex items-center gap-2.5">
          <svg class="w-8 h-8 shrink-0" viewBox="0 0 100 100" fill="none">
            <rect width="100" height="100" rx="16" fill="#FFFFFF"/>
            <path d="M18 45L50 18L82 45" stroke="#E65100" stroke-width="8" stroke-linecap="round" stroke-linejoin="round"/>
            <path d="M28 80V46L50 74V46" stroke="#0B3B68" stroke-width="7.5" stroke-linecap="round" stroke-linejoin="round"/>
            <path d="M56 46L67 80L78 46" stroke="#E65100" stroke-width="7.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
          <div>
            <div class="font-extrabold text-white text-sm">CÔNG TY TNHH MTV XD &amp; TM NHẤT VŨ</div>
            <div class="text-[11px] text-amber-400">Website: nhatvu.com</div>
          </div>
        </div>
        <p class="leading-relaxed text-slate-300">
          Chuyên cung cấp Sơn nước Jotun, Dulux, Tito, Chống thấm Sika, Thiết bị vệ sinh, Gạch men ốp lát, Ngói lợp, Bồn nước, Bình nóng lạnh, Keo dán gạch &amp; chà ron chính hãng.
        </p>
        <ul class="space-y-1.5 text-slate-200">
          <li><i class="fa-solid fa-location-dot text-amber-400 mr-2"></i>Địa chỉ: 65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng</li>
          <li><i class="fa-solid fa-phone text-amber-400 mr-2"></i>Hotline: <a href="tel:0905343016" class="font-bold text-white hover:text-amber-300">0905.343.016</a> - <a href="tel:0905327257" class="font-bold text-white hover:text-amber-300">0905.327.257</a></li>
          <li><i class="fa-solid fa-globe text-amber-400 mr-2"></i>Website: nhatvu.com</li>
        </ul>
      </div>

      <!-- Danh mục sản phẩm -->
      <div class="space-y-2">
        <h3 class="font-bold text-white text-sm uppercase border-b border-white/15 pb-1.5">Danh Mục Sản Phẩm</h3>
        <div class="grid grid-cols-2 gap-1.5 text-slate-300">
          <a href="#sec-son" class="hover:text-amber-400">• Sơn Jotun / Dulux</a>
          <a href="#sec-tbvs" class="hover:text-amber-400">• Thiết bị vệ sinh</a>
          <a href="#sec-gach-men" class="hover:text-amber-400">• Gạch men Đồng Tâm</a>
          <a href="#sec-ngoi-lop" class="hover:text-amber-400">• Ngói lợp DIC / Đất Việt</a>
          <a href="#sec-bon-nuoc" class="hover:text-amber-400">• Bồn nước Sơn Hà / Tân Á</a>
          <a href="#sec-binh-nong-lanh" class="hover:text-amber-400">• Bình nóng lạnh Ariston</a>
          <a href="#sec-keo-dan-gach" class="hover:text-amber-400">• Keo dán gạch &amp; Chà ron</a>
          <a href="#form-bao-gia" class="hover:text-amber-400">• Yêu cầu báo giá sỉ</a>
        </div>
      </div>

      <!-- Liên kết Kết nối -->
      <div class="space-y-2">
        <h3 class="font-bold text-white text-sm uppercase border-b border-white/15 pb-1.5">Kết Nối Với Nhất Vũ</h3>
        <p class="text-slate-300">Theo dõi hoặc liên hệ trực tiếp qua Facebook, Zalo và Google Map chính thức:</p>
        <div class="flex flex-wrap gap-2 pt-1">
          <a href="https://www.facebook.com/profile.php?id=100018933160246" target="_blank" rel="noopener noreferrer" class="bg-[#1877F2] hover:bg-blue-600 text-white px-3 py-1.5 rounded font-semibold inline-flex items-center gap-1.5">
            <i class="fa-brands fa-facebook-f"></i> Facebook
          </a>
          <a href="https://zalo.me/0905343016" target="_blank" rel="noopener noreferrer" class="bg-[#0068FF] hover:bg-blue-500 text-white px-3 py-1.5 rounded font-semibold inline-flex items-center gap-1.5">
            <i class="fa-solid fa-comment-dots"></i> Chat Zalo
          </a>
          <a href="https://share.google/1XOj3LATI4UPCFgoy" target="_blank" rel="noopener noreferrer" class="bg-brand-accent hover:bg-orange-600 text-white px-3 py-1.5 rounded font-semibold inline-flex items-center gap-1.5">
            <i class="fa-solid fa-map-location-dot"></i> Bản Đồ Map
          </a>
        </div>
      </div>

    </div>
    <div class="flatsome-container pt-4 text-center text-[11px] text-slate-400">
      Copyright 2026 © <strong>nhatvu.com - CÔNG TY TNHH MỘT THÀNH VIÊN XD &amp; TM NHẤT VŨ</strong>. Địa chỉ: 65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng.
    </div>
  </footer>

  <!-- =========================================================================
       CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) TƯƠNG THÍCH MÁY TÍNH & ĐIỆN THOẠI
       ========================================================================= -->
  <div class="fixed right-3 bottom-4 z-50 flex flex-col items-end gap-2.5">
    
    <!-- Nút Zalo nổi bật -->
    <a href="https://zalo.me/0905343016" target="_blank" rel="noopener noreferrer" title="Chat Zalo: 0905343016" class="flex items-center gap-2 bg-[#0068FF] hover:bg-blue-600 text-white pl-3 pr-3.5 py-2 rounded-full shadow-lg transition">
      <span class="w-6 h-6 rounded-full bg-white text-[#0068FF] font-extrabold text-[11px] flex items-center justify-center shrink-0">Zalo</span>
      <span class="text-xs font-bold whitespace-nowrap">Chat Zalo</span>
    </a>

    <!-- Nút Facebook nổi bật -->
    <a href="https://www.facebook.com/profile.php?id=100018933160246" target="_blank" rel="noopener noreferrer" title="Facebook Nhất Vũ" class="flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white pl-3 pr-3.5 py-2 rounded-full shadow-lg transition">
      <span class="w-6 h-6 rounded-full bg-white text-[#1877F2] flex items-center justify-center shrink-0">
        <i class="fa-brands fa-facebook-f text-xs"></i>
      </span>
      <span class="text-xs font-bold whitespace-nowrap">Facebook</span>
    </a>

    <!-- Nút Hotline 1 -->
    <a href="tel:0905343016" title="Gọi 0905343016" class="floating-pulse flex items-center gap-2 bg-brand-accent hover:bg-orange-700 text-white pl-3 pr-3.5 py-2 rounded-full shadow-lg transition">
      <span class="w-6 h-6 rounded-full bg-white text-brand-accent flex items-center justify-center shrink-0">
        <i class="fa-solid fa-phone text-xs"></i>
      </span>
      <span class="text-xs font-extrabold whitespace-nowrap">0905.343.016</span>
    </a>

    <!-- Nút Hotline 2 -->
    <a href="tel:0905327257" title="Gọi 0905327257" class="flex items-center gap-2 bg-brand-primary hover:bg-slate-800 text-white pl-3 pr-3.5 py-2 rounded-full shadow-lg transition border border-white/20">
      <span class="w-6 h-6 rounded-full bg-amber-400 text-brand-primary flex items-center justify-center shrink-0">
        <i class="fa-solid fa-phone-volume text-xs"></i>
      </span>
      <span class="text-xs font-extrabold whitespace-nowrap">0905.327.257</span>
    </a>

  </div>

  <!-- =========================================================================
       MODAL XEM CHI TIẾT SẢN PHẨM & ẢNH THỰC TẾ
       ========================================================================= -->
  <div id="productModal" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center p-3">
    <div class="bg-white rounded-lg max-w-lg w-full overflow-hidden shadow-2xl border border-slate-200">
      <div class="bg-brand-primary text-white px-4 py-3 flex items-center justify-between">
        <h3 id="modalTitle" class="text-sm font-bold pr-4">Chi tiết sản phẩm</h3>
        <button type="button" onclick="closeProductModal()" class="w-7 h-7 rounded bg-white/10 hover:bg-white/20 flex items-center justify-center">
          <i class="fa-solid fa-xmark"></i>
        </button>
      </div>
      <div class="p-4 space-y-3">
        <div class="relative rounded border border-slate-200 overflow-hidden bg-slate-50 flex items-center justify-center h-64">
          <span id="modalBadge" class="flatsome-discount-badge">-18%</span>
          <img id="modalImage" src="" alt="Ảnh sản phẩm thực tế" class="max-h-full max-w-full object-contain" />
        </div>
        <div class="flex items-baseline gap-3">
          <span id="modalSalePrice" class="text-lg font-extrabold text-brand-accent"></span>
          <span id="modalOldPrice" class="text-xs text-slate-400 line-through"></span>
        </div>
        <p class="text-xs text-slate-600 leading-relaxed">
          Sản phẩm phân phối chính hãng tại <strong>CÔNG TY TNHH MTV XD &amp; TM NHẤT VŨ</strong> (65 Nguyễn Quang Diêu, Phường Hòa Xuân, TP Đà Nẵng). Liên hệ trực tiếp để nhận chiết khấu tốt nhất theo số lượng công trình.
        </p>
        <div class="pt-2 flex flex-wrap gap-2">
          <a href="tel:0905343016" class="flex-1 bg-brand-accent hover:bg-orange-700 text-white text-center py-2.5 px-3 rounded text-xs font-bold">
            <i class="fa-solid fa-phone mr-1"></i>Gọi 0905.343.016
          </a>
          <a href="https://zalo.me/0905343016" target="_blank" rel="noopener noreferrer" class="flex-1 bg-[#0068FF] hover:bg-blue-700 text-white text-center py-2.5 px-3 rounded text-xs font-bold">
            <i class="fa-solid fa-comment-dots mr-1"></i>Nhắn Zalo Báo Giá
          </a>
        </div>
      </div>
    </div>
  </div>

  <!-- =========================================================================
       JAVASCRIPT: DỮ LIỆU 19 ẢNH SẢN PHẨM THỰC TẾ GOOGLE DRIVE & DANH MỤC CHUẨN MẪU
       ========================================================================= -->
  <script>
    // Danh sách đúng 19 ID file ảnh sản phẩm thực tế từ Google Drive do khách hàng cung cấp
    const driveProductImageIds = [
      '1P2fePSvPXm6YIcNDixVa0YwFWshcHFDY', // 1
      '11z7ir7cmqEcdrYuAThZvpOhgUVFsLUnP', // 2
      '1KTDzdSGqiXWuLZDkPoDD7oZZVL-5F3Rr', // 3
      '1X31hmhpLVVORV-tmMSZYzBO-qtpyusry', // 4
      '171kMlCqYFeFpvYcgH1wQbaIMszY0Ns3O', // 5
      '1t8U7WQsmDbGWzmSelkxzjVv8M0BvIxAg', // 6
      '1uqL6ACCB5ne0G1BYkXCurdnrsf1m2lr4', // 7
      '1NwR4v0eypEtIwPi6NJVJCKoNCFFQ8G54', // 8
      '19jauCH_X7lcc0KNlu2OJ75CRiw3ArT7r', // 9
      '1_HXfxWiPLtWiayxMPjgFCsl1WS1wGb7h', // 10
      '1ciwHcFfmGbsIyjTsi9KlyIsx6EXBNJTN', // 11
      '1vHG-pgeryaSItJoQ5ciiCGSWA7SJSU8c', // 12
      '1X-ECML9CKN4ycBfVFu4pC0wnqzTS12CP', // 13
      '1CGBZ4cuB7DMWadnoktlMoji6MB3dioC-', // 14
      '17YrxXteZmzhvVRYgfaklNGC2hKjN09N8', // 15
      '19k5uWHn_xeas2_BMP_JgBDwwu-IysSRP', // 16
      '1oah4j6YAPIsJacMYQFJ0JGVemrMwqCgf', // 17
      '15IWAPhzVLsyUO5TDRoWXxvncrHoFcH1_', // 18
      '1WLKyUBxRc63xFN9GBUhFcqE0xPo0sQKh'  // 19
    ];

    // Hàm tạo URL ảnh trực tiếp từ Google Drive
    function getDriveImgUrl(fileId) {
      return `https://drive.google.com/thumbnail?id=${fileId}&sz=w800`;
    }

    // Xử lý dự phòng đa tầng nếu ảnh Google Drive gặp giới hạn băng thông trình duyệt
    function handleDriveImgError(imgEl, fileId, fallbackText) {
      const step = imgEl.getAttribute('data-fallback-step') || '0';
      if (step === '0') {
        imgEl.setAttribute('data-fallback-step', '1');
        imgEl.src = `https://lh3.googleusercontent.com/d/${fileId}=w800`;
      } else {
        imgEl.onerror = null;
        imgEl.src = `https://placehold.co/600x600/f1f5f9/0b3b68?text=${fallbackText}`;
      }
    }

    // Dữ liệu 7 Danh mục sản phẩm lấy từ web mẫu noithatngonguyen.com kết hợp 19 ảnh thực tế
    const catalogSections = [
      {
        id: 'sec-son',
        title: 'SƠN',
        subCategories: ['Jotun', 'Dulux - Maxilite', 'Tito', 'Chống thấm'],
        products: [
          {
            name: 'Sơn Ngoại Thất Jotun Jotashield Bền Màu Tối Ưu',
            driveId: driveProductImageIds[0],
            discount: '-18%',
            oldPrice: '2.650.000₫',
            salePrice: '2.170.000₫'
          },
          {
            name: 'Sơn Ngoại Thất Jotun Tough Shield Max Cao Cấp',
            driveId: driveProductImageIds[1],
            discount: '-16%',
            oldPrice: '1.890.000₫',
            salePrice: '1.580.000₫'
          },
          {
            name: 'Sơn Nội Thất Jotun Essence Che Phủ Tối Đa Bóng',
            driveId: driveProductImageIds[2],
            discount: '-15%',
            oldPrice: '1.450.000₫',
            salePrice: '1.230.000₫'
          },
          {
            name: 'Sơn Nước Ngoại Thất Dulux Weathershield Bề Mặt Bóng',
            driveId: driveProductImageIds[3],
            discount: '-17%',
            oldPrice: '2.780.000₫',
            salePrice: '2.310.000₫'
          },
          {
            name: 'Chất Chống Thấm Sika Raintite & Sơn Chống Thấm Tito',
            driveId: driveProductImageIds[4],
            discount: '-20%',
            oldPrice: '1.350.000₫',
            salePrice: '1.080.000₫'
          }
        ]
      },
      {
        id: 'sec-tbvs',
        title: 'THIẾT BỊ VỆ SINH',
        subCategories: ['Bồn cầu', 'Sen vòi', 'Lavabo', 'Gương', 'Phụ kiện nhà tắm'],
        products: [
          {
            name: 'Sen Cây Tắm Inax BFV-615S-8C Nóng Lạnh Chính Hãng',
            driveId: driveProductImageIds[5],
            discount: '-20%',
            oldPrice: '4.850.000₫',
            salePrice: '3.880.000₫'
          },
          {
            name: 'Sen Tắm Âm Tường Inax BFV-81SEHW Cao Cấp',
            driveId: driveProductImageIds[6],
            discount: '-18%',
            oldPrice: '5.400.000₫',
            salePrice: '4.420.000₫'
          },
          {
            name: 'Sen Cây Viglacera Nóng Lạnh VG596 / VG519 Đồng Mạ Crom',
            driveId: driveProductImageIds[7],
            discount: '-22%',
            oldPrice: '3.650.000₫',
            salePrice: '2.850.000₫'
          },
          {
            name: 'Bồn Cầu Khối Viglacera & Inax Men Kháng Khuẩn',
            driveId: driveProductImageIds[8],
            discount: '-19%',
            oldPrice: '4.200.000₫',
            salePrice: '3.400.000₫'
          },
          {
            name: 'Bộ Chậu Rửa Lavabo, Gương & Phụ Kiện Phòng Tắm Caesar',
            driveId: driveProductImageIds[9],
            discount: '-15%',
            oldPrice: '2.300.000₫',
            salePrice: '1.950.000₫'
          }
        ]
      },
      {
        id: 'sec-gach-men',
        title: 'GẠCH MEN',
        subCategories: ['Đồng Tâm', 'Kimgres', 'Gạch 80x80', 'Gạch 60x60', 'Gạch 30x60'],
        products: [
          {
            name: 'Gạch Porcelain Kháng Khuẩn Đồng Tâm 8080FANSIPAN007-FP',
            driveId: driveProductImageIds[10],
            discount: '-15%',
            oldPrice: '395.000₫/m²',
            salePrice: '335.000₫/m²'
          },
          {
            name: 'Gạch Porcelain 2 Da Đồng Tâm 8080PLATINUM003 (80x80cm)',
            driveId: driveProductImageIds[11],
            discount: '-16%',
            oldPrice: '410.000₫/m²',
            salePrice: '345.000₫/m²'
          },
          {
            name: 'Gạch Porcelain Kháng Khuẩn Đồng Tâm 8080DONGVAN010-FP-H+',
            driveId: driveProductImageIds[12],
            discount: '-14%',
            oldPrice: '380.000₫/m²',
            salePrice: '325.000₫/m²'
          },
          {
            name: 'Gạch Ốp Lát Kimgres Vân Đá Tự Nhiên Cao Cấp 60x60cm',
            driveId: driveProductImageIds[13],
            discount: '-18%',
            oldPrice: '295.000₫/m²',
            salePrice: '242.000₫/m²'
          }
        ]
      },
      {
        id: 'sec-ngoi-lop',
        title: 'NGÓI LỢP',
        subCategories: ['DIC', 'Ngói Đất Việt'],
        products: [
          {
            name: 'Ngói Màu Cao Cấp DIC Đỏ Tươi DT10S & Đỏ Đậm DD09S',
            driveId: driveProductImageIds[14],
            discount: '-15%',
            oldPrice: '36.000₫/viên',
            salePrice: '30.500₫/viên'
          },
          {
            name: 'Ngói Lợp Đất Việt Xám Tro XT07S & Nâu Socola NN02S',
            driveId: driveProductImageIds[15],
            discount: '-14%',
            oldPrice: '35.000₫/viên',
            salePrice: '30.000₫/viên'
          }
        ]
      },
      {
        id: 'sec-bon-nuoc',
        title: 'BỒN NƯỚC',
        subCategories: ['Letton', 'Sơn Hà', 'Tân Á'],
        products: [
          {
            name: 'Bồn Nước Inox Tân Á 8 Đứng 1000 Lít TA8D1000 (F940)',
            driveId: driveProductImageIds[16],
            discount: '-18%',
            oldPrice: '4.150.000₫',
            salePrice: '3.400.000₫'
          },
          {
            name: 'Bồn Nước Sơn Hà & Letton Inox / Nhựa Cao Cấp Đứng - Ngang',
            driveId: driveProductImageIds[0],
            discount: '-17%',
            oldPrice: '4.350.000₫',
            salePrice: '3.610.000₫'
          }
        ]
      },
      {
        id: 'sec-binh-nong-lanh',
        title: 'BÌNH NÓNG LẠNH',
        subCategories: ['Ariston', 'Ferroli'],
        products: [
          {
            name: 'Máy Nước Nóng Ariston AN2 30 RS 2.5 FE 30 Lít 2.5KW',
            driveId: driveProductImageIds[17],
            discount: '-19%',
            oldPrice: '3.850.000₫',
            salePrice: '3.120.000₫'
          },
          {
            name: 'Máy Nước Nóng Ferroli Divo SSN 4.5S 4.5KW & QQ Evo 15L',
            driveId: driveProductImageIds[5],
            discount: '-20%',
            oldPrice: '2.750.000₫',
            salePrice: '2.200.000₫'
          }
        ]
      },
      {
        id: 'sec-keo-dan-gach',
        title: 'KEO DÁN GẠCH, CHÀ RON',
        subCategories: ['Bestmix', 'Đồng Tâm', 'Keo cá sấu', 'Sika'],
        products: [
          {
            name: 'Keo Dán Gạch Gecko Floor Đồng Tâm Chuyên Lát Nền Bao 25Kg',
            driveId: driveProductImageIds[18],
            discount: '-15%',
            oldPrice: '285.000₫/bao',
            salePrice: '242.000₫/bao'
          },
          {
            name: 'Keo Dán Gạch Sika Tilebond GP & Keo Chà Ron Cá Sấu Silver',
            driveId: driveProductImageIds[4],
            discount: '-16%',
            oldPrice: '260.000₫/bao',
            salePrice: '218.000₫/bao'
          }
        ]
      }
    ];

    // Render toàn bộ các Section danh mục sản phẩm chuẩn bố cục Flatsome
    function renderCatalog(filterKeyword = '') {
      const container = document.getElementById('catalogContainer');
      const kw = filterKeyword.trim().toLowerCase();
      let html = '';

      catalogSections.forEach((sec) => {
        const filteredProducts = sec.products.filter((p) =>
          !kw || p.name.toLowerCase().includes(kw) || sec.title.toLowerCase().includes(kw)
        );

        if (filteredProducts.length === 0) return;

        const subCatsHtml = sec.subCategories
          .map((sub) => `<a href="#${sec.id}" class="cat-pill-compact">${sub}</a>`)
          .join('');

        const productsHtml = filteredProducts
          .map((prod, idx) => {
            const imgUrl = getDriveImgUrl(prod.driveId);
            const safeName = prod.name.replace(/'/g, "\\'");
            return `
              <div class="col">
                <div class="product-small box cursor-pointer" onclick="openProductModal('${safeName}', '${prod.driveId}', '${prod.discount}', '${prod.oldPrice}', '${prod.salePrice}')">
                  <!-- Góc trên bên trái: % Giảm giá giống Flatsome (không thêm nhãn dán thừa) -->
                  <div class="box-image relative bg-slate-50 border-b border-slate-100 aspect-square flex items-center justify-center overflow-hidden">
                    <div class="flatsome-discount-badge">${prod.discount}</div>
                    <img
                      src="${imgUrl}"
                      onerror="handleDriveImgError(this, '${prod.driveId}', 'San+Pham+Nhat+Vu')"
                      alt="${prod.name}"
                      loading="lazy"
                      class="w-full h-full object-cover hover:scale-105 transition duration-300"
                    />
                  </div>
                  <!-- Box Text: Tên sản phẩm đầy đủ không mất chữ + Giá gốc & Giá giảm -->
                  <div class="box-text p-2.5 sm:p-3 flex-1 flex flex-col justify-between">
                    <h3 class="product-title-full">${prod.name}</h3>
                    <div class="pt-1 border-t border-slate-100 flex flex-wrap items-baseline gap-1.5">
                      <span class="text-xs sm:text-sm font-extrabold text-brand-accent">${prod.salePrice}</span>
                      <span class="text-[11px] text-slate-400 line-through">${prod.oldPrice}</span>
                    </div>
                  </div>
                </div>
              </div>
            `;
          })
          .join('');

        html += `
          <section id="${sec.id}" class="flatsome-container">
            <div class="bg-white rounded-lg border border-slate-200 p-3.5 sm:p-4 shadow-sm">
              <!-- Tiêu đề danh mục & Các tiểu mục nhỏ gọn trên 1 hàng -->
              <div class="flex flex-wrap items-center justify-between gap-2 border-b-2 border-brand-primary pb-2.5 mb-3.5">
                <h2 class="text-sm sm:text-base font-extrabold text-brand-primary uppercase whitespace-nowrap">
                  ${sec.title}
                </h2>
                <div class="flex flex-wrap items-center gap-1.5">
                  ${subCatsHtml}
                  <a href="#form-bao-gia" class="cat-pill-compact !bg-brand-primary !text-white !border-brand-primary">Xem thêm &gt;</a>
                </div>
              </div>
              <!-- Grid sản phẩm: Chia 2 cột trên điện thoại (grid-cols-2), 4-5 cột trên máy tính -->
              <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-2.5 sm:gap-3.5">
                ${productsHtml}
              </div>
            </div>
          </section>
        `;
      });

      container.innerHTML = html;
    }

    // Render đầy đủ 19 ảnh thực tế từ Google Drive để khách hàng kiểm tra trực quan
    function renderAll19RealPhotos() {
      const grid = document.getElementById('allRealPhotosGrid');
      const mappedNames = [
        'Sơn Ngoại Thất Jotun Jotashield Bền Màu',
        'Sơn Ngoại Thất Jotun Tough Shield Max',
        'Sơn Nội Thất Jotun Essence Bóng',
        'Sơn Nước Dulux Weathershield Chính Hãng',
        'Chống Thấm Sika & Phụ Gia Xây Dựng',
        'Sen Cây Tắm Nóng Lạnh Inax BFV-615S',
        'Sen Tắm Âm Tường Inax Cao Cấp',
        'Sen Cây Nóng Lạnh Viglacera VG596',
        'Bồn Cầu Khối Men Tuyết Kháng Khuẩn',
        'Chậu Rửa Lavabo & Phụ Kiện Phòng Tắm',
        'Gạch Porcelain Đồng Tâm 8080FANSIPAN',
        'Gạch Porcelain 2 Da Đồng Tâm 80x80',
        'Gạch Porcelain Kháng Khuẩn 8080DONGVAN',
        'Gạch Ốp Lát Kimgres Vân Đá 60x60',
        'Ngói Màu Lợp Nhà DIC Đỏ Tươi DT10S',
        'Ngói Lợp Đất Việt Cao Cấp Chính Hãng',
        'Bồn Nước Inox Tân Á / Sơn Hà Chính Hãng',
        'Bình Nóng Lạnh Ariston & Ferroli',
        'Keo Dán Gạch Đồng Tâm, Sika & Chà Ron'
      ];

      grid.innerHTML = driveProductImageIds
        .map((id, index) => {
          const title = mappedNames[index] || `Sản phẩm thực tế Nhất Vũ #${index + 1}`;
          const safeTitle = title.replace(/'/g, "\\'");
          return `
            <div class="product-small box cursor-pointer" onclick="openProductModal('${safeTitle}', '${id}', '-15%', 'Liên hệ', 'Giá ưu đãi tại kho')">
              <div class="box-image relative bg-slate-50 aspect-square overflow-hidden border-b border-slate-100">
                <div class="flatsome-discount-badge">-15%</div>
                <img
                  src="${getDriveImgUrl(id)}"
                  onerror="handleDriveImgError(this, '${id}', 'Anh+Thuc+Te+${index + 1}')"
                  alt="${title}"
                  loading="lazy"
                  class="w-full h-full object-cover hover:scale-105 transition duration-300"
                />
              </div>
              <div class="box-text p-2.5 flex-1 flex flex-col justify-between">
                <h3 class="product-title-full">${title}</h3>
                <div class="flex items-center justify-between text-[11px] pt-1 border-t border-slate-100">
                  <span class="font-bold text-brand-accent">Giá tốt tại kho</span>
                  <span class="text-slate-400 line-through">Giá niêm yết</span>
                </div>
              </div>
            </div>
          `;
        })
        .join('');
    }

    // Logic Tự trượt 2 Banner
    let currentBannerIndex = 0;
    const totalBanners = 2;
    let bannerInterval = null;

    function updateBannerUI() {
      const slides = document.querySelectorAll('.banner-slide');
      const dots = document.querySelectorAll('.banner-dot');
      slides.forEach((slide, idx) => {
        if (idx === currentBannerIndex) {
          slide.classList.add('active');
        } else {
          slide.classList.remove('active');
        }
      });
      dots.forEach((dot, idx) => {
        dot.className = idx === currentBannerIndex
          ? 'banner-dot w-2.5 h-2.5 rounded-full bg-white transition'
          : 'banner-dot w-2.5 h-2.5 rounded-full bg-white/40 transition';
      });
    }

    function changeBanner(step) {
      currentBannerIndex = (currentBannerIndex + step + totalBanners) % totalBanners;
      updateBannerUI();
      resetBannerTimer();
    }

    function goToBanner(index) {
      currentBannerIndex = index;
      updateBannerUI();
      resetBannerTimer();
    }

    function resetBannerTimer() {
      if (bannerInterval) clearInterval(bannerInterval);
      bannerInterval = setInterval(() => {
        currentBannerIndex = (currentBannerIndex + 1) % totalBanners;
        updateBannerUI();
      }, 4500);
    }

    // Tìm kiếm sản phẩm
    function handleSearch(e) {
      e.preventDefault();
      const desktopVal = document.getElementById('searchInputDesktop')?.value || '';
      const mobileVal = document.getElementById('searchInputMobile')?.value || '';
      const keyword = desktopVal || mobileVal;
      renderCatalog(keyword);
      document.getElementById('catalogContainer').scrollIntoView({ behavior: 'smooth' });
    }

    // Đóng/mở Menu Điện thoại
    const mobileMenuOverlay = document.getElementById('mobileMenuOverlay');
    document.getElementById('mobileMenuBtn').addEventListener('click', () => {
      mobileMenuOverlay.classList.remove('hidden');
    });
    document.getElementById('closeMobileMenuBtn').addEventListener('click', () => {
      mobileMenuOverlay.classList.add('hidden');
    });
    function closeMobileMenu() {
      mobileMenuOverlay.classList.add('hidden');
    }

    // Modal xem chi tiết sản phẩm
    function openProductModal(name, driveId, discount, oldPrice, salePrice) {
      document.getElementById('modalTitle').textContent = name;
      const imgEl = document.getElementById('modalImage');
      imgEl.removeAttribute('data-fallback-step');
      imgEl.onerror = function () {
        handleDriveImgError(imgEl, driveId, 'San+Pham+Nhat+Vu');
      };
      imgEl.src = getDriveImgUrl(driveId);
      document.getElementById('modalBadge').textContent = discount;
      document.getElementById('modalSalePrice').textContent = salePrice;
      document.getElementById('modalOldPrice').textContent = oldPrice;
      const modal = document.getElementById('productModal');
      modal.classList.remove('hidden');
      modal.classList.add('flex');
    }

    function closeProductModal() {
      const modal = document.getElementById('productModal');
      modal.classList.add('hidden');
      modal.classList.remove('flex');
    }

    // Xử lý gửi Form Báo Giá
    function submitQuoteForm(e) {
      e.preventDefault();
      const name = document.getElementById('qName').value.trim();
      const phone = document.getElementById('qPhone').value.trim();
      const cat = document.getElementById('qCategory').value;
      const msgBox = document.getElementById('quoteSuccessMsg');
      msgBox.innerHTML = `<i class="fa-solid fa-circle-check mr-1.5"></i>Cảm ơn <strong>${name}</strong> (${phone})! Yêu cầu báo giá danh mục <strong>${cat}</strong> đã được ghi nhận. Bộ phận kinh doanh Nhất Vũ (0905.343.016 - 0905.327.257) sẽ liên hệ báo giá ngay.`;
      msgBox.classList.remove('hidden');
      document.getElementById('quoteForm').reset();
    }

    // Khởi chạy khi tải trang
    window.onload = function () {
      renderCatalog();
      renderAll19RealPhotos();
      resetBannerTimer();
    };
  </script>
</body>
</html>
