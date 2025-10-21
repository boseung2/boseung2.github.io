---
# Use the Intro widget of the Blog template
widget: about.avatar

# This file represents a page section.
headless: true

# Order that this section will appear in.
weight: 10

author: admin
#design:
#  background:
#    color: '#090a0b'
#    text_color_light: true
#    video:
#      path:  # enter filename of a video in /assets/media
#  css_class: fullscreen
---

👋 전북대학교 컴퓨터인공지능학부 정보승입니다.
{style="font-size: 1.2rem; background: #FFB76B; background: linear-gradient(to right, #FFB76B 0%, #FFA73D 30%, #FF7C00 60%, #FF7F04 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent;"}

Check out my [resumé](/about/) and portfolio below 😍

---

<!-- ✅ 3단 자동 사진 슬라이더 -->
<div class="home-slider">
  <div class="slides">
    <img src="/media/slider1.png" alt="Slider 1">
    <img src="/media/slider2.png" alt="Slider 2">
    <img src="/media/slider3.png" alt="Slider 3">
  </div>
</div>

<!-- ✅ 전북대학교 지도 (Google Maps Embed) -->
<div class="home-map">
  <iframe
    title="Jeonbuk National University Map"
    src="https://www.openstreetmap.org/export/embed.html?bbox=127.12%2C35.84%2C127.14%2C35.86&layer=mapnik&marker=35.85%2C127.13"
    width="100%"
    height="420"
    style="border:0;"
    loading="lazy"
    referrerpolicy="no-referrer-when-downgrade">
  </iframe>
</div>

<style>
/* ----- Slider Styles ----- */
.home-slider {
  position: relative;
  max-width: 100%;
  margin: 1.5rem 0 2rem;
  overflow: hidden;
  border-radius: 12px;
}

.home-slider .slides {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 8px;
  animation: slideFade 12s infinite;
}

.home-slider img {
  width: 100%;
  height: 260px;
  object-fit: cover;
  display: block;
  border-radius: 10px;
}

/* 3장 슬라이드를 페이드로 자동 전환 */
@keyframes slideFade {
  0%, 27%   { opacity: 1; }
  33%, 60%  { opacity: 1; }
  66%, 93%  { opacity: 1; }
  100%      { opacity: 1; }
}

/* Hover 시 일시정지 (선택) */
.home-slider:hover .slides {
  animation-play-state: paused;
}

/* 반응형 높이 조정 */
@media (min-width: 768px) {
  .home-slider img { height: 300px; }
}
@media (min-width: 1200px) {
  .home-slider img { height: 360px; }
}

/* ----- Map Styles ----- */
.home-map {
  margin-top: 1rem;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 6px 20px rgba(0,0,0,0.08);
}
</style>

<!-- 🔧 사용법 안내:
1) /assets/media/ 폴더에 slider1.jpg, slider2.jpg, slider3.jpg 파일을 추가하세요.
2) 이미지 경로/파일명은 자유롭게 변경 가능합니다.
3) 지도는 Google Maps embed를 사용합니다. OpenStreetMap 등을 쓰려면 iframe src를 바꾸세요.
-->
