---
layout: home
title: (주) 에스비테크
permalink: /
cover: https://sbtech-korea.github.io/assets/main.jpg
---

<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>(주)에스비테크 - Home</title>

  <style>
    :root{
      --blue:#2563eb;
      --blue2:#1d4ed8;
      --gray50:#f9fafb;
      --gray100:#f3f4f6;
      --gray200:#e5e7eb;
      --gray400:#9ca3af;
      --gray600:#4b5563;
      --gray700:#374151;
      --gray800:#1f2937;
      --gray900:#111827;
      --white:#fff;
      --shadow: 0 10px 20px rgba(0,0,0,.08);
      --shadow2: 0 14px 30px rgba(0,0,0,.12);
      --radius: 14px;
      --container: 1200px;
    }

    *{ box-sizing: border-box; }
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple SD Gothic Neo", "Noto Sans KR", sans-serif;
      color: var(--gray900);
      background: linear-gradient(to bottom, var(--gray50), var(--gray100));
    }
    a{ color: inherit; text-decoration: none; }
    .container{
      max-width: var(--container);
      margin: 0 auto;
      padding: 0 16px;
    }

    /* Header */
    header{
      position: sticky;
      top: 0;
      z-index: 50;
      background: rgba(255,255,255,.8);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--gray200);
    }
    .header-inner{
      display:flex;
      align-items:center;
      justify-content: space-between;
      padding: 16px 0;
    }
    .brand{
      display:flex;
      align-items:center;
      gap: 10px;
      font-weight: 800;
      font-size: 20px;
    }
    .logo-box{
      width:40px;
      height:40px;
      background: var(--blue);
      border-radius: 10px;
    }

    nav{
      display:none;
      align-items:center;
      gap: 28px;
      color: var(--gray600);
      font-weight: 600;
    }
    nav a, nav button{
      color: var(--gray600);
      background: transparent;
      border: 0;
      padding: 8px 0;
      cursor: pointer;
      font: inherit;
      display: inline-flex;
      align-items:center;
      gap: 6px;
    }
    nav a:hover, nav button:hover{ color: var(--blue); }

    @media (min-width: 768px){
      nav{ display:flex; }
    }

    /* Dropdown */
    .dropdown{
      position: relative;
    }
    .dropdown-menu{
      position:absolute;
      left:0;
      top: 100%;
      margin-top: 8px;
      width: 200px;
      background: var(--white);
      border: 1px solid var(--gray200);
      border-radius: 10px;
      box-shadow: var(--shadow);
      padding: 6px;
      display:none;
    }
    .dropdown-menu a{
      display:block;
      padding: 10px 12px;
      border-radius: 8px;
      font-size: 14px;
      color: var(--gray700);
    }
    .dropdown-menu a:hover{
      background: var(--gray100);
    }
    .dropdown.open .dropdown-menu{
      display:block;
    }
    .chev{
      width: 16px;
      height: 16px;
      display:inline-block;
      transform: translateY(1px);
    }

    /* Buttons */
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap: 8px;
      border-radius: 14px;
      border: 1px solid transparent;
      padding: 14px 22px;
      font-weight: 700;
      cursor: pointer;
      user-select:none;
      transition: transform .12s ease, box-shadow .12s ease, background .12s ease, border-color .12s ease;
      text-decoration:none;
    }
    .btn:active{ transform: translateY(1px); }

    .btn-primary{
      background: var(--blue);
      color: white;
    }
    .btn-primary:hover{ background: var(--blue2); }
    .btn-outline{
      background: transparent;
      border-color: var(--gray200);
      color: var(--gray900);
    }
    .btn-outline:hover{ background: var(--gray100); }

    .btn-lg{ padding: 16px 26px; font-size: 18px; }

    /* Sections */
    section{ padding: 80px 0; }
    .section-white{ background: white; }
    .section-gray{ background: var(--gray50); }

    .center{ text-align:center; }
    h1{
      margin:0 0 18px 0;
      line-height: 1.15;
      font-size: 42px;
      letter-spacing: -0.02em;
    }
    .accent{ color: var(--blue); }
    .lead{
      color: var(--gray600);
      font-size: 20px;
      max-width: 760px;
      margin: 0 auto 28px;
    }
    @media (min-width: 768px){
      h1{ font-size: 58px; }
    }

    /* Hero background */
    .hero{
      position: relative;
      overflow:hidden;
      padding: 90px 0;
    }
    .hero-bg{
      position:absolute;
      inset:0;
      background: url('/battery-bg.jpg') center/cover no-repeat;
      opacity: .1;
      pointer-events:none;
    }
    .hero-inner{ position:relative; z-index:1; }

    .hero-actions{
      display:flex;
      flex-direction: column;
      gap: 12px;
      justify-content:center;
      align-items:center;
      margin-top: 10px;
    }
    @media (min-width: 640px){
      .hero-actions{ flex-direction: row; }
    }

    /* Company info grid */
    .grid-2{
      display:grid;
      grid-template-columns: 1fr;
      gap: 28px;
      margin-top: 20px;
    }
    @media (min-width: 1024px){
      .grid-2{ grid-template-columns: 1fr 1fr; }
    }
    .placeholder{
      height: 320px;
      background: var(--gray200);
      border-radius: var(--radius);
      display:flex;
      align-items:center;
      justify-content:center;
      color: var(--gray400);
      font-weight: 700;
    }

    /* Cards grid */
    .grid-cards{
      display:grid;
      grid-template-columns: 1fr;
      gap: 18px;
      margin-top: 24px;
    }
    @media (min-width: 640px){
      .grid-cards{ grid-template-columns: repeat(2, 1fr); }
    }
    @media (min-width: 1024px){
      .grid-cards{ grid-template-columns: repeat(5, 1fr); }
    }

    .card{
      border-radius: 16px;
      background: white;
      box-shadow: var(--shadow);
      overflow:hidden;
      transition: transform .2s ease, box-shadow .2s ease;
    }
    .card:hover{
      transform: translateY(-6px);
      box-shadow: var(--shadow2);
    }
    .card-img{
      height: 190px;
      background: var(--gray200);
      display:flex;
      align-items:center;
      justify-content:center;
      color: var(--gray400);
      font-weight: 700;
    }
    .card-body{ padding: 18px; }
    .card-title{ margin: 0 0 10px 0; font-size: 18px; }
    .card-desc{ margin: 0; color: var(--gray700); font-size: 14px; line-height: 1.6; }

    /* Detail blocks */
    .detail-box{
      border-radius: 18px;
      padding: 26px;
    }
    .detail-blue{ background: #eff6ff; }
    .detail-green{ background: #ecfdf5; }
    .detail-box h3{ margin:0 0 12px 0; font-size: 22px; }
    .detail-blue h3{ color: #1e40af; }
    .detail-green h3{ color: #166534; }
    .detail-box p{ color: var(--gray700); line-height: 1.7; margin: 10px 0; }
    .detail-box ul{ margin: 10px 0 0 0; padding-left: 18px; color: var(--gray700); line-height: 1.7; }

    /* Catalog */
    .catalog-actions{
      display:flex;
      flex-wrap: wrap;
      gap: 12px;
      justify-content:center;
      margin-top: 18px;
    }
    .btn-outline-blue{
      border-color: var(--blue);
      color: var(--blue);
      background: transparent;
    }
    .btn-outline-blue:hover{
      background: #eff6ff;
    }

    /* Marquee Gallery */
    .marquee-wrap{
      overflow:hidden;
      white-space: nowrap;
      padding: 16px 0;
    }
    .marquee{
      display:inline-flex;
      gap: 24px;
      animation: marquee 22s linear infinite;
      will-change: transform;
    }
    @keyframes marquee{
      0% { transform: translateX(0); }
      100% { transform: translateX(-50%); }
    }
    .gallery-card{
      width: 260px;
      background:white;
      border-radius: 14px;
      box-shadow: 0 8px 16px rgba(0,0,0,.08);
      overflow:hidden;
      transition: box-shadow .15s ease;
    }
    .gallery-card:hover{ box-shadow: 0 12px 24px rgba(0,0,0,.12); }
    .gallery-img{
      height: 190px;
      background: var(--gray200);
      display:flex;
      align-items:center;
      justify-content:center;
      color: var(--gray400);
      font-weight: 700;
    }
    .gallery-body{ padding: 14px; }
    .gallery-body h3{ margin:0 0 6px 0; font-size: 15px; }
    .gallery-body p{ margin:0; color: var(--gray600); font-size: 13px; }

    /* Support */
    .support-grid{
      display:grid;
      grid-template-columns: 1fr;
      gap: 26px;
      margin-top: 26px;
    }
    @media (min-width: 768px){
      .support-grid{ grid-template-columns: 1fr 1fr; gap: 40px; }
    }
    .info-item{
      display:flex;
      gap: 14px;
      align-items:flex-start;
    }
    .icon-box{
      width: 34px;
      height: 34px;
      border-radius: 10px;
      background: #dbeafe;
      display:flex;
      align-items:center;
      justify-content:center;
      flex: 0 0 auto;
      margin-top: 2px;
    }
    .info-item h4{ margin:0 0 4px 0; font-size: 14px; }
    .info-item p{ margin:0; color: var(--gray600); font-size: 14px; line-height: 1.4; }

    .form{
      display:flex;
      flex-direction: column;
      gap: 12px;
    }
    input, textarea{
      width: 100%;
      border: 1px solid var(--gray200);
      border-radius: 12px;
      padding: 12px 14px;
      font-size: 14px;
      outline: none;
      transition: border-color .12s ease, box-shadow .12s ease;
      background: white;
    }
    textarea{ resize: vertical; }
    input:focus, textarea:focus{
      border-color: #93c5fd;
      box-shadow: 0 0 0 4px rgba(59,130,246,.12);
    }

    /* Footer */
    footer{
      background: var(--gray900);
      color: white;
      padding: 48px 0;
    }
    .footer-grid{
      display:grid;
      grid-template-columns: 1fr;
      gap: 22px;
    }
    @media (min-width: 768px){
      .footer-grid{ grid-template-columns: repeat(4, 1fr); gap: 28px; }
    }
    .footer-title{
      font-weight: 800;
      font-size: 18px;
      margin: 0 0 10px 0;
    }
    .muted{ color: rgba(255,255,255,.65); }
    .footer-links{
      list-style:none;
      padding:0;
      margin:0;
      display:flex;
      flex-direction: column;
      gap: 10px;
    }
    .footer-links a{ color: rgba(255,255,255,.65); }
    .footer-links a:hover{ color: white; }

    .footer-bottom{
      border-top: 1px solid rgba(255,255,255,.12);
      margin-top: 26px;
      padding-top: 20px;
      text-align:center;
      color: rgba(255,255,255,.65);
      font-size: 14px;
    }
  </style>
</head>

<body>
  <!-- Hero -->
  <section class="hero" id="introduction">
    <div class="hero-bg"></div>
    <div class="container hero-inner center">
      <h1>
        배터리 No1 배터리 전문기업<br />
        <span class="accent">(주)에스비테크</span>
      </h1>
      <p class="lead">차량용밧테리 / 산업용밧테리 / UPS 밧테리 전문</p>

      <div class="hero-actions">
        <a class="btn btn-primary btn-lg" href="#">무료 체험 시작</a>
        <a class="btn btn-outline btn-lg" href="#">데모 보기</a>
      </div>
    </div>
  </section>

  <!-- Company Info -->
  <section class="section-white">
    <div class="container">
      <div class="center" style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">(주) 에스비테크</h2>
        <p class="lead" style="margin-bottom:0;">우리는 실제 차이를 만드는 솔루션을 만드는 데熱심합니다</p>
      </div>

      <div class="grid-2">
        <div class="placeholder">Company Image</div>

        <div>
          <h3 style="margin:0 0 12px 0; font-size: 26px;">산업용/자동차용 배터리 전문기업</h3>
          <p style="color:var(--gray700); line-height:1.8; margin:0 0 12px 0;">
            ※ 델코 전국 판매1위<br />
            ※ X-Pro 전국판매 1위<br />
            ※ GM 순정배터리 전국총판<br />
            ※ 쌍용용자동차 순정배터리 전국총판<br />
            ※ 아트라스 배터리 산업용 판매우수업체
          </p>
          <p style="color:var(--gray700); line-height:1.8; margin:0;">
            승용차/화물차/중장비/산업용/농기계/선박용/비상발전용 UPS 배터리 설치 및 공급
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Products -->
  <section class="section-gray" id="products">
    <div class="container">
      <div class="center" style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">제품안내</h2>
        <p class="lead" style="margin-bottom:0;">고객님께 가장 적합한 배터리 솔루션을 제공합니다</p>
      </div>

      <div class="grid-cards" id="batteryGrid"></div>
    </div>
  </section>

  <!-- Product Details -->
  <section class="section-white">
    <div class="container">
      <div class="center" style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">제품 상세 소개</h2>
        <p class="lead" style="margin-bottom:0;">차량용 배터리와 산업용 배터리의 특징과 장점을 확인하세요</p>
      </div>

      <div class="grid-2" style="gap: 36px;">
        <div class="detail-box detail-blue">
          <h3>차량용 배터리</h3>
          <p>
            전기차 및 하이브리드 차량에 최적화된 고성능 리튬 이온 배터리입니다.
            높은 에너지 밀도와 긴 수명을 제공하여 차량의 주행 성능과 효율성을 극대화합니다.
          </p>
          <p>특징:</p>
          <ul>
            <li>높은 에너지 밀도</li>
            <li>긴 수명 (5~8년)</li>
            <li>빠른 충전 속도</li>
            <li>안정적인 전력 공급</li>
            <li>환경 친화적 설계</li>
          </ul>
          <p>
            차량용 배터리는 차량의 전기 시스템을 안정적으로 지원하며,
            최신 기술로 제작되어 뛰어난 성능과 신뢰성을 제공합니다.
          </p>
        </div>

        <div class="detail-box detail-green">
          <h3>산업용 배터리</h3>
          <p>
            산업용 장비 및 시설에 적합한 고성능 배터리로,
            장시간 사용에 특화된 설계를 가지고 있습니다.
            저온 성능 우수하고, 장기적인 사용을 위한 내구성을 갖추고 있습니다.
          </p>
          <p>특징:</p>
          <ul>
            <li>장시간 사용 가능</li>
            <li>저온 성능 우수 (-20°C까지 작동)</li>
            <li>고신뢰성 설계</li>
            <li>장기적인 사용 수명</li>
            <li>안정적인 전력 공급</li>
          </ul>
          <p>
            산업용 배터리는 공장 자동화, 저장 시스템, 재생 에너지 저장 등
            다양한 산업 분야에서 안정적인 전력 공급을 제공합니다.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Catalog -->
  <section class="section-white" id="catalog">
    <div class="container center">
      <div style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">제품카다로그</h2>
        <p class="lead" style="margin-bottom:0;">자세한 정보를 위해 제품 카탈로그를 다운로드하세요</p>
      </div>

      <div class="catalog-actions">
        <a class="btn btn-primary" href="#">PDF 카탈로그 다운로드</a>
        <a class="btn btn-outline-blue" href="#">온라인 카탈로그 보기</a>
      </div>
    </div>
  </section>

  <!-- Gallery -->
  <section class="section-gray" id="gallery">
    <div class="container">
      <div class="center" style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">설치갤러리</h2>
        <p class="lead" style="margin-bottom:0;">설치 및 프로젝트를 직접 확인하세요</p>
      </div>

      <div class="marquee-wrap">
        <div class="marquee" id="galleryMarquee"></div>
      </div>
    </div>
  </section>

  <!-- Support -->
  <section class="section-white" id="support">
    <div class="container">
      <div class="center" style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">고객센터</h2>
        <p class="lead" style="margin-bottom:0;">궁금한 점이 있으신가요? 저희에게 말씀해주세요.</p>
      </div>

      <div class="support-grid">
        <div>
          <h3 style="margin:0 0 18px 0; font-size: 24px;">연락처 정보</h3>

          <div style="display:flex; flex-direction:column; gap:14px;">
            <div class="info-item">
              <div class="icon-box">☎</div>
              <div>
                <h4>전화</h4>
                <p>1588-1234</p>
              </div>
            </div>

            <div class="info-item">
              <div class="icon-box">✉</div>
              <div>
                <h4>이메일</h4>
                <p>support@sbtech.com</p>
              </div>
            </div>

            <div class="info-item">
              <div class="icon-box">📍</div>
              <div>
                <h4>사무실</h4>
                <p>123 비즈니스 아바니드<br />서울, 한국</p>
              </div>
            </div>
          </div>
        </div>

        <div>
          <h3 style="margin:0 0 18px 0; font-size: 24px;">메시지 보내기</h3>

          <form class="form" id="contactForm">
            <input id="emailInput" type="email" placeholder="이메일" required />
            <textarea id="messageInput" rows="4" placeholder="메시지" required></textarea>
            <button class="btn btn-primary" type="submit" style="width:100%;">메시지 보내기</button>
          </form>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="container">
      <div class="footer-grid">
        <div>
          <div style="display:flex; align-items:center; gap:10px; margin-bottom:12px;">
            <div style="width:32px;height:32px;background:var(--blue);border-radius:10px;"></div>
            <div class="footer-title" style="margin:0;">(주)에스비테크</div>
          </div>
          <p class="muted" style="margin:0;">미래를 위한 혁신적인 솔루션을 제공합니다.</p>
        </div>

        <div>
          <div class="footer-title">빠른 링크</div>
          <ul class="footer-links">
            <li><a href="#introduction">회사소개</a></li>
            <li><a href="#products">제품개요</a></li>
            <li><a href="#specifications">자동차배터리제원표</a></li>
            <li><a href="/locations">전국협력점안내</a></li>
            <li><a href="#catalog">제품카다로그</a></li>
            <li><a href="/gallery">설치갤러리</a></li>
            <li><a href="#support">고객센터</a></li>
          </ul>
        </div>

        <div>
          <div class="footer-title">서비스</div>
          <ul class="footer-links">
            <li><a href="#">웹 개발</a></li>
            <li><a href="#">모바일 앱</a></li>
            <li><a href="#">UI/UX 디자인</a></li>
            <li><a href="#">클라우드 솔루션</a></li>
          </ul>
        </div>

        <div>
          <div class="footer-title">연락처 정보</div>
          <ul class="footer-links">
            <li class="muted">(주)에스비테크</li>
            <li class="muted">주소: 경기도 김포시 금포로 1517(운양동)</li>
            <li class="muted">사업자번호: 137-86-31906</li>
            <li class="muted">대표자: 박승태</li>
            <li class="muted">TEL: 031-985-7315</li>
            <li class="muted">FAX: 031-985-1661</li>
            <li class="muted">E-mail: pst1001@naver.com</li>
          </ul>
        </div>
      </div>

      <div class="footer-bottom">
        <span id="copyright"></span>
      </div>
    </div>
  </footer>

  <script>
    // ----------------------------
    // Data (React의 batteries 배열)
    // ----------------------------
    const batteries = [
      {
        id: 1,
        name: "델코 배터리",
        description: "고성능 리튬 이온 배터리로, 전기차 및 하이브리드 차량에 최적화되어 있습니다. 높은 에너지 밀도와 긴 수명을 제공합니다.",
        image: "delco-battery.jpg"
      },
      {
        id: 2,
        name: "로케트 배터리",
        description: "산업용 장비 및 시설용 고성능 배터리로, 장시간 사용에 적합한 설계를 가지고 있습니다. 저온 성능 우수합니다.",
        image: "rocket-battery.jpg"
      },
      {
        id: 3,
        name: "아트라스 배터리",
        description: "전동 편의차 및 전동 도구용 배터리로, 가벼운 무게와 높은 성능을 동시에 제공합니다. 효율적인 충전 기능을 갖추고 있습니다.",
        image: "atlas-battery.jpg"
      },
      {
        id: 4,
        name: "엑스프로 배터리",
        description: "고출력 전기차용 배터리로, 빠른 충전 속도와 높은 출력력을 자랑합니다. 최신 기술로 제작되어 안정적인 성능을 제공합니다.",
        image: "xpro-battery.jpg"
      },
      {
        id: 5,
        name: "솔라이트 배터리",
        description: "친환경 에너지 솔루션으로, 재활용 가능한 재료로 제작되어 환경에 미치는 영향을 최소화합니다. 지속 가능한 에너지 공급을 목표로 합니다.",
        image: "solight-battery.jpg"
      }
    ];

    // ----------------------------
    // Render batteries cards
    // ----------------------------
    const batteryGrid = document.getElementById("batteryGrid");
    batteryGrid.innerHTML = batteries.map(b => `
      <div class="card">
        <div class="card-img">Battery Image</div>
        <div class="card-body">
          <h3 class="card-title">${b.name}</h3>
          <p class="card-desc">${b.description}</p>
        </div>
      </div>
    `).join("");

    // ----------------------------
    // Gallery marquee (1~10 두 번)
    // ----------------------------
    const galleryMarquee = document.getElementById("galleryMarquee");
    const items = Array.from({length: 10}, (_, i) => i + 1);
    const renderGalleryItem = (n, keyPrefix="") => `
      <a href="/gallery/${n}" aria-label="설치 갤러리 ${n}">
        <div class="gallery-card">
          <div class="gallery-img">설치 이미지 ${n}</div>
          <div class="gallery-body">
            <h3>설치 ${n}</h3>
            <p>프로젝트 설명이 여기에 옵니다</p>
          </div>
        </div>
      </a>
    `;
    galleryMarquee.innerHTML =
      items.map(n => renderGalleryItem(n, "")).join("") +
      items.map(n => renderGalleryItem(n, "duplicate-")).join("");

    // ----------------------------
    // Dropdown logic (React useState/useRef/useEffect 대체)
    // ----------------------------
    const companyDropdown = document.getElementById("companyDropdown");
    const productsDropdown = document.getElementById("productsDropdown");

    companyDropdown.querySelector("button").addEventListener("click", (e) => {
      e.stopPropagation();
      companyDropdown.classList.toggle("open");
      productsDropdown.classList.remove("open");
    });

    productsDropdown.querySelector("button").addEventListener("click", (e) => {
      e.stopPropagation();
      productsDropdown.classList.toggle("open");
      companyDropdown.classList.remove("open");
    });

    document.addEventListener("mousedown", (e) => {
      // 바깥 클릭 시 닫기
      if (!companyDropdown.contains(e.target)) companyDropdown.classList.remove("open");
      if (!productsDropdown.contains(e.target)) productsDropdown.classList.remove("open");
    });

    // ----------------------------
    // Contact form submit (React handleSubmit 대체)
    // ----------------------------
    const contactForm = document.getElementById("contactForm");
    const emailInput = document.getElementById("emailInput");
    const messageInput = document.getElementById("messageInput");

    contactForm.addEventListener("submit", (e) => {
      e.preventDefault();
      const payload = {
        email: emailInput.value.trim(),
        message: messageInput.value.trim()
      };
      console.log("Form submitted:", payload);
      alert("Thank you for your message! We'll get back to you soon.");
      emailInput.value = "";
      messageInput.value = "";
    });

    // ----------------------------
    // Footer year
    // ----------------------------
    document.getElementById("copyright").textContent =
      `© ${new Date().getFullYear()} (주)에스비테크. All rights reserved.`;
  </script>
</body>
</html>
