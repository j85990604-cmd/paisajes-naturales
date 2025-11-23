<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Paisajes Naturales - Un Mundo por Explorar</title>
    <!-- Carga de Tailwind CSS para un diseño moderno y responsive -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f9fb; /* Fondo suave para mejor contraste */
        }
        .section-bg {
            background-color: #ffffff;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        .header-bg {
            background-color: #3b82f6; /* Azul primario para el encabezado */
        }
        .footer-bg {
            background-color: #1f2937; /* Gris oscuro para el pie de página */
        }
    </style>
</head>
<body class="text-gray-800">

    <!-- 1. ESTRUCTURA BÁSICA (HTML) y MENÚ (Usabilidad) -->
    <!-- Uso de <header>, <nav> (Semántica) -->
    <header class="header-bg sticky top-0 z-50 shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                <!-- Título jerarquizado (<h1/h2>) -->
                <h1 class="text-3xl font-bold text-white tracking-wider">
                    <a href="#" class="hover:text-blue-200 transition duration-300">GEO MUNDO</a>
                </h1>
                <!-- Navegación simple y funcional (<nav>) -->
                <nav class="hidden md:block">
                    <ul class="flex space-x-6">
                        <li><a href="#introduccion" class="text-white hover:text-blue-200 transition duration-300 font-medium">Inicio</a></li>
                        <li><a href="#tipos" class="text-white hover:text-blue-200 transition duration-300 font-medium">Tipos</a></li>
                        <li><a href="#galeria" class="text-white hover:text-blue-200 transition duration-300 font-medium">Galería</a></li>
                        <li><a href="#contacto" class="text-white hover:text-blue-200 transition duration-300 font-medium">Contacto</a></li>
                    </ul>
                </nav>
                <!-- Botón de menú para móvil (funcionalidad) -->
                <button id="menu-button" class="md:hidden p-2 rounded-md text-white hover:bg-blue-600 transition duration-300">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
        </div>
        <!-- Menú desplegable para móvil (navegación intuitiva) -->
        <div id="mobile-menu" class="md:hidden hidden bg-blue-700">
            <a href="#introduccion" class="block px-4 py-2 text-white hover:bg-blue-600">Inicio</a>
            <a href="#tipos" class="block px-4 py-2 text-white hover:bg-blue-600">Tipos</a>
            <a href="#galeria" class="block px-4 py-2 text-white hover:bg-blue-600">Galería</a>
            <a href="#contacto" class="block px-4 py-2 text-white hover:bg-blue-600">Contacto</a>
        </div>
    </header>

    <!-- Uso de <main> (Semántica) -->
    <main class="max-w-7xl mx-auto p-4 sm:p-6 lg:p-8">

        <!-- Sección de Introducción y Contenido Principal -->
        <section id="introduccion" class="section-bg rounded-xl p-8 mb-12">
            <h2 class="text-4xl font-extrabold text-blue-600 mb-6">La Inmensidad de los Paisajes Naturales</h2>
            <!-- Texto claro y relevante, párrafos organizados -->
            <p class="text-lg leading-relaxed mb-4">
                Los paisajes naturales son las áreas de la Tierra que no han sido alteradas significativamente por la actividad humana. Desde majestuosas montañas hasta vastos océanos y densas selvas, estos entornos representan la belleza prístina y la complejidad de los ecosistemas de nuestro planeta. Son esenciales para la biodiversidad y el equilibrio climático global.
            </p>
            <p class="text-lg leading-relaxed mb-6">
                Explorar y comprender estos paisajes nos conecta con la naturaleza y subraya la importancia de su conservación. Cada tipo de paisaje ofrece una experiencia única y alberga formas de vida especializadas.
            </p>

            <!-- Imagen destacada (Accesibilidad: texto alternativo) -->
            <div class="mt-8">
                <img class="rounded-lg shadow-xl w-full h-64 object-cover" 
                     src="https://placehold.co/1200x400/1e40af/ffffff?text=Montañas+Nevadas" 
                     alt="Vista panorámica de altas montañas nevadas reflejándose en un lago alpino.">
            </div>
        </section>

        <!-- 2. DISEÑO Y ESTILO (CSS) y CONTENIDO - Tipos de Paisajes -->
        <!-- Información organizada en secciones -->
        <section id="tipos" class="grid md:grid-cols-3 gap-8 mb-12">
            
            <!-- TARJETA 1: Montañas -->
            <div class="section-bg rounded-xl p-6 transition duration-300 hover:shadow-2xl">
                <h3 class="text-2xl font-semibold text-gray-900 mb-3">Montañas y Cordilleras</h3>
                <!-- Uso de lista organizada -->
                <ul class="list-disc list-inside space-y-2 text-gray-600">
                    <li>Se caracterizan por grandes altitudes y pendientes pronunciadas.</li>
                    <li>Clima frío y variaciones extremas de temperatura.</li>
                    <li>Hogar de especies adaptadas a la altura (ej. cabras montesas).</li>
                </ul>
                <img class="mt-4 rounded-md w-full h-40 object-cover" 
                     src="https://placehold.co/400x300/15803d/ffffff?text=Paisaje+Montañoso" 
                     alt="Cima rocosa de una montaña cubierta de nieve.">
            </div>

            <!-- TARJETA 2: Selvas y Bosques -->
            <div class="section-bg rounded-xl p-6 transition duration-300 hover:shadow-2xl">
                <h3 class="text-2xl font-semibold text-gray-900 mb-3">Selvas Tropicales</h3>
                <ul class="list-disc list-inside space-y-2 text-gray-600">
                    <li>Alta humedad y precipitaciones constantes (bosques lluviosos).</li>
                    <li>Máxima biodiversidad del planeta.</li>
                    <li>Sistemas de dosel denso y vegetación exuberante.</li>
                </ul>
                <img class="mt-4 rounded-md w-full h-40 object-cover" 
                     src="https://placehold.co/400x300/ca8a04/ffffff?text=Selva+Densa" 
                     alt="Interior de una selva densa con luz filtrándose a través del dosel.">
            </div>

            <!-- TARJETA 3: Desiertos y Zonas Áridas -->
            <div class="section-bg rounded-xl p-6 transition duration-300 hover:shadow-2xl">
                <h3 class="text-2xl font-semibold text-gray-900 mb-3">Desiertos Áridos</h3>
                <ul class="list-disc list-inside space-y-2 text-gray-600">
                    <li>Escasez extrema de agua y poca vegetación.</li>
                    <li>Grandes oscilaciones térmicas entre el día y la noche.</li>
                    <li>Formaciones de dunas de arena o paisajes rocosos.</li>
                </ul>
                <img class="mt-4 rounded-md w-full h-40 object-cover" 
                     src="https://placehold.co/400x300/991b1f/ffffff?text=Dunas+del+Desierto" 
                     alt="Dunas de arena rojiza bajo un cielo azul brillante.">
            </div>
        </section>

        <!-- Galería (Imágenes de diferentes fuentes/placeholders) -->
        <section id="galeria" class="mb-12">
            <h2 class="text-3xl font-bold text-gray-900 mb-6">Galería de Maravillas Naturales</h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <img class="rounded-lg shadow-md hover:scale-105 transition duration-300 aspect-square object-cover" 
                     src="https://placehold.co/400x400/10b981/ffffff?text=Glaciar" 
                     alt="Bloque de hielo azul de un glaciar.">
                <img class="rounded-lg shadow-md hover:scale-105 transition duration-300 aspect-square object-cover" 
                     src="https://placehold.co/400x400/9333ea/ffffff?text=Catarata" 
                     alt="Impresionante cascada cayendo sobre rocas musgosas.">
                <img class="rounded-lg shadow-md hover:scale-105 transition duration-300 aspect-square object-cover" 
                     src="https://placehold.co/400x400/f59e0b/ffffff?text=Arrecife" 
                     alt="Arrecife de coral submarino lleno de peces tropicales.">
                <img class="rounded-lg shadow-md hover:scale-105 transition duration-300 aspect-square object-cover" 
                     src="https://placehold.co/400x400/06b6d4/ffffff?text=Volcán" 
                     alt="Volcán activo con humo saliendo de su cráter.">
            </div>
        </section>

        <!-- Sección de Contacto (Enlaces funcionales y retroalimentación en botones) -->
        <section id="contacto" class="section-bg rounded-xl p-8 mb-12">
            <h2 class="text-3xl font-bold text-gray-900 mb-6">Únete a la Conservación</h2>
            <p class="text-lg leading-relaxed mb-6">
                Para más información sobre cómo proteger estos increíbles lugares, síguenos en nuestras redes sociales y visita organizaciones dedicadas.
            </p>

            <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                <!-- Botón con retroalimentación (cambio de color al pasar el mouse - Usabilidad/Funcionalidad) -->
                <a href="#" class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-medium rounded-full shadow-lg text-white bg-blue-600 hover:bg-blue-700 transition duration-150 ease-in-out">
                    <!-- Enlace funcional interno -->
                    Visita Nuestra Galería &rarr;
                </a>
                
                <!-- Enlace funcional externo -->
                <a href="https://www.worldwildlife.org/" target="_blank" class="inline-flex items-center justify-center px-6 py-3 border border-blue-600 text-base font-medium rounded-full shadow-lg text-blue-600 bg-white hover:bg-blue-50 transition duration-150 ease-in-out">
                    Organización de Conservación Externa
                </a>
            </div>
        </section>

    </main>

    <!-- Uso de <footer> (Semántica) -->
    <footer class="footer-bg text-white py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <!-- Texto alternativo en un pie de página -->
            <p class="text-sm">
                &copy; 2025 GEO MUNDO. Todos los derechos reservados por jose carlos trocha
                <a href="#introduccion" class="hover:text-blue-300">Política de Privacidad</a> |
                <a href="#contacto" class="hover:text-blue-300">Términos de Uso</a>
            </p>
            <!-- Uso de <small> para texto secundario (Semántica) -->
            <small class="block mt-2 text-gray-400">
                Diseño optimizado para dispositivos  y un buen uso de la pagina.
            </small>
        </div>
    </footer>

    <!-- Script para la funcionalidad del menú móvil -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const menuButton = document.getElementById('menu-button');
            const mobileMenu = document.getElementById('mobile-menu');

            menuButton.addEventListener('click', () => {
                // Toggle para mostrar/ocultar el menú
                mobileMenu.classList.toggle('hidden');
            });

            // Ocultar el menú móvil después de hacer clic en un enlace
            mobileMenu.querySelectorAll('a').forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });
        });

        // Simulación de log de debug para aspecto técnico (Compatibilidad)
        console.log("DEBUG: La página ha cargado la estructura, el estilo (Tailwind) y el script básico de navegación.");
    </script>
</body>
</html>


