<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Halaman Password</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      background: linear-gradient(45deg, #ff6b6b, #f4a261, #2a9d8f, #264653);
      background-size: 400% 400%;
      animation: gradientAnimation 10s ease infinite;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      overflow: hidden;
    }

    @keyframes gradientAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .login-container {
      text-align: center;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
      position: relative;
      z-index: 2;
      width: 90%;
      max-width: 300px;
      box-sizing: border-box;
    }

    .login-container h1 {
      margin-bottom: 15px;
      font-size: 20px;
    }

    .login-container input {
      padding: 8px;
      font-size: 14px;
      width: 100%;
      margin-bottom: 10px;
      border: 2px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
    }

    .notification {
      display: none;
      margin-top: 10px;
      padding: 10px;
      font-size: 14px;
      color: white;
      border-radius: 5px;
    }

    .notification.success {
      background-color: #28a745;
    }

    .notification.error {
      background-color: #dc3545;
    }

    canvas {
      position: absolute;
      top: 0;
      left: 0;
      z-index: 1;
      pointer-events: none;
    }

    #changePasswordBtn {
      display: none;
      padding: 8px 16px;
      background-color: #28a745;
      color: white;
      font-size: 14px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 10px;
    }

    .link-buttons {
      display: none;
      margin-top: 15px;
    }

    .link-buttons a {
      display: inline-block;
      margin: 5px;
      padding: 8px 14px;
      background-color: #007bff;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      font-size: 14px;
    }

    .link-buttons a:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <canvas id="confettiCanvas"></canvas>

  <div class="login-container">
    <h1>Masukkan Password</h1>
    <input type="password" id="passwordInput" placeholder="Password" />
    <div id="notification" class="notification"></div>

    <div class="link-buttons" id="linkButtons">
      <a href="https://www.poki.com" target="_blank">Lanjut ke Poki</a>
      <a href="https://linktr.ee/M.hafiz.albukhori" target="_blank">Lanjut ke Linktree</a>
    </div>

    <hr style="margin: 20px 0;" />

    <input type="password" id="newPassword" placeholder="Password Baru" />
    <input type="password" id="confirmPassword" placeholder="Konfirmasi Password Baru" />
    <button id="changePasswordBtn">Ubah Password</button>
    <div id="changeNotification" class="notification"></div>
  </div>

  <script>
    document.addEventListener("DOMContentLoaded", function () {
      let correctPassword = "asd123";

      const passwordInput = document.getElementById("passwordInput");
      const notification = document.getElementById("notification");

      const newPassword = document.getElementById("newPassword");
      const confirmPassword = document.getElementById("confirmPassword");
      const changePasswordBtn = document.getElementById("changePasswordBtn");
      const changeNotification = document.getElementById("changeNotification");

      const canvas = document.getElementById("confettiCanvas");
      const ctx = canvas.getContext("2d");
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;

      const confetti = [];
      const colors = ["#FF0000", "#FF7F00", "#FFFF00", "#00FF00", "#0000FF", "#4B0082", "#8B00FF"];
      const linkButtons = document.getElementById("linkButtons");

      function createConfetti(x, y) {
        const size = Math.random() * 10 + 5;
        const color = colors[Math.floor(Math.random() * colors.length)];
        const speed = Math.random() * 4 + 2;
        const angle = Math.random() * 2 * Math.PI;
        const xSpeed = Math.cos(angle) * speed;
        const ySpeed = Math.sin(angle) * speed;
        confetti.push({ x, y, size, color, xSpeed, ySpeed, opacity: 1 });
      }

      function updateConfetti() {
        for (let i = confetti.length - 1; i >= 0; i--) {
          const p = confetti[i];
          p.x += p.xSpeed;
          p.y += p.ySpeed;
          p.opacity -= 0.02;
          if (p.opacity <= 0) confetti.splice(i, 1);
        }
      }

      function drawConfetti() {
        ctx.clearRect(0, 0, canvas.width, canvas.height);
        updateConfetti();
        for (const p of confetti) {
          ctx.beginPath();
          ctx.arc(p.x, p.y, p.size, 0, Math.PI * 2);
          ctx.fillStyle = p.color;
          ctx.globalAlpha = p.opacity;
          ctx.fill();
        }
        ctx.globalAlpha = 1;
        requestAnimationFrame(drawConfetti);
      }

      passwordInput.addEventListener("input", () => {
        if (passwordInput.value === correctPassword) {
          notification.className = "notification success";
          notification.textContent = "Password Benar!";
          notification.style.display = "block";
          linkButtons.style.display = "block";

          for (let i = 0; i < 200; i++) {
            createConfetti(window.innerWidth / 2, window.innerHeight / 2);
          }
          drawConfetti();
        } else if (passwordInput.value.length > 0) {
          notification.className = "notification error";
          notification.textContent = "Password Salah!";
          notification.style.display = "block";
          linkButtons.style.display = "none";
        }
      });

      function checkPasswordMatch() {
        const newVal = newPassword.value;
        const confirmVal = confirmPassword.value;

        if (newVal === "" || confirmVal === "") {
          changeNotification.style.display = "none";
          changePasswordBtn.style.display = "none";
          return;
        }

        if (newVal === confirmVal) {
          changeNotification.className = "notification success";
          changeNotification.textContent = "Password cocok, siap diubah";
          changeNotification.style.display = "block";
          changePasswordBtn.style.display = "inline-block";
        } else {
          changeNotification.className = "notification error";
          changeNotification.textContent = "Password tidak cocok";
          changeNotification.style.display = "block";
          changePasswordBtn.style.display = "none";
        }
      }

      newPassword.addEventListener("input", checkPasswordMatch);
      confirmPassword.addEventListener("input", checkPasswordMatch);

      changePasswordBtn.addEventListener("click", () => {
        correctPassword = newPassword.value;
        changeNotification.className = "notification success";
        changeNotification.textContent = "Password berhasil diubah!";
        newPassword.value = "";
        confirmPassword.value = "";
        changePasswordBtn.style.display = "none";
        setTimeout(() => (changeNotification.style.display = "none"), 5000);
      });
    });
  </script>
</body>
</html>
