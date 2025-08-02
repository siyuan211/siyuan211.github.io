---
layout: no-nav
permalink: /achievement/
title: 我们的成就
---

<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <title>{{ page.title }}</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    /* 页面整体背景和字体 */
    body {
      margin: 0;
      padding: 2rem 1rem;
      background: #121212;
      font-family: -apple-system, BlinkMacSystemFont, "Helvetica Neue", "PingFang SC", "Microsoft YaHei", sans-serif;
      color: #eee;
      min-height: 100vh;
      line-height: 1.6;
    }

    h1, h2 {
      text-align: center;
      color: #00bfff;
      margin-bottom: 1rem;
      font-weight: 700;
    }

    p {
      max-width: 720px;
      margin: 0.5rem auto 1.5rem;
      font-size: 1rem;
      color: #ccc;
    }

    /* fade-in动画初始样式 */
    .fade-in {
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.7s ease-out, transform 0.7s ease-out;
      will-change: opacity, transform;
      margin-bottom: 2rem;
      max-width: 720px;
      margin-left: auto;
      margin-right: auto;
    }

    /* 动画触发后 */
    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* 图片基本样式 */
    .fade-in img {
      max-width: 100%;
      border-radius: 8px;
      margin-top: 1rem;
      box-shadow: 0 4px 12px rgba(0,0,0,0.6);
      display: block;
      margin-left: auto;
      margin-right: auto;
    }

    /* 图集布局 */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill,minmax(150px,1fr));
      gap: 1rem;
      margin-top: 1rem;
      max-width: 720px;
      margin-left: auto;
      margin-right: auto;
    }

    .gallery img {
      width: 100%;
      height: auto;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 16px rgba(0,0,0,0.8);
    }

  </style>
</head>
<body>
  <h1>{{ page.title }}</h1>

  <h2>2025年奖项</h2>

  <div class="fade-in">
    <img src="https://s21.ax1x.com/2025/07/10/pVQTbdO.jpg" alt="五一歌唱比赛" />
    <p>这是2025年八年级下学期举行的五一歌咏比赛，我们获得了特等奖，祝贺！</p>
  </div>

  <div class="fade-in">
    <img src="https://s21.ax1x.com/2025/07/13/pVlIJvq.jpg" alt="值周活动1" />
    <img src="https://s21.ax1x.com/2025/07/13/pVlItK0.jpg" alt="值周活动2" />
    <p>这是2025年八年级下期的值周活动，以上是👩‍❤️‍💋‍👨</p>
  </div>

  <div class="fade-in">
    <img src="https://s21.ax1x.com/2025/07/13/pVlINrV.jpg" alt="外出活动" />
    <p>玩的真是很开心😁</p>
  </div>

  <h2>周年校庆图集 🎉</h2>
  <p style="max-width:720px;margin:auto 0 1.5rem;">以下是我们在周年校庆活动中的精彩照片：</p>

  <div class="gallery fade-in">
    <img src="https://s21.ax1x.com/2025/07/13/pVlIdVU.jpg" alt="活动照1" />
    <img src="https://s21.ax1x.com/2025/07/13/pVlI054.jpg" alt="活动照2" />
    <img src="https://s21.ax1x.com/2025/07/13/pVlIUbT.jpg" alt="活动照3" />
    <img src="https://s21.ax1x.com/2025/07/13/pVlIwaF.jpg" alt="活动照4" />
  </div>

  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const fadeEls = document.querySelectorAll('.fade-in');
      const observer = new IntersectionObserver(entries => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            observer.unobserve(entry.target);
          }
        });
      }, { threshold: 0.1 });

      fadeEls.forEach(el => observer.observe(el));
    });
  </script>
</body>
</html>