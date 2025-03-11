<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Repositorio de Dashboards</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            height: 100vh;
        }
        .top-panel {
            background-color: #004080;
            color: white;
            padding: 15px;
            text-align: center;
            font-size: 20px;
            font-weight: bold;
        }
        .container {
            display: flex;
            flex: 1;
        }
        .sidebar {
            width: 250px;
            background: #f4f4f4;
            padding: 15px;
            display: flex;
            flex-direction: column;
        }
        .sidebar a {
            padding: 10px;
            text-decoration: none;
            color: #333;
            display: block;
            margin-bottom: 10px;
            border-radius: 5px;
            background: #ddd;
        }
        .sidebar a:hover {
            background: #bbb;
        }
        .content {
            flex: 1;
            padding: 15px;
        }
        iframe {
            width: 100%;
            height: 100%;
            border: none;
            allowfullscreen: true;
        }
    </style>
    <script>
        function loadDashboard(url) {
            document.getElementById('dashboardFrame').src = url + "&navContentPaneEnabled=false";
        }
    </script>
</head>
<body>
    <div class="top-panel">Repositorio de Dashboards</div>
    <div class="container">
        <div class="sidebar">
            <a href="#" onclick="loadDashboard('https://app.powerbi.com/view?r=eyJrIjoiZjJhYTVmNGQtNmZiZC00MTYyLWI3OWQtNzM0YTkxNjU2NTkyIiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9')">Dashboard Interno</a>
            <a href="#" onclick="loadDashboard('https://app.powerbi.com/view?r=eyJrIjoiMzY1NGJjNWQtYjFjYy00MTQwLWJlMjEtYTk5NzAyODUyNTY2IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9')">Dashboard Clientes</a>
            <a href="#" onclick="loadDashboard('https://app.powerbi.com/view?r=eyJrIjoiOTc3MjhjZDctNWRmNy00OGE4LTg3ZDUtMDYxMGI2Njg5MDg1IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9')">Dashboard Pannel KeepGo</a>
        </div>
        <div class="content">
            <iframe id="dashboardFrame" allowfullscreen></iframe>
        </div>
    </div>
</body>
</html>

