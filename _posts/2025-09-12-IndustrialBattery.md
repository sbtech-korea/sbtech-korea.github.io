---
title: 산업용 배터리
author: 박민서
date: 2025-08-22
category: 산업용 배터리
layout: post
mermaid: true
---

<hr>


# 설치 사진

<hr>

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
    <div class="min-h-screen bg-background text-foreground flex flex-col">
  <main class="flex-grow p-6">
    <section class="mb-8">
      <h2 class="text-xl font-semibold mb-4">Featured Images</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Featured Image 1" src="https://picsum.photos/400/300?random=1" class="w-full h-48 object-cover" />
          <div class="p-4">
            <h3 class="text-lg font-medium mb-2">Image Title 1</h3>
            <p class="text-muted-foreground">A beautiful landscape captured in the morning light.</p>
          </div>
        </div>
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Featured Image 2" src="https://picsum.photos/400/300?random=2" class="w-full h-48 object-cover" />
          <div class="p-4">
            <h3 class="text-lg font-medium mb-2">Image Title 2</h3>
            <p class="text-muted-foreground">A vibrant cityscape at sunset.</p>
          </div>
        </div>
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Featured Image 3" src="https://picsum.photos/400/300?random=3" class="w-full h-48 object-cover" />
          <div class="p-4">
            <h3 class="text-lg font-medium mb-2">Image Title 3</h3>
            <p class="text-muted-foreground">A serene beach with clear blue waters.</p>
          </div>
        </div>
      </div>
    </section>
    <section class="mb-8">
      <h2 class="text-xl font-semibold mb-4">Recent Uploads</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-4">
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Recent Image 1" src="https://picsum.photos/300/200?random=4" class="w-full h-32 object-cover" />
          <div class="p-2">
            <p class="text-muted-foreground">Recent Image 1</p>
          </div>
        </div>
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Recent Image 2" src="https://picsum.photos/300/200?random=5" class="w-full h-32 object-cover" />
          <div class="p-2">
            <p class="text-muted-foreground">Recent Image 2</p>
          </div>
        </div>
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Recent Image 3" src="https://picsum.photos/300/200?random=6" class="w-full h-32 object-cover" />
          <div class="p-2">
            <p class="text-muted-foreground">Recent Image 3</p>
          </div>
        </div>
        <div class="bg-card rounded-lg overflow-hidden shadow">
          <img alt="Recent Image 4" src="https://picsum.photos/300/200?random=7" class="w-full h-32 object-cover" />
          <div class="p-2">
            <p class="text-muted-foreground">Recent Image 4</p>
          </div>
        </div>
      </div>
    </section>
  </main>
  <footer class="p-4 bg-muted text-muted-foreground text-center">
    <p>&copy; 2025 My Gallery. All rights reserved.</p>
  </footer>
  
  <div id="imageModal" class="fixed inset-0 bg-black bg-opacity-75 flex items-center justify-center hidden z-50">
    <div class="bg-card rounded-lg shadow-lg max-w-4xl max-h-4xl overflow-hidden">
      <img id="modalImage" class="w-full h-full object-contain" />
      <button onclick="closeModal()" class="absolute top-2 right-2 bg-destructive text-destructive-foreground px-4 py-2 rounded hover:bg-destructive/80">Close</button>
    </div>
  </div>
</div>

<script>
  function showImage(src, alt) {
    const modal = document.getElementById('imageModal');
    const modalImage = document.getElementById('modalImage');
    modalImage.src = src;
    modalImage.alt = alt;
    modal.classList.remove('hidden');
  }
  function closeModal() {
    document.getElementById('imageModal').classList.add('hidden');
  }
</script>

  </body>
</html>