---
title: 배터리 설치
author: 박민서
date: 2026-01-26
category: 배터리 설치
layout: post
mermaid: true
---

<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>배터리 설치 - 박민서 블로그</title>
  <style>
    body {
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      margin: 0;
      padding: 20px;
      background-color: #f5f5f5;
      color: #333;
    }
    .container {
      max-width: 800px;
      margin: 0 auto;
      background-color: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    h1 {
      color: #2c3e50;
      text-align: center;
      border-bottom: 2px solid #3498db;
      padding-bottom: 10px;
    }
    .meta-info {
      text-align: center;
      color: #7f8c8d;
      margin-bottom: 30px;
      font-size: 0.9em;
    }

    :root {
      --gallery-ratio: 4 / 3;
      --img-radius: 10px;

      /* ✅ 연락처(내사진/명함) 행 높이: 여기만 바꾸면 크기 조절 */
      --contact-row-h: 170px;
    }

    /* =========================
       갤러리
    ========================= */
    .photo-gallery {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 15px;
      margin: 30px 0;
    }
    .photo-item img {
      width: 100%;
      aspect-ratio: var(--gallery-ratio);
      object-fit: cover;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      background: #fff;
      display: block;
    }
    .photo-caption {
      margin-top: 8px;
      font-size: 0.85em;
      color: #7f8c8d;
      text-align: center;
    }
    .photo-item.full-width {
      grid-column: 1 / -1;
    }
    .photo-item.full-width img {
      aspect-ratio: 16 / 9;
    }

    /* =========================
       담당자/연락처 섹션
       ✅ 핵심: 가로 1:3, 높이 고정
    ========================= */
    .contact-section {
      margin-top: 40px;
      padding: 26px;
      border: 1px solid #e5e7eb;
      border-radius: 14px;
      background: #fafafa;
    }
    .contact-title {
      font-weight: 700;
      color: #2c3e50;
      margin-bottom: 16px;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 3fr; /* ✅ 무조건 1:3 */
      gap: 18px;
      align-items: stretch;
    }

    .card-box {
      border: 1px dashed #cbd5e1;
      border-radius: 14px;
      background: #fff;

      height: var(--contact-row-h); /* ✅ 두 박스 높이 동일 */
      padding: 12px;
      box-sizing: border-box;

      display: block;  /* flex 제거 */
      min-height: 0;   /* ✅ 기존 min-height 영향 제거 */
    }

    .profile-photo,
    .business-card-img {
      width: 100%;
      height: 100%; /* ✅ card-box 높이를 그대로 사용 */
      border-radius: var(--img-radius);
      overflow: hidden;
      border: 1px solid #e5e7eb;
      background: #fff;
      box-sizing: border-box;
    }

    /* 내 사진: 꽉 차게 */
    .profile-photo img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
    }

    /* 명함: 전체가 다 보이게 */
    .business-card-img {
      cursor: zoom-in;
    }
    .business-card-img img {
      width: 100%;
      height: 100%;
      object-fit: contain;
      padding: 10px;
      background: #fff;
      display: block;
      box-sizing: border-box;
    }

    /* =========================
       라이트박스
    ========================= */
    .lightbox {
      position: fixed;
      inset: 0;
      background: rgba(0, 0, 0, 0.65);
      display: none;
      align-items: center;
      justify-content: center;
      z-index: 9999;
      padding: 20px;
    }
    .lightbox.open {
      display: flex;
    }
    .lightbox-content {
      max-width: 960px;
      width: 96vw;
      background: #fff;
      border-radius: 14px;
      overflow: hidden;
      position: relative;
    }
    .lightbox-content img {
      width: 100%;
      display: block;
    }
    .lightbox-close {
      position: absolute;
      top: 10px;
      right: 10px;
      background: rgba(0, 0, 0, 0.6);
      color: #fff;
      border: none;
      width: 36px;
      height: 36px;
      border-radius: 50%;
      cursor: pointer;
      font-size: 18px;
    }

    .footer {
      text-align: center;
      margin-top: 30px;
      padding-top: 20px;
      border-top: 1px solid #eee;
      color: #95a5a6;
      font-size: 0.8em;
    }

    /* =========================
       반응형
    ========================= */
    @media (max-width: 600px) {
      .photo-gallery {
        grid-template-columns: 1fr;
      }

      /* 모바일은 세로로 쌓기 */
      .contact-grid {
        grid-template-columns: 1fr;
      }

      /* 모바일에서 보기 좋게 높이 조정 */
      .card-box {
        height: 200px;
      }
    }
  </style>
