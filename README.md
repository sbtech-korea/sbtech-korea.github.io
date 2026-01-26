---
layout: home
title: (주) 에스비테크
permalink: /
cover: https://sbtech-korea.github.io/assets/main.jpg
---

<!DOCTYPE html>
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
      font-weight: 800;
      color: #1e40af;
    }
    .info-item h4{ margin:0 0 4px 0; font-size: 14px; }
    .info-item p{ margin:0; color: var(--gray600); font-size: 14px; line-height: 1.5; }

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
        <a class="btn btn-primary btn-lg" href="#support">상담 문의하기</a>
        <a class="btn btn-outline btn-lg" href="#catalog">카탈로그 보기</a>
      </div>
    </div>
  </section>

  <!-- Company Info -->
  <section class="section-white">
    <div class="container">
      <div class="center" style="margin-bottom: 52px;">
        <h2 style="margin:0 0 10px 0; font-size: 34px;">(주) 에스비테크</h2>
        <p class="lead" style="margin-bottom:0;">기준과 원칙으로 답하는 배터리 전문기업</p>
      </div>

      <div class="grid-2">
        <div class="placeholder">Company Image</div>

        <div>
          <h3 style="margin:0 0 12px 0; font-size: 26px;">산업용/자동차용 배터리 전문기업</h3>
          <p style="color:var(--gray700); line-height:1.8; margin:0 0 12px 0;">
            ※ 델코 전국 판매1위<br />
            ※ X-Pro 전국판매 1위<br />
            ※ GM 순정배터리 전국총판<br />
            ※ 쌍용자동차 순정배터리 전국총판<br />
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
            차량 모델 및 규격에 맞춘 정확한 호환 확인을 기반으로,
            안정적인 시동 성능과 전장 시스템 보호를 돕습니다.
          </p>
          <p>특징:</p>
          <ul>
            <li>차종/연식/규격 기반 호환 확인</li>
            <li>설치 후 전압/충전 상태 점검</li>
            <li>안정적인 전력 공급</li>
            <li>정품/출처 명확</li>
            <li>사후관리 기준 안내</li>
          </ul>
          <p>
            과한 권유보다 필요한 사양을 정확히 안내드리며,
            설치 후 점검까지 책임집니다.
          </p>
        </div>

        <div class="detail-box detail-green">
          <h3>산업용 배터리</h3>
          <p>
            산업 현장 및 UPS 환경에 맞춰 용량·방전특성·운용 조건을 고려해
            안정적인 백업 전원을 제공합니다.
          </p>
          <p>특징:</p>
          <ul>
            <li>UPS/시설 환경 맞춤 제안</li>
            <li>장시간 운용에 적합한 구성</li>
            <li>저온/부하 환경 고려</li>
            <li>고신뢰성 설계</li>
            <li>점검/교체 주기 안내</li>
          </ul>
          <p>
            공장 자동화, 저장 시스템, 재생 에너지 저장 등
            다양한 산업 분야에 안정적인 전력 공급을 지원합니다.
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
        <p class="lead" style="margin-bottom:0;">상담이 필요하시면 연락처 또는 문의폼을 이용해 주세요.</p>
      </div>

      <div class="support-grid">
        <div>
          <h3 style="margin:0 0 18px 0; font-size: 24px;">연락처 정보</h3>

          <div style="display:flex; flex-direction:column; gap:14px;">
            <div class="info-item">
              <div class="icon-box">📍</div>
              <div>
                <h4>주소</h4>
                <p>경기도 김포시 금포로 1517(운양동)</p>
              </div>
            </div>

            <div class="info-item">
              <div class="icon-box">🧾</div>
              <div>
                <h4>사업자 정보</h4>
                <p>사업자번호: 137-86-31906<br />대표자: 박승태</p>
              </div>
            </div>

            <div class="info-item">
              <div class="icon-box">☎</div>
              <div>
                <h4>전화 / 팩스</h4>
                <p>TEL: 031-985-7315<br />FAX: 031-985-1661</p>
              </div>
            </div>

            <div class="info-item">
              <div class="icon-box">✉</div>
              <div>
                <h4>이메일</h4>
                <p><a href="mailto:pst1001@naver.com" style="text-decoration:underline; color: var(--blue);">pst1001@naver.com</a></p>
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
          <p style="margin:10px 0 0; color: var(--gray600); font-size: 13px; line-height:1.5;">
            ※ 문의 내용 확인 후 순차적으로 연락드립니다.
          </p>
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
          <p class="muted" style="margin:0;">
            기준과 원칙으로 답하는 배터리 전문기업
          </p>
        </div>

        <div>
          <div class="footer-title">빠른 링크</div>
          <ul class="footer-links">
            <li><a href="#introduction">회사소개</a></li>
            <li><a href="#products">제품개요</a></li>
            <li><a href="#catalog">제품카다로그</a></li>
            <li><a href="#gallery">설치갤러리</a></li>
            <li><a href="#support">고객센터</a></li>
          </ul>
        </div>

        <div>
          <div class="footer-title">취급 분야</div>
          <ul class="footer-links">
            <li class="muted">차량용 배터리</li>
            <li class="muted">산업용 배터리</li>
            <li class="muted">UPS 배터리</li>
            <li class="muted">설치 및 공급</li>
          </ul>
        </div>

        <div>
          <div class="footer-title">연락처 정보</div>
          <ul class="footer-links">
            <li class="muted">주소: 경기도 김포시 금포로 1517(운양동)</li>
            <li class="muted">사업자번호: 137-86-31906</li>
            <li class="muted">대표자: 박승태</li>
            <li class="muted">TEL: 031-985-7315</li>
            <li class="muted">FAX: 031-985-1661</li>
            <li class="muted">E-mail: <a href="mailto:pst1001@naver.com" style="text-decoration:underline;">pst1001@naver.com</a></li>
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
        description: "차량용/산업용 전 라인업 취급. 규격 확인 후 정확한 사양으로 안내드립니다.",
        image: "delco-battery.jpg"
      },
      {
        id: 2,
        name: "로케트 배터리",
        description: "산업 현장 및 장비 환경에 맞춘 배터리 솔루션을 제공합니다.",
        image: "rocket-battery.jpg"
      },
      {
        id: 3,
        name: "아트라스 배터리",
        description: "다양한 운용 조건을 고려한 안정적인 전력 공급을 지원합니다.",
        image: "atlas-battery.jpg"
      },
      {
        id: 4,
        name: "엑스프로 배터리",
        description: "용도/부하 조건에 맞춰 성능과 안정성을 균형 있게 제안합니다.",
        image: "xpro-battery.jpg"
      },
      {
        id: 5,
        name: "솔라이트 배터리",
        description: "검증된 제품과 표준 절차로 설치부터 사후관리까지 책임집니다.",
        image: "solight-battery.jpg"
      }
    ];

    // ----------------------------
    // Render batteries cards
    // ----------------------------
    const batteryGrid = document.getElementById("batteryGrid");
    if (batteryGrid) {
      batteryGrid.innerHTML = batteries.map(b => `
        <div class="card">
          <div class="card-img">Battery Image</div>
          <div class="card-body">
            <h3 class="card-title">${b.name}</h3>
            <p class="card-desc">${b.description}</p>
          </div>
        </div>
      `).join("");
    }

    // ----------------------------
    // Gallery marquee (1~10 두 번)
    // ----------------------------
    const galleryMarquee = document.getElementById("galleryMarquee");
    if (galleryMarquee) {
      const items = Array.from({length: 10}, (_, i) => i + 1);
      const renderGalleryItem = (n) => `
        <a href="/gallery/${n}" aria-label="설치 갤러리 ${n}">
          <div class="gallery-card">
            <div class="gallery-img">설치 이미지 ${n}</div>
            <div class="gallery-body">
              <h3>설치 ${n}</h3>
              <p>설치 사례 설명이 여기에 표시됩니다</p>
            </div>
          </div>
        </a>
      `;
      galleryMarquee.innerHTML =
        items.map(n => renderGalleryItem(n)).join("") +
        items.map(n => renderGalleryItem(n)).join("");
    }

    // ----------------------------
    // Contact form submit
    // ----------------------------
    const contactForm = document.getElementById("contactForm");
    const emailInput = document.getElementById("emailInput");
    const messageInput = document.getElementById("messageInput");

    if (contactForm && emailInput && messageInput) {
      contactForm.addEventListener("submit", (e) => {
        e.preventDefault();
        const payload = {
          email: emailInput.value.trim(),
          message: messageInput.value.trim()
        };
        console.log("Form submitted:", payload);
        alert("문의가 접수되었습니다. 확인 후 빠르게 연락드리겠습니다.");
        emailInput.value = "";
        messageInput.value = "";
      });
    }

    // ----------------------------
    // Footer year
    // ----------------------------
    const c = document.getElementById("copyright");
    if (c) {
      c.textContent = `© ${new Date().getFullYear()} (주)에스비테크. All rights reserved.`;
    }
  </script>
</body>
</html>

