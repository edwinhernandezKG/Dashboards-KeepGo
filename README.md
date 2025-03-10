<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Viewer</title>

    <!-- CDN de Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Ajuste para ocupar toda la pantalla */
        html, body {
            height: 100%;
            margin: 0;
            overflow: hidden;
        }
        main {
            height: calc(100vh - 70px); /* Ajusta al tamaño del header */
        }
    </style>
</head>
<body class="bg-gray-100 flex flex-col">

    <!-- Panel Superior (Header) -->
    <header class="bg-blue-600 text-white p-4 shadow-md flex justify-between items-center w-full fixed top-0 left-0 z-50 h-[70px]">
        <h1 class="text-2xl font-semibold">Dashboard Viewer</h1>
        <nav>
            <ul class="flex space-x-6 text-lg">
                <li><a href="#" class="hover:underline">Inicio</a></li>
                <li><a href="#" class="hover:underline">Dashboards</a></li>
                <li><a href="#" class="hover:underline">Configuración</a></li>
            </ul>
        </nav>
    </header>

    <!-- Contenido Principal -->
    <main class="flex-1 p-4 mt-[70px] w-full">
        <div class="bg-white p-6 rounded-lg shadow-lg h-full">
            <h2 class="text-2xl font-bold mb-6">Cargar Dashboard</h2>
            <div class="mb-6 space-x-4">
                <button onclick="loadDashboard('clientes')" class="bg-blue-600 text-white px-4 py-2 text-lg rounded hover:bg-blue-700">Clientes</button>
                <button onclick="loadDashboard('interno')" class="bg-blue-600 text-white px-4 py-2 text-lg rounded hover:bg-blue-700">Interno</button>
                <button onclick="loadDashboard('keepgo')" class="bg-blue-600 text-white px-4 py-2 text-lg rounded hover:bg-blue-700">Pannel Keepgo</button>
            </div>
            <iframe id="dashboardFrame" class="w-full h-full border rounded-md" src="" frameborder="0" allowfullscreen></iframe>
        </div>
    </main>

    <script>
        function loadDashboard(type) {
            var urls = {
                'clientes': 'https://app.powerbi.com/view?r=eyJrIjoiMzY1NGJjNWQtYjFjYy00MTQwLWJlMjEtYTk5NzAyODUyNTY2IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9',
                'interno': 'https://app.powerbi.com/view?r=eyJrIjoiZjJhYTVmNGQtNmZiZC00MTYyLWI3OWQtNzM0YTkxNjU2NTkyIiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9',
                'keepgo': 'https://app.powerbi.com/view?r=eyJrIjoiOTc3MjhjZDctNWRmNy00OGE4LTg3ZDUtMDYxMGI2Njg5MDg1IiwidCI6ImIxM2NlNGM5LTJiZTYtNDg0NC04Y2Q5LTYwOTcyMGFmYWY5YiJ9'
            };
            document.getElementById('dashboardFrame').src = urls[type];
        }
    </script>

</body>
</html>
