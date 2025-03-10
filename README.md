<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Viewer</title>

    <!-- CDN de Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        html, body {
            height: 100%;
            margin: 0;
            font-size: 14px;
        }
        main {
            height: calc(100vh - 70px);
            padding: 16px;
        }
        iframe {
            width: 100%;
            height: 100%;
            border-radius: 8px;
        }
        header {
            height: 60px;
        }
    </style>
</head>
<body class="bg-gray-100 flex flex-col">

    <!-- Panel Superior (Header) -->
    <header class="bg-blue-600 text-white p-4 shadow-md flex justify-between items-center w-full fixed top-0 left-0 z-50">
        <h1 class="text-xl font-semibold">Dashboard Viewer</h1>
        <nav>
            <ul class="flex space-x-6 text-lg">
                <li><a href="#" class="hover:underline">Inicio</a></li>
                <li><a href="#" class="hover:underline">Dashboards</a></li>
                <li><a href="#" class="hover:underline">Configuración</a></li>
            </ul>
        </nav>
    </header>

    <!-- Contenido Principal -->
    <main class="flex-1 mt-[60px] w-full">
        <div class="bg-white p-6 rounded-lg shadow-lg h-full">
            <h2 class="text-2xl font-bold mb-6">Cargar Dashboard</h2>
            <div class="mb-6 space-x-4">
                <button onclick="loadDashboard('clientes')" class="bg-blue-600 text-white px-4 py-2 text-lg rounded hover:bg-blue-700">Clientes</button>
                <button onclick="loadDashboard('interno')" class="bg-blue-600 text-white px-4 py-2 text-lg rounded hover:bg-blue-700">Interno</button>
                <button onclick="loadDashboard('keepgo')" class="bg-blue-600 text-white px-4 py-2 text-lg rounded hover:bg-blue-700">Pannel Keepgo</button>
            </div>
            <iframe id="dashboardFrame" src="" frameborder="0" allowfullscreen></iframe>
        </div>
    </main>

    <script>
        function loadDashboard(type) {
            var urls = {
                'clientes': 'https://app.powerbi.com/view?r=eyJrIjoiMzY1NGJjNWQtYjFjYy00MTQwLWJlMj

