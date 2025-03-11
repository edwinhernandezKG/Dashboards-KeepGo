<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboards de Power BI</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        h1 {
            background-color: #0078D7;
            color: white;
            padding: 15px;
            margin: 0;
        }
        .content {
            max-width: 900px;
            margin: auto;
            padding: 20px;
            text-align: left;
        }
        .dashboard-container {
            display: flex;
            justify-content: center;
            gap: 10px;
            padding: 20px;
            flex-wrap: wrap;
        }
        .dashboard {
            flex: 1;
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
            min-width: 300px;
        }
        iframe {
            width: 100%;
            height: 500px;
            border: none;
        }
        .footer {
            position: fixed;
            bottom: 10px;
            right: 10px;
            font-size: 14px;
            color: rgba(0, 0, 0, 0.5);
        }
        .footer a {
            text-decoration: none;
            color: #0078D7;
        }
    </style>
</head>
<body>
    <h1>Dashboards de Power BI</h1>

    <div class="content">
        <h2>📊 Acerca del Proyecto</h2>
        <p>Este proyecto proporciona una interfaz web para visualizar dashboards de Power BI en una sola pestaña, mejorando la experiencia del usuario y facilitando el acceso a la información.</p>
        
        <h2>🚀 Características</h2>
        <ul>
            <li>Visualización de dashboards directamente en la página mediante `iframe`.</li>
            <li>Diseño moderno y responsivo con CSS.</li>
            <li>Organización eficiente con un layout flexible.</li>
            <li>Incluye enlaces directos a los dashboards de Power BI.</li>
        </ul>
    </div>

    <div class="dashboard-container">
        <div class="dashboard">
            <h2>Clientes</h2>
            <iframe src="https://app.powerbi.com/view?r=eyJrIjoiMzY1NGJjNWQtYjFjYy00MTQwLWJlMjEtYTk5NzAyODUyNTY2IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9"></iframe>
        </div>
        <div class="dashboard">
            <h2>Interno</h2>
            <iframe src="https://app.powerbi.com/view?r=eyJrIjoiZjJhYTVmNGQtNmZiZC00MTYyLWI3OWQtNzM0YTkxNjU2NTkyIiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9"></iframe>
        </div>
    </div>
    <div class="dashboard-container">
        <div class="dashboard">
            <h2>Pannel KeepGo</h2>
            <iframe src="https://app.powerbi.com/view?r=eyJrIjoiOTc3MjhjZDctNWRmNy00OGE4LTg3ZDUtMDYxMGI2Njg5MDg1IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9&pageName=527e30742b4415e0ee60"></iframe>
        </div>
    </div>

    <div class="content">
        <h2>🛠 Instalación y Uso</h2>
        <ol>
            <li>Clona este repositorio:</li>
            <pre><code>git clone https://github.com/tu-repo/dashboards-powerbi.git</code></pre>
            <li>Abre el archivo <code>index.html</code> en tu navegador.</li>
            <li>Disfruta de los dashboards sin salir de la pestaña.</li>
        </ol>
    </div>
    
    <div class="footer">
        Powered by <a href="https://www.keepgo.com/" target="_blank">KeepGo</a>
    </div>
</body>
</html>