</head>

<body>
  <div class="container">
    <h1>[설치 인증] [서울]에서 안전하게 블로그 설치 완료!</h1>

    <div class="meta-info">
      작성일: 2026년 1월 25일<br />
      블로그명: [당신의 블로그 이름]
    </div>

    <p style="text-align:center;">
      <strong>배터리 설치 과정 사진</strong>
    </p>

    <div class="photo-gallery">
      <div class="photo-item">
        <img src="https://bf.sbgpt.ddns.net/download/d4ae7786-e2f8-40ae-a33d-d083210d4091_KakaoTalk_20200507_140003536_04.jpg" alt="배터리 설치 준비 사진">
        <div class="photo-caption">배터리 설치 준비 사진</div>
      </div>

      <div class="photo-item">
        <img src="https://bf.sbgpt.ddns.net/download/62a7cd7a-0dc2-4834-9af9-99e88ca8e067_KakaoTalk_20200507_140003536_01.jpg" alt="배터리 철거 후 사진">
        <div class="photo-caption">배터리 철거 후 사진</div>
      </div>

      <div class="photo-item">
        <img src="https://bf.sbgpt.ddns.net/download/816ed9c5-4667-4ec6-a819-db6a42227b8e_KakaoTalk_20200507_140003536_06.jpg" alt="배터리 설치 후 사진">
        <div class="photo-caption">배터리 설치 후 사진</div>
      </div>

      <div class="photo-item">
        <img src="https://bf.sbgpt.ddns.net/download/b9720d39-07fe-4739-b52f-33724209f96f_KakaoTalk_20200507_140003536_07.jpg" alt="배터리 전압 체크 사진">
        <div class="photo-caption">배터리 전압 체크 사진</div>
      </div>

      <div class="photo-item full-width">
        <img src="https://bf.sbgpt.ddns.net/download/08d4e1b7-1028-44d5-926b-733e3984da2d_KakaoTalk_20200507_140003536_06.jpg" alt="설치 위치 장소 사진">
        <div class="photo-caption">설치 위치 장소 사진</div>
      </div>
    </div>

    <div class="contact-section">
      <p class="contact-title">담당자 / 연락처</p>

      <div class="contact-grid">
        <!-- ✅ 내 사진 (왼쪽 1) -->
        <div class="card-box">
          <div class="profile-photo">
            <img src="https://bf.sbgpt.ddns.net/download/cc0a031b-abf6-4d5a-b031-cd76e3f2ffb4_minseo.png" alt="프로필 사진" />
          </div>
        </div>

        <!-- ✅ 명함 (오른쪽 3) -->
        <div class="card-box">
          <div class="business-card-img"
               data-full="https://bf.sbgpt.ddns.net/download/ada2f78c-5766-47fb-8d41-d2979193ffca_minseo1.jpg">
            <img src="https://bf.sbgpt.ddns.net/download/ada2f78c-5766-47fb-8d41-d2979193ffca_minseo1.jpg" alt="명함 이미지" />
          </div>
        </div>
      </div>
    </div>

    <div class="footer">
      본 글은 2026년 1월 25일 진행된 UPS 배터리 설치 작업을 기반으로 작성되었습니다.
    </div>
  </div>

  <!-- 라이트박스 -->
  <div class="lightbox" id="lightbox">
    <div class="lightbox-content">
      <button class="lightbox-close" id="close">×</button>
      <img id="lightboxImg" alt="명함 확대" />
    </div>
  </div>

  <script>
    const lb = document.getElementById("lightbox");
    const lbImg = document.getElementById("lightboxImg");
    const close = document.getElementById("close");

    document.querySelectorAll(".business-card-img").forEach((el) => {
      el.onclick = () => {
        lbImg.src = el.dataset.full;
        lb.classList.add("open");
        document.body.style.overflow = "hidden";
      };
    });

    close.onclick = () => {
      lb.classList.remove("open");
      document.body.style.overflow = "";
    };

    lb.onclick = (e) => {
      if (e.target === lb) close.onclick();
    };
  </script>
</body>
</html>