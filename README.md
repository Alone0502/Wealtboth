<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Suscripción Premium - WealtBoth</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: black;
      overflow: hidden;
    }
    .background {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -2;
      background: url('https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExb2Z6bzRwc2V3N2dvMmQ1M2M3bzZ1Z3N2bTRtZHNncWFuaWF2YzY1bCZlcD12MV9naWZzX3NlYXJjaCZjdD1n/Wq8B4Djs0AoTuG8yow/giphy.gif') no-repeat center center fixed;
      background-size: cover;
      animation: pulseBG 10s ease-in-out infinite;
    }
    @keyframes pulseBG {
      0%, 100% { filter: brightness(1); }
      50% { filter: brightness(1.1); }
    }
    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(255, 255, 255, 0.7);
      z-index: -1;
    }
    .container {
      position: relative;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 40px 30px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
      width: 100%;
      max-width: 420px;
      text-align: center;
      animation: fadeIn 1s ease-in-out;
      z-index: 1;
      backdrop-filter: blur(3px);
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    h2 {
      color: #6a1b9a;
      margin-bottom: 20px;
    }
    p {
      color: #444;
      font-size: 15px;
      margin-bottom: 20px;
    }
    input {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 14px;
    }
    button {
      width: 100%;
      padding: 12px;
      background-color: #8e24aa;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s, transform 0.2s;
      margin-top: 10px;
    }
    button:hover {
      background-color: #6a1b9a;
      transform: translateY(-2px);
    }
    .card-preview {
      background: linear-gradient(135deg, #ab47bc, #ce93d8);
      color: white;
      padding: 20px;
      border-radius: 12px;
      text-align: left;
      margin-top: 25px;
      font-family: 'Courier New', Courier, monospace;
      font-size: 14px;
      animation: floatCard 4s ease-in-out infinite;
    }
    @keyframes floatCard {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-5px); }
    }
    .note {
      font-size: 12px;
      color: #888;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="background"></div>
  <div class="overlay"></div>
  <div class="container">
    <h2>🌟 Suscripción Premium a WealtBoth</h2>
    <p>Accede a consejos financieros exclusivos, herramientas personalizadas y asistencia de inversión simulada. ¡Tu camino al éxito empieza aquí!</p>

    <input type="email" placeholder="Tu correo electrónico" required />
    <input type="text" placeholder="Nombre en la tarjeta" />
    <input type="text" placeholder="0000 0000 0000 0000" maxlength="19" />
    <input type="text" placeholder="MM/AA - CVV" maxlength="9" />

    <button>Simular Suscripción</button>

    <div class="card-preview">
      💳 <strong>Vista previa de tarjeta</strong><br>
      Titular: Juan Pérez<br>
      Número: **** **** **** 1234<br>
      Expira: 12/28<br>
      CVV: ***
    </div>

    <p class="note">⚠️ Esta es una simulación educativa. No se recolectan datos reales ni se realizan pagos.</p>
  </div>
</body>
</html>
