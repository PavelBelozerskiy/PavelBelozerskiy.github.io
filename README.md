# PavelBelozerskiy.github.io
Сайт визитка HTML, CSS
[style.css](https://github.com/user-attachments/files/23327566/style.css)
:root {
  --bg: #0b0f19;
  --accent: #4ade80;
  --text: #f1f5f9;
  --muted: #94a3b8;
  --card: #111827;
  --border: rgba(255,255,255,0.1);
}
* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Inter', sans-serif;
  line-height: 1.6;
}
header {
  background: rgba(17,24,39,0.9);
  position: fixed;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;[index.html](https://github.com/user-attachments/files/23327568/index.html)<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Павел Белозерский — QA Engineer</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Павел Белозерский</h1>
    <nav>
      <a href="#about">Обо мне</a>
      <a href="#skills">Навыки</a>
      <a href="#projects">Проекты</a>
      <a href="#contact">Контакты</a>
    </nav>
  </header>

  <section class="hero">
    <img src="images/profile.jpg" alt="Павел Белозерский">
    <h2>QA Engineer с опытом 3 года</h2>
    <p>Тестирую, автоматизирую и помогаю продуктам становиться лучше.</p>
  </section>

  <section id="about" class="about">
    <h3>Обо мне</h3>
    <p>Я QA инженер с 3-летним опытом работы в сфере тестирования веб и мобильных приложений. Специализируюсь на ручном и автоматизированном тестировании, CI/CD интеграции и улучшении процессов качества. Люблю анализировать сложные сценарии, находить тонкие баги и делать продукт стабильнее.</p>
  </section>

  <section id="skills" class="skills">
    <h3>Навыки</h3>
    <div class="skills-list">
      <div class="skill">Selenium / Playwright</div>
      <div class="skill">Postman / REST API</div>
      <div class="skill">CI/CD (GitHub Actions)</div>
      <div class="skill">Java / JavaScript / Python</div>
      <div class="skill">Test Strategy / Reporting</div>
    </div>
  </section>

  <section id="projects" class="projects">
    <h3>Проекты</h3>
    <div class="projects-grid">
      <div class="project">
        <h4>Проект A — eCommerce</h4>
        <p>Разработка автотестов для пользовательских сценариев, интеграция с CI/CD пайплайном, тестирование checkout-флоу и API.</p>
      </div>
      <div class="project">
        <h4>Проект B — Fintech</h4>
        <p>API тестирование, нагрузочные тесты, ведение тест-документации и отчетности.</p>
      </div>
      <div class="project">
        <h4>Проект C — SaaS</h4>
        <p>Разработка стратегии тестирования, интеграция Playwright автотестов, мониторинг стабильности релизов.</p>
      </div>
    </div>
  </section>

  <section id="contact" class="contact">
    <h3>Контакты</h3>
    <p>Email: <a href="mailto:89504317422@mail.ru" style="color:var(--accent);">89504317422@mail.ru</a></p>
    <p>Telegram: <a href="https://t.me/s1nupLe" style="color:var(--accent);">@s1nupLe</a></p>
  </section>

  <footer>
    © 2025 Павел Белозерский — QA Engineer
  </footer>
</body>
</html>


  align-items: center;
  padding: 20px 60px;
  z-index: 1000;
  border-bottom: 1px solid var(--border);
}
header h1 {
  font-size: 20px;
  color: var(--accent);
}
nav a {
  margin-left: 24px;
  text-decoration: none;
  color: var(--text);
  font-weight: 500;
  transition: color 0.2s;
}
nav a:hover { color: var(--accent); }
.hero {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding-top: 140px;
  padding-bottom: 100px;
  background: radial-gradient(circle at top center, rgba(76,175,80,0.15), transparent 70%);
  text-align: center;
}
.hero img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid var(--accent);
  margin-bottom: 20px;
}
.hero h2 { font-size: 28px; margin-bottom: 10px; }
.hero p { color: var(--muted); }
section {
  padding: 80px 20px;
  max-width: 1000px;
  margin: 0 auto;
}
section h3 {
  font-size: 24px;
  color: var(--accent);
  margin-bottom: 20px;
  text-align: center;
}
.about, .skills, .projects, .contact {
  background: var(--card);
  border-radius: 16px;
  padding: 40px;
  box-shadow: 0 0 40px rgba(0,0,0,0.3);
  margin-bottom: 60px;
}
.skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  justify-content: center;
}
.skill {
  background: rgba(255,255,255,0.05);
  border: 1px solid var(--border);
  padding: 10px 18px;
  border-radius: 12px;
  font-size: 14px;
  color: var(--text);
  transition: background 0.2s;
}
.skill:hover { background: rgba(255,255,255,0.1); }
footer {
  text-align: center;
  color: var(--muted);
  font-size: 14px;
  padding: 40px 0;
  border-top: 1px solid var(--border);
  margin-top: 80px;
}
