<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portal Power BI | Powerade</title>
<style>
  body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #0d1117, #1c1f26);
    color: #e6edf3;
  }

  header {
    display: flex;
    align-items: center;
    justify-content: center; /* centra el título */
    background: rgba(22, 27, 34, 0.85);
    backdrop-filter: blur(10px);
    padding: 12px 30px; /* más pequeño */
    box-shadow: 0 2px 15px rgba(0,0,0,0.6);
    position: sticky;
    top: 0;
    z-index: 1000;
  }

  header img {
    height: 55px;
    margin-right: auto; /* lo pega a la izquierda */
    background: rgba(255,255,255,0.8); /* fondo blanco transparente */
    border-radius: 8px;
    padding: 4px 8px;
  }

  header h1 {
    font-size: 1.6rem;
    color: #00b4ff;
    margin: 0;
    text-align: center;
    flex: 1;
  }

  main {
    max-width: 1600px;
    margin: auto;
    padding: 40px 20px;
  }

  .dashboard-card {
    background: rgba(22, 27, 34, 0.7);
    border-radius: 20px;
    padding: 25px;
    margin-bottom: 50px;
    box-shadow: 0 8px 24px rgba(0,0,0,0.6);
    backdrop-filter: blur(12px);
    transition: transform 0.3s ease;
    text-align: center;
  }

  .dashboard-card:hover {
    transform: translateY(-5px);
  }

  .dashboard-card h2 {
    margin-top: 0;
    font-size: 1.5rem;
    color: #00b4ff;
  }

  .dashboard-card p {
    margin: 8px 0 20px;
    color: #c9d1d9;
  }

  iframe {
    border: none;
    border-radius: 16px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.4);
  }

  .big {
    width: 1400px;
    height: 850px;
  }

  .medium {
    width: 100%;
    height: 550px;
  }

  footer {
    text-align: center;
    padding: 25px;
    background: rgba(22, 27, 34, 0.9);
    font-size: 0.95rem;
    color: #8b949e;
    border-top: 1px solid #30363d;
    margin-top: 40px;
  }

  footer strong {
    color: #00b4ff;
  }

  .lb-whatsapp-widget {
    bottom: 190px !important;
  }
</style>
</head>
<body>

  <header>
    <img src="https://i.postimg.cc/tTD72y2F/c947d0-eadc0d6e3f3c4184a5f64991dc4338a1-mv2-removebg-preview.png" alt="Logo Powerade">
    <h1>Portal de Dashboards</h1>
  </header>

  <main>
    <div class="dashboard-card">
      <h2>Dashboard Clientes</h2>
      <p>Análisis detallado de clientes.</p>
      <iframe title="Dashboard Clientes" class="big" src="https://app.powerbi.com/view?r=eyJrIjoiOGMyMDc4OTItMGQ5Ny00OTcxLWIzYjctMDZlN2I3YzNiMmE0IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9" allowFullScreen="true"></iframe>
    </div>

    <div class="dashboard-card">
      <h2>Dashboard Interno</h2>
      <p>Datos internos estratégicos de la empresa.</p>
      <iframe title="MesaDeServicio KeepGo" class="big" src="https://app.powerbi.com/view?r=eyJrIjoiY2VhYzdkZmMtZDY1NS00YTkwLTkwNTQtNTVjOWJkZDcyYjNhIiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9" allowFullScreen="true"></iframe>
    </div>

    <div class="dashboard-card">
      <h2>Dashboard Pannel KeepGo</h2>
      <p>Información de Pannel KeepGo.</p>
      <iframe class="medium" allowFullScreen="true" 
        src="https://app.powerbi.com/view?r=eyJrIjoiZmM4OGU2MWQtZDRhZS00YzU4LWEzMWEtMTBhMjhlYmY0MzQzIiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9"></iframe>
    </div>
  </main>

  <footer>
    <p><strong>Powered by KeepGo 🚀</strong></p>
  </footer>

  <!-- WhatsApp Widget -->
  <script>
    window.lbWhatsappWidgetSettings = {
     "avatar_url": "https://storage.googleapis.com/media.landbot.io/774092/web_widget/fda0ccf0-194f-4b2c-9767-aebec1097b01/avatar/avatar.jpg?1752104288765",
     "brand_name": "STRATECH Mesa de Servicio",
     "button_background_color": "#0f0c0c",
     "button_rounded_corners": "4",
     "button_text": "Envianos Un Mensaje!",
     "cta_text": "¡Iniciar Chat!",
     "input_color": "#0f0c0c",
     "welcome_text": "💬 ¡Hola, bienvenido/a a STRATECH! 🚀",
     "wa_phone": "5215651138365"
    };
  </script>
  <script src="https://static.landbot.io/livechat-widget/index.js" defer></script>

</body>
</html>

