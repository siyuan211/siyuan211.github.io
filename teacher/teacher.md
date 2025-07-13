---
permalink: /teacher/
title: 老师
layout: archive
---

<style>
.teacher-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.teacher-card {
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 12px;
  padding: 1rem;
  box-shadow: 0 0 12px rgba(0, 0, 0, 0.4);
  text-align: center;
  color: #fff;
  backdrop-filter: blur(8px);
  transition: transform 0.3s ease;
}

.teacher-card:hover {
  transform: translateY(-5px);
}

.teacher-card img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  margin-bottom: 0.8rem;
}

.teacher-name {
  font-size: 1.3rem;
  font-weight: bold;
  margin-bottom: 0.4rem;
}

.teacher-intro {
  font-size: 1rem;
  line-height: 1.6;
}
</style>

## 👩‍🏫 我们的老师

<div class="teacher-gallery">

  <div class="teacher-card">
    <img src="https://你的图床链接1.jpg" alt="张老师">
    <div class="teacher-name">张老师</div>
    <div class="teacher-intro">负责数学教学，亲和力强，善于启发学生思维。</div>
  </div>

  <div class="teacher-card">
    <img src="https://你的图床链接2.jpg" alt="李老师">
    <div class="teacher-name">李老师</div>
    <div class="teacher-intro">语文教学一把好手，讲课风趣生动，擅长写作指导。</div>
  </div>

  <div class="teacher-card">
    <img src="https://你的图床链接3.jpg" alt="王老师">
    <div class="teacher-name">王老师</div>
    <div class="teacher-intro">严中有爱，教学有方，带领我们征服物理难题。</div>
  </div>

  <!-- 继续添加更多老师 -->
  
</div>
