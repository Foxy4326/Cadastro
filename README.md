<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Cadastro para 2026</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .form-container {
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      width: 300px;
    }
    h2 {
      text-align: center;
      margin-bottom: 20px;
    }
    input {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
    }
    button {
      width: 100%;
      padding: 10px;
      background-color: #ff6f61;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover {
      background-color: #e05d52;
    }
  </style>
</head>
<body>

  <div class="form-container">
    <h2>🎉 Cadastre-se!</h2>
    <form id="signupForm">
      <input type="text" id="name" placeholder="Seu nome" required />
      <input type="email" id="email" placeholder="Seu e-mail" required />
      <button type="submit">Avançar para 2026!</button>
    </form>
  </div>

  <script>
    document.getElementById('signupForm').addEventListener('submit', function(e) {
      e.preventDefault(); // Impede o envio real (sem backend)

      // Aqui você poderia enviar os dados para um backend, se quiser
      // Por enquanto, só redirecionamos
      alert('Cadastro feito com sucesso! 🎊');
      window.location.href = 'https://foxy4326.github.io/Contagem-regressiva-para-2026/';
    });
  </script>

</body>
</html>