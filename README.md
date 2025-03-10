<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Viewer</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100">
    <div class="flex flex-col h-screen">
        <!-- Panel Superior -->
        <header class="bg-blue-600 text-white p-4 shadow-md flex justify-between items-center">
            <h1 class="text-lg font-semibold">Dashboard Viewer</h1>
            <nav>
                <ul class="flex space-x-4">
                    <li><a href="#" class="hover:underline">Inicio</a></li>
                    <li><a href="#" class="hover:underline">Dashboards</a></li>
                    <li><a href="#" class="hover:underline">Configuración</a></li>
                </ul>
            </nav>
        </header>

        <!-- Contenido Principal -->
        <main class="flex-1 p-4">
            <div class="bg-white p-6 rounded-lg shadow-md h-full">
                <h2 class="text-xl font-bold mb-4">Cargar Dashboard</h2>
                <div class="mb-4">
                    <button onclick="loadDashboard('clientes')" class="bg-blue-600 text-white p-2 rounded hover:bg-blue-700 mr-2">Clientes</button>
                    <button onclick="loadDashboard('interno')" class="bg-blue-600 text-white p-2 rounded hover:bg-blue-700 mr-2">Interno</button>
                    <button onclick="loadDashboard('keepgo')" class="bg-blue-600 text-white p-2 rounded hover:bg-blue-700">Pannel Keepgo</button>
                </div>
                <iframe id="dashboardFrame" class="w-full h-[80vh] border rounded-md" src="" frameborder="0" allowfullscreen></iframe>
            </div>
        </main>
    </div>

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
