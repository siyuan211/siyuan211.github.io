---
layout: no-nav
title: 联系我们
permalink: /contact/
---

<div class="contact-container">
  <h1>📬 联系我们</h1>

  <form name="contact" method="POST" data-netlify="true">
    <label for="name">姓名：</label>
    <input type="text" id="name" name="name" required />

    <label for="email">邮箱：</label>
    <input type="email" id="email" name="email" required />

    <label for="message">留言内容：</label>
    <textarea id="message" name="message" rows="5" required></textarea>

    <button type="submit">提交</button>
  </form>

  <p class="note">✅ 提交后，我们会收到你的留言。</p>
</div>