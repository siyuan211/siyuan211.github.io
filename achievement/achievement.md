---
layout: no-nav
permalink: /achievement/
title: 我们的成就
---

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