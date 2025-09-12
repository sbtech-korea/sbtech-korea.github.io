---
title: Contact
author: 박민서
date: 2022-02-05
category: Jekyll
layout: post
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
    <div class="max-w-4xl mx-auto p-6 space-y-8">
  <div class="text-3xl font-bold text-primary">연락처</div>
  
  <div class="space-y-4">
    <div class="flex items-center space-x-4">
      <img aria-hidden="true" alt="company" src="https://batteryfriendserverapi.com/openui/24x24.svg?text=🏢" />
      <div class="text-lg">
        <p class="text-foreground font-medium">회사명: (주)에스비테크</p>
        <p class="text-muted-foreground">주소: 경기도 김포시 금포로 1517(운양동)</p>
      </div>
    </div>
    <div class="flex items-center space-x-4">
      <img aria-hidden="true" alt="business-number" src="https://batteryfriendserverapi.com/openui/24x24.svg?text=📄" />
      <div class="text-lg">
        <p class="text-foreground font-medium">사업자번호: 137-86-31906</p>
        <p class="text-muted-foreground">대표자: 박승태</p>
      </div>
    </div>
    <div class="flex items-center space-x-4">
      <img aria-hidden="true" alt="phone" src="https://batteryfriendserverapi.com/openui/24x24.svg?text=📞" />
      <div class="text-lg">
        <p class="text-foreground font-medium">전화: 031-985-7315</p>
        <p class="text-muted-foreground">팩스: 031-985-1661</p>
      </div>
    </div>
    <div class="flex items-center space-x-4">
      <img aria-hidden="true" alt="email" src="https://batteryfriendserverapi.com/openui/24x24.svg?text=📧" />
      <div class="text-lg">
        <p class="text-foreground font-medium">이메일: pst1001@naver.com</p>
      </div>
    </div>
  </div>
  
  <div class="relative w-full h-64 rounded-lg overflow-hidden">
    <img
      src="https://batteryfriendserverapi.com/openui/600x400.svg?text=회사%20사진"
      alt="회사 사진"
      class="w-full h-full object-cover"
    />
  </div>
  
  <div class="bg-card p-6 rounded-lg shadow-md">
    <h2 class="text-2xl font-semibold text-foreground mb-4">문의하기</h2>
    <form class="space-y-4">
      <div>
        <label for="name" class="block text-sm font-medium text-foreground">이름</label>
        <input
          type="text"
          id="name"
          name="name"
          required
          class="mt-1 block w-full px-3 py-2 bg-input border border-border rounded-md shadow-sm focus:outline-none focus:ring-2 focus:ring-ring focus:border-ring"
          placeholder="이름을 입력해주세요"
        />
      </div>
      <div>
        <label for="email" class="block text-sm font-medium text-foreground">이메일</label>
        <input
          type="email"
          id="email"
          name="email"
          required
          class="mt-1 block w-full px-3 py-2 bg-input border border-border rounded-md shadow-sm focus:outline-none focus:ring-2 focus:ring-ring focus:border-ring"
          placeholder="이메일을 입력해주세요"
        />
      </div>
      <div>
        <label for="message" class="block text-sm font-medium text-foreground">문의 내용</label>
        <textarea
          id="message"
          name="message"
          required
          rows="4"
          class="mt-1 block w-full px-3 py-2 bg-input border border-border rounded-md shadow-sm focus:outline-none focus:ring-2 focus:ring-ring focus:border-ring"
          placeholder="문의사항을 입력해주세요"
        ></textarea>
      </div>
      <button
        type="submit"
        class="px-4 py-2 bg-primary text-primary-foreground rounded-md hover:bg-primary/90 focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 transition-colors"
      >
        보내기
      </button>
    </form>
  </div>
  <div class="text-sm text-muted-foreground mt-4">
    COPYRIGHT(c) 2020 (주)에스비테크 ALL RIGHTS RESERVED.
  </div>
</div>


  </body>
</html>
