<!DOCTYPE html>
<html lang="mk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Kategorii za motor vozacka dozvola</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet" />
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: 'Inter', sans-serif;
      background: linear-gradient(135deg, #f0f4fb 0%, #d9e2f3 100%);
      color: #1a1a1a;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }
    header {
      background: linear-gradient(135deg, #2b6cb0, #4a90e2);
      color: white;
      padding: 60px 20px;
      text-align: center;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
      border-bottom-left-radius: 60px;
      border-bottom-right-radius: 60px;
    }
    header h1 {
      font-size: 36px;
      font-weight: 700;
      letter-spacing: 1px;
      text-transform: uppercase;
      text-shadow: 0 2px 6px rgba(0,0,0,0.25);
    }

    .intro-highlight {
      font-size: 20px;
      color: #2b4a78;
      font-weight: 500;
      text-align: center;
      line-height: 1.6;
      max-width: 700px;
      margin: 40px auto;
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      overflow: hidden;
      text-overflow: ellipsis;
    }

    main.container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 30px;
      max-width: 1200px;
      margin: 0 auto 100px;
      padding: 0 20px;
      flex-grow: 1;
    }

    .card {
      background: white;
      border-radius: 18px;
      padding: 25px 20px;
      box-shadow: 0 10px 24px rgba(0, 0, 0, 0.06);
      transition: transform 0.25s ease, box-shadow 0.25s ease;
      text-decoration: none;
      color: inherit;
      border-top: 6px solid #2b6cb0;
      position: relative;
      overflow: hidden;
      cursor: pointer;
    }

    .card:hover {
      transform: translateY(-8px);
      box-shadow: 0 18px 40px rgba(0, 0, 0, 0.12);
    }

    .card h2 {
      font-size: 26px;
      margin-bottom: 12px;
      color: #2b6cb0;
      font-weight: 700;
    }

    .details {
      font-size: 16px;
      line-height: 1.7;
      color: #2f2f2f;
    }

    footer {
      background-color: #1f2d48;
      color: #cfd9e8;
      padding: 50px 20px 20px;
      position: relative;
      overflow: hidden;
      text-align: center;
      font-size: 14px;
      letter-spacing: 0.02em;
      box-shadow: inset 0 10px 30px rgba(255, 255, 255, 0.05);
    }

    footer::before {
      content: "";
      position: absolute;
      top: 20px;
      left: 50%;
      transform: translateX(-50%);
      width: 80%;
      height: 6px;
      background: repeating-linear-gradient(
        90deg,
        #4a90e2,
        #4a90e2 10px,
        transparent 10px,
        transparent 20px
      );
      border-radius: 3px;
      opacity: 0.6;
    }

    .email-btn {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      width: 48px;
      height: 48px;
      background-color: #4a90e2;
      border-radius: 50%;
      text-decoration: none;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
      margin-left: 15px;
      cursor: pointer;
    }

    .email-btn svg {
      fill: #fff;
    }

    .modal {
      display: none;
      position: fixed;
      z-index: 999;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0,0,0,0.5);
    }

    .modal-content {
      background-color: #ffffff;
      margin: 10% auto;
      padding: 20px 30px;
      border-radius: 10px;
      max-width: 400px;
      text-align: center;
    }

    .modal-content h3 {
      margin-bottom: 10px;
      font-size: 20px;
      color: #2b4a78;
    }

    .modal-content p {
      font-size: 16px;
      color: #333;
    }

    .close-btn {
      margin-top: 20px;
      padding: 8px 16px;
      background-color: #2b6cb0;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    @media (max-width: 1000px) {
      main.container {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 600px) {
      main.container {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>КАТЕГОРИИ ЗА МОТОР / ВОЗАЧКА ДОЗВОЛА</h1>
  </header>

  <div class="intro-highlight">
    Дознајте која категорија на мотор ви одговара според вашата <strong>возраст</strong>, <strong>искуство</strong> и <strong>потреби</strong>. 
  </div>

  <main class="container">
    <a href="am.html" class="card">
      <h2>AM</h2>
      <div class="details">
        • Лесни мотори (скутери, мопеди)<br>
        • До 49 cm³, max 45 km/h<br>
        • Мин. возраст: 15 години
      </div>
    </a>

    <a href="a1.html" class="card">
      <h2>A1</h2>
      <div class="details">
        • Мотори до 125 cm³, max 11 kW<br>
        • Трицикли до 15 kW<br>
        • Мин. возраст: 16 години
      </div>
    </a>

    <a href="a2.html" class="card">
      <h2>A2</h2>
      <div class="details">
        • Мотори до 35 kW (48 PS)<br>
        • Сооднос до 0.2 kW/kg<br>
        • Мин. возраст: 18 години
      </div>
    </a>

    <a href="a.html" class="card">
      <h2>A</h2>
      <div class="details">
        • Сите типови мотори и трицикли<br>
        • Без ограничувања<br>
        • Мин. возраст: 24 или 20 со A2 (2 години)
      </div>
    </a>
  </main>

  <footer>
    <div style="display: flex; justify-content: center; align-items: center; gap: 16px; flex-wrap: wrap;">
      <div>
        Информациите се базирани на официјални извори од Министерството за внатрешни работи.<br>
        Контактирајте нѐ доколку имате прашања или ви треба дополнителна помош.
      </div>
      <div class="email-btn" onclick="document.getElementById('modal').style.display='block'">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
          <path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 
          2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 
          4-8 5-8-5V6l8 5 8-5v2z"/>
        </svg>
      </div>
    </div>
  </footer>

  <!-- Modal -->
  <div class="modal" id="modal">
    <div class="modal-content">
      <h3>Контакт е-пошта</h3>
      <p>petar.gjorgjiev7@gmail.com</p>
      <button class="close-btn" onclick="document.getElementById('modal').style.display='none'">Затвори</button>
    </div>
  </div>

</body>
</html>
