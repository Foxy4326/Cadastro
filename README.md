<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Cadastro para 2026</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }
    .form-container {
      background: white;
      padding: 30px;
      border-radius: 16px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
      width: 100%;
      max-width: 400px;
      text-align: center;
    }
    h2 {
      margin-bottom: 24px;
      color: #333;
      font-size: 24px;
    }
    input {
      width: 100%;
      padding: 14px;
      margin: 10px 0;
      border: 1px solid #ddd;
      border-radius: 8px;
      font-size: 16px;
      transition: border-color 0.3s;
    }
    input:focus {
      outline: none;
      border-color: #ff6b6b;
    }
    button {
      width: 100%;
      padding: 14px;
      background: #ff6b6b;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 18px;
      font-weight: bold;
      cursor: pointer;
      margin-top: 10px;
      transition: background 0.3s;
    }
    button:hover {
      background: #ff5252;
    }
    @media (max-width: 480px) {
      .form-container {
        padding: 20px;
      }
    }
  </style>
</head>
<body>
  <div class="form-container">
    <h2>🎉 Cadastre-se para 2026!</h2>
    <form id="signupForm">
      <input type="text" id="name" placeholder="Seu nome completo" required />
      <input type="email" id="email" placeholder="Seu e-mail" required />
      <button type="submit">Ir para a contagem regressiva!</button>
    </form>
  </div>

  <script>
    document.getElementById('signupForm').addEventListener('submit', function(e) {
      e.preventDefault();
      
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();

      // Opcional: validação simples
      if (!name || !email) {
        alert('Por favor, preencha todos os campos.');
        return;
      }

      // Aqui você poderia enviar para um backend (ex: Formspree, Firebase)
      // Mas como é só redirecionamento, vamos direto:
      alert(`Obrigado, ${name}! 🎊\nVocê será redirecionado para a contagem regressiva.`);
      
      // Redireciona para o site de contagem regressiva
      window.location.href = 'https://foxy4326.github.io/Contagem-regressiva-para-2026/';
    });
  </script>
</body>
</html>