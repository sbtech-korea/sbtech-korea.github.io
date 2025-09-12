---
title: 
author: SBTECH
date: 2022-02-04
category: Jekyll
layout: post
cover: https://sbtech-korea.github.io/assets/main.jpg
---

<html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com?plugins=forms,typography"></script>
		<script src="https://unpkg.com/unlazy@0.11.3/dist/unlazy.with-hashing.iife.js" defer init></script>
		<script type="text/javascript">
			window.tailwind.config = {
				darkMode: ['class'],
				theme: {
					extend: {
						colors: {
							border: 'hsl(var(--border))',
							input: 'hsl(var(--input))',
							ring: 'hsl(var(--ring))',
							background: 'hsl(var(--background))',
							foreground: 'hsl(var(--foreground))',
							primary: {
								DEFAULT: 'hsl(var(--primary))',
								foreground: 'hsl(var(--primary-foreground))'
							},
							secondary: {
								DEFAULT: 'hsl(var(--secondary))',
								foreground: 'hsl(var(--secondary-foreground))'
							},
							destructive: {
								DEFAULT: 'hsl(var(--destructive))',
								foreground: 'hsl(var(--destructive-foreground))'
							},
							muted: {
								DEFAULT: 'hsl(var(--muted))',
								foreground: 'hsl(var(--muted-foreground))'
							},
							accent: {
								DEFAULT: 'hsl(var(--accent))',
								foreground: 'hsl(var(--accent-foreground))'
							},
							popover: {
								DEFAULT: 'hsl(var(--popover))',
								foreground: 'hsl(var(--popover-foreground))'
							},
							card: {
								DEFAULT: 'hsl(var(--card))',
								foreground: 'hsl(var(--card-foreground))'
							},
						},
					}
				}
			}
		</script>
		<style type="text/tailwindcss">
			@layer base {
				:root {
					--background: 0 0% 100%;
--foreground: 240 10% 3.9%;
--card: 0 0% 100%;
--card-foreground: 240 10% 3.9%;
--popover: 0 0% 100%;
--popover-foreground: 240 10% 3.9%;
--primary: 240 5.9% 10%;
--primary-foreground: 0 0% 98%;
--secondary: 240 4.8% 95.9%;
--secondary-foreground: 240 5.9% 10%;
--muted: 240 4.8% 95.9%;
--muted-foreground: 240 3.8% 46.1%;
--accent: 240 4.8% 95.9%;
--accent-foreground: 240 5.9% 10%;
--destructive: 0 84.2% 60.2%;
--destructive-foreground: 0 0% 98%;
--border: 240 5.9% 90%;
--input: 240 5.9% 90%;
--ring: 240 5.9% 10%;
--radius: 0.5rem;
				}
				.dark {
					--background: 240 10% 3.9%;
--foreground: 0 0% 98%;
--card: 240 10% 3.9%;
--card-foreground: 0 0% 98%;
--popover: 240 10% 3.9%;
--popover-foreground: 0 0% 98%;
--primary: 0 0% 98%;
--primary-foreground: 240 5.9% 10%;
--secondary: 240 3.7% 15.9%;
--secondary-foreground: 0 0% 98%;
--muted: 240 3.7% 15.9%;
--muted-foreground: 240 5% 64.9%;
--accent: 240 3.7% 15.9%;
--accent-foreground: 0 0% 98%;
--destructive: 0 62.8% 30.6%;
--destructive-foreground: 0 0% 98%;
--border: 240 3.7% 15.9%;
--input: 240 3.7% 15.9%;
--ring: 240 4.9% 83.9%;
				}
			}
		</style>
  </head>
  <body>
    <div class="max-w-6xl mx-auto p-6 space-y-8">
  <div class="text-center">
    <h1 class="text-4xl font-bold text-foreground mb-2">에스비테크</h1>
    <p class="text-lg text-muted-foreground">배터리 O2O 유통플랫폼 전문기업</p>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">회사 개요</h2>
    <p class="text-muted-foreground mb-2">
      (주)에스비테크는 배터리 유통에서 유지관리 및 AS까지 종합적인 토탈서비스를 제공하며,
      다양한 분야의 경험과 노하우를 통해 브랜드의 가치를 극대화하는 O2O 유통플랫폼 전문기업입니다.
    </p>
    <p class="text-muted-foreground">
      경쟁력 있는 제품과 서비스로 다양한 분야에서 제휴를 통해 안정적인 제품 공급과 현장 설치 AS 등
     을 제공함으로써 본연의 기업 정신을 지키고 있습니다.
    </p>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">회사 정보</h2>
    <ul class="space-y-2 text-muted-foreground">
      <li><strong>회사명:</strong> (주)에스비테크</li>
      <li><strong>대표이사:</strong> 박승태</li>
      <li><strong>등록번호:</strong> 137-86-31906</li>
      <li><strong>주소:</strong> 경기도 김포시 금포로 1517 (운양동)</li>
      <li><strong>서비스:</strong> 축전지, 배터리 판매 및 유통</li>
    </ul>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">사업 현황</h2>
    <ul class="space-y-2 text-muted-foreground">
      <li>델코 전국 판매 1위</li>
      <li>X-Pro 전국 판매 1위</li>
      <li>GM 순정배터리 전국 총판 업체</li>
      <li>쌍용자동차 순정배터리 전국 총판 업체</li>
      <li>아트라스 배터리 산업용 판매 우수 업체</li>
      <li>승용차, 화물차, 중장비, 산업용, 농기계, 선박용, 비상발전용 배터리 유통</li>
    </ul>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">회사 신념</h2>
    <ul class="space-y-2 text-muted-foreground">
      <li>고객과 소통하며 최고라는 신념을 지키고 있습니다.</li>
      <li>정직하게 영업하며 다양한 제휴를 통해 고객 만족을 실천합니다.</li>
      <li>철저한 AS로 정확한 업무 처리를 실천합니다.</li>
      <li>15년 무사고 서비스를 제공하며 온라인 원격 지원 서비스를 개발했습니다.</li>
      <li>정기적인 무상 관리 서비스를 통해 신뢰를 쌓고 있습니다.</li>
    </ul>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">우수한 제품</h2>
    <ul class="space-y-2 text-muted-foreground">
      <li>델코 전국 판매 1위이며, 14년 연속 품질 부문 1위 수상</li>
      <li>X-Pro 전국 판매 1위</li>
      <li>국내용으로 개발한 프리미엄급 고성능 자동차 배터리</li>
      <li>아트라스 배터리 산업용 판매 우수 업체</li>
      <li>UPS, 수배전설비 및 기계장치류 등 다양한 분야에 적용 가능한 경제적인 배터리</li>
    </ul>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">제휴 및 협력</h2>
    <ul class="space-y-2 text-muted-foreground">
      <li>GM 순정배터리 전국 총판 업체</li>
      <li>쌍용자동차 순정배터리 전국 총판 업체</li>
      <li>배터리와 관련된 지속된 학습과 트랜드 연구</li>
      <li>거래처의 의견 수렴 및 반영</li>
    </ul>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm">
    <h2 class="text-2xl font-semibold text-foreground mb-4">에스비테크의 기업문화</h2>
    <p class="text-muted-foreground mb-2">
      에스비테크는 판매보다 A/S를 더 중요시하는 기업 문화를 가지고 있으며,
      고객의 신뢰를 바탕으로 한 서비스를 제공합니다.
    </p>
    <p class="text-muted-foreground">
      다양한 분야의 고객과 파트너들과의 협력을 통해 지속적인 성장과 발전을 추구하고 있습니다.
    </p>
  </div>
  <div class="bg-card p-6 rounded-lg shadow-sm text-center">
    <p class="text-muted-foreground">에스비테크는 고객과 함께 성장하는 기업입니다.</p>
  </div>
</div>
  </body>
</html>

