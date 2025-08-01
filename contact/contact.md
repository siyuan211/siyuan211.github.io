---
layout: none
title: 联系我们
permalink: /contact/
---

<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <title>{{ page.title }}</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    body {
      margin: 0;
      padding: 2rem;
      font-family: "Segoe UI", Roboto, "PingFang SC", sans-serif;
      background: linear-gradient(120deg, #1e3c72, #2a5298);
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .contact-container {
      background: rgba(0, 0, 0, 0.6);
      padding: 2rem 2.5rem;
      border-radius: 16px;
      max-width: 480px;
      width: 100%;
      box-shadow: 0 8px 30px rgba(0,0,0,0.4);
      animation: slideFadeIn 1s ease-out;
    }

    h1 {
      text-align: center;
      margin-bottom: 1.5rem;
      font-size: 2rem;
      color: #f1f1f1;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    label {
      font-weight: 500;
      margin-bottom: 0.3rem;
      display: block;
      color: #d0e7ff;
    }

    input, textarea {
      width: 100%;
      padding: 0.75rem;
      border-radius: 8px;
      border: none;
      font-size: 1rem;
      background: #fff;
      color: #222;
      transition: box-shadow 0.3s ease;
    }

    input:focus, textarea:focus {
      box-shadow: 0 0 8px #00bfff;
      outline: none;
    }

    button {
      background: #00bfff;
      color: white;
      font-size: 1rem;
      border: none;
      padding: 0.8rem;
      border-radius: 10px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    button:hover {
      background: #009acd;
    }

    p.note {
      text-align: center;
      margin-top: 1.2rem;
      font-size: 0.95rem;
      color: #a7dcff;
    }

    @keyframes slideFadeIn {
      0% {
        opacity: 0;
        transform: translateY(30px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @media screen and (max-width: 600px) {
      body {
        padding: 1.5rem;
      }
      .contact-container {
        padding: 1.5rem;
      }
    }
  </style>
</head>
<body>
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
</body>
</html>