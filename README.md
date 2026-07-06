<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>W&F Aroma Café - Tienda Oficial</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts Premium -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome para iconos de Yape, Plin y WhatsApp -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        espresso: '#2E1E12',
                        gold: '#C19D60',
                        cream: '#FAF6F0',
                        forest: '#1E352F',
                        yape: '#742384',
                        plin: '#00D1C4'
                    }
                }
            }
        }
    </script>
    
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #FAF6F0;
            color: #2E1E12;
        }
        h1, h2, h3, h4, .font-serif {
            font-family: 'Playfair Display', serif;
        }
        .glass-nav {
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
        }
    </style>
</head>
<body class="min-h-screen flex flex-col antialiased">

    <!-- Barra de Navegación -->
    <nav class="glass-nav sticky top-0 z-50 border-b border-stone-200/80 shadow-sm transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logotipo de la Marca -->
                <div class="flex flex-col items-center sm:items-start">
                    <span class="text-xl sm:text-2xl font-bold tracking-widest text-espresso font-serif">W & F</span>
                    <span class="text-[10px] uppercase tracking-[0.2em] text-gold font-medium mt-[-4px]">Aroma Café</span>
                </div>
                <!-- Enlaces de Navegación -->
                <div class="hidden md:flex items-center gap-8 text-sm font-medium text-espresso/80">
                    <a href="#inicio" class="hover:text-gold transition-colors duration-200 border-b-2 border-transparent hover:border-gold pb-1">Inicio</a>
                    <a href="#productos" class="hover:text-gold transition-colors duration-200 border-b-2 border-transparent hover:border-gold pb-1">Tienda</a>
                    <a href="#origen" class="hover:text-gold transition-colors duration-200 border-b-2 border-transparent hover:border-gold pb-1">Origen</a>
                    <a href="#pago" class="hover:text-gold transition-colors duration-200 border-b-2 border-transparent hover:border-gold pb-1">Método de Pago</a>
                </div>
                <!-- Botón de Pedido Rápido -->
                <div class="flex items-center gap-4">
                    <a href="#productos" class="bg-espresso hover:bg-gold text-white hover:text-espresso px-5 py-2.5 rounded-full text-xs font-semibold tracking-wider uppercase transition-all duration-300 shadow-sm flex items-center gap-2">
                        <i class="fa-solid fa-bag-shopping"></i> Comprar Premium
                    </a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Sección de Portada Hero (Inspirada en image_71743e.jpg y usando tu foto real) -->
    <section id="inicio" class="relative bg-forest text-white py-20 lg:py-32 overflow-hidden">
        <!-- Fondo de Naturaleza Amazonas -->
        <div class="absolute inset-0 z-0 opacity-40 mix-blend-multiply bg-cover bg-center" style="background-image: url('https://images.unsplash.com/photo-1516253593875-bd7ba052fbc5?q=80&w=1600&auto=format&fit=crop');"></div>
        <div class="absolute inset-0 bg-gradient-to-r from-espresso via-forest/90 to-transparent z-0"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
            <!-- Textos del Banner -->
            <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                <span class="inline-flex items-center gap-2 bg-gold/20 border border-gold/40 text-gold px-4 py-1.5 rounded-full text-xs font-semibold uppercase tracking-wider">
                    <i class="fa-solid fa-certificate"></i> 100% Gourmet de Lonya Grande
                </span>
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold font-serif leading-tight text-cream">
                    Amazonas Premium WF <br>
                    <span class="text-gold italic font-normal">Directo desde Lonya Grande, Perú</span>
                </h1>
                <p class="text-stone-300 text-sm sm:text-base lg:text-lg max-w-xl mx-auto lg:mx-0 leading-relaxed font-light">
                    Disfruta de un café artesanal selecto de la selva alta, tostado a la perfección con notas dulces, cuerpo denso y un aroma único que transformará tus mañanas.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start pt-2">
                    <a href="#productos" class="bg-gold hover:bg-amber-600 text-espresso hover:text-white font-bold px-8 py-4 rounded-xl transition duration-300 shadow-lg text-center text-sm uppercase tracking-wider flex items-center justify-center gap-2">
                        Ver Ofertas del Menú <i class="fa-solid fa-arrow-down"></i>
                    </a>
                    <a href="#pago" class="bg-white/10 hover:bg-white/20 border border-white/30 text-white font-semibold px-8 py-4 rounded-xl transition duration-300 text-center text-sm flex items-center justify-center gap-2">
                        Pagar con Yape/Plin <i class="fa-solid fa-mobile-screen"></i>
                    </a>
                </div>
            </div>

            <!-- Imagen Destacada del Producto Real (image_a43b9f.jpg) -->
            <div class="lg:col-span-5 flex justify-center">
                <div class="relative max-w-[340px] sm:max-w-[380px] w-full bg-white/5 p-4 rounded-3xl border border-white/10 backdrop-blur-sm shadow-2xl">
                    <div class="rounded-2xl overflow-hidden aspect-[3/4] relative shadow-inner">
                        <!-- Imagen real del producto como presentación principal en el Banner -->
                        <img src="image_a43b9f.jpg" alt="Café Premium Selecto" class="w-full h-full object-cover">
                        <div class="absolute inset-0 bg-gradient-to-t from-espresso via-transparent to-transparent opacity-60"></div>
                        <div class="absolute bottom-4 left-4 right-4 text-left">
                            <p class="text-[10px] text-gold font-bold uppercase tracking-widest mb-1">Empaque de 500gr</p>
                            <h3 class="text-lg font-bold font-serif text-cream">Café Premium Gourmet</h3>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Productos / Packs Especiales -->
    <section id="productos" class="py-20 bg-cream">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-16">
                <span class="text-gold text-xs font-bold tracking-widest uppercase block mb-2">Nuestras Ofertas Especiales</span>
                <h2 class="text-3xl sm:text-4xl font-bold text-espresso font-serif">Elige tu Pack de Café Favorito</h2>
                <div class="w-20 h-1 bg-gold mx-auto mt-4 rounded-full"></div>
                <p class="text-stone-500 text-sm mt-4 leading-relaxed">Disfruta de la mejor calidad artesanal. Compra más bolsas juntas y obtén increíbles descuentos familiares con entrega garantizada.</p>
            </div>

            <!-- Grid de Packs de Productos -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- PRODUCTO 1: Bolsa Sola (S/. 30) -->
                <div class="bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-stone-200/60 flex flex-col justify-between">
                    <div>
                        <!-- Contenedor de Imagen de Bolsa Única con image_a43b9f.jpg -->
                        <div class="h-72 bg-stone-100 relative overflow-hidden flex items-center justify-center p-4">
                            <div class="absolute inset-0 bg-gradient-to-b from-stone-50 to-stone-200/30"></div>
                            <img src="image_a43b9f.jpg" alt="1 Bolsa W&F" class="h-[90%] w-[90%] object-cover rounded-xl shadow-md hover:scale-105 transition duration-300">
                            <span class="absolute top-4 left-4 bg-espresso text-gold text-[10px] font-bold px-3 py-1 rounded-full uppercase tracking-wider">Unidad</span>
                        </div>
                        <div class="p-6 sm:p-8 space-y-3">
                            <div class="flex justify-between items-start">
                                <h3 class="text-xl font-bold text-espresso font-serif">1 Bolsa de Café Gourmet</h3>
                                <span class="bg-stone-100 text-stone-600 text-xs px-2.5 py-1 rounded-md font-semibold">500g</span>
                            </div>
                            <p class="text-stone-500 text-xs leading-relaxed">
                                Un paquete individual de nuestro exclusivo Café Gourmet Premium. Mismo aroma intenso y tostado selecto perfecto para disfrutar de un buen café cada mañana.
                            </p>
                        </div>
                    </div>
                    <div class="p-6 sm:p-8 pt-0 space-y-4">
                        <div class="flex justify-between items-center border-t border-stone-100 pt-4">
                            <span class="text-stone-400 text-xs font-medium">Precio Regular</span>
                            <span class="text-2xl font-bold font-serif text-espresso">S/. 30.00</span>
                        </div>
                        <button onclick="requestProduct('1 Bolsa de Café Gourmet (500g)', '30.00')" class="w-full bg-espresso hover:bg-gold text-white hover:text-espresso font-bold py-3.5 rounded-xl transition duration-300 flex items-center justify-center gap-2 text-xs uppercase tracking-wider shadow-sm">
                            <i class="fa-brands fa-whatsapp text-base"></i> Pedir por WhatsApp
                        </button>
                    </div>
                </div>

                <!-- PRODUCTO 2: Dos Bolsas Juntas (S/. 60) -->
                <div class="bg-white rounded-3xl overflow-hidden shadow-md hover:shadow-2xl transition-all duration-300 border-2 border-gold/40 flex flex-col justify-between relative md:-translate-y-2">
                    <span class="absolute top-4 right-4 z-10 bg-gold text-white text-[10px] font-bold px-3 py-1.5 rounded-full uppercase tracking-widest shadow-md">Dúo Recomendado</span>
                    <div>
                        <!-- Contenedor con efecto de doble bolsa usando image_a43b9f.jpg -->
                        <div class="h-72 bg-stone-100 relative overflow-hidden flex items-center justify-center p-4">
                            <div class="absolute inset-0 bg-gradient-to-b from-stone-50 to-stone-200/30"></div>
                            <!-- Dos bolsas superpuestas artísticamente -->
                            <div class="relative w-[85%] h-[90%]">
                                <img src="image_a43b9f.jpg" alt="Bolsa Izquierda" class="absolute left-2 top-2 h-[90%] w-[75%] object-cover rounded-xl shadow-md rotate-[-6deg] transition duration-300 hover:rotate-0 z-10">
                                <img src="image_a43b9f.jpg" alt="Bolsa Derecha" class="absolute right-2 bottom-2 h-[90%] w-[75%] object-cover rounded-xl shadow-lg rotate-[6deg] transition duration-300 hover:rotate-0 z-20">
                            </div>
                        </div>
                        <div class="p-6 sm:p-8 space-y-3">
                            <div class="flex justify-between items-start">
                                <h3 class="text-xl font-bold text-espresso font-serif">Dúo Pack W&F Aroma</h3>
                                <span class="bg-gold/15 text-gold text-xs px-2.5 py-1 rounded-md font-semibold">1.0 Kg</span>
                            </div>
                            <p class="text-stone-500 text-xs leading-relaxed">
                                Dos empaques completos de nuestro selecto grano de Lonya Grande. Ideal para abastecer tu hogar o regalar una verdadera experiencia cafetera premium.
                            </p>
                        </div>
                    </div>
                    <div class="p-6 sm:p-8 pt-0 space-y-4">
                        <div class="flex justify-between items-center border-t border-stone-100 pt-4">
                            <span class="text-stone-400 text-xs font-medium">Precio por Dúo</span>
                            <span class="text-2xl font-bold font-serif text-espresso">S/. 60.00</span>
                        </div>
                        <button onclick="requestProduct('Dúo Pack W&F (2 Bolsas juntas - 1Kg)', '60.00')" class="w-full bg-gold hover:bg-amber-600 text-white font-bold py-3.5 rounded-xl transition duration-300 flex items-center justify-center gap-2 text-xs uppercase tracking-wider shadow-md">
                            <i class="fa-brands fa-whatsapp text-base"></i> Pedir por WhatsApp
                        </button>
                    </div>
                </div>

                <!-- PRODUCTO 3: Tres Bolsas Juntas (S/. 89) -->
                <div class="bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all duration-300 border border-stone-200/60 flex flex-col justify-between">
                    <div>
                        <!-- Contenedor de Tres Bolsas Juntas utilizando image_a43b9f.jpg -->
                        <div class="h-72 bg-stone-100 relative overflow-hidden flex items-center justify-center p-4">
                            <div class="absolute inset-0 bg-gradient-to-b from-stone-50 to-stone-200/30"></div>
                            <!-- Tres bolsas en abanico tridimensional -->
                            <div class="relative w-[90%] h-[90%] flex items-center justify-center">
                                <img src="image_a43b9f.jpg" alt="Bolsa Fondo Izquierda" class="absolute left-1 h-[80%] w-[60%] object-cover rounded-xl shadow-sm rotate-[-12deg] opacity-90 z-10">
                                <img src="image_a43b9f.jpg" alt="Bolsa Fondo Derecha" class="absolute right-1 h-[80%] w-[60%] object-cover rounded-xl shadow-sm rotate-[12deg] opacity-90 z-10">
                                <img src="image_a43b9f.jpg" alt="Bolsa Frente Centro" class="absolute h-[90%] w-[65%] object-cover rounded-xl shadow-xl z-20">
                            </div>
                            <span class="absolute top-4 left-4 bg-emerald-500 text-white text-[10px] font-bold px-3 py-1 rounded-full uppercase tracking-wider animate-pulse">Súper Ahorro</span>
                        </div>
                        <div class="p-6 sm:p-8 space-y-3">
                            <div class="flex justify-between items-start">
                                <h3 class="text-xl font-bold text-espresso font-serif">Trío Pack Familiar</h3>
                                <span class="bg-emerald-100 text-emerald-800 text-xs px-2.5 py-1 rounded-md font-semibold">1.5 Kg</span>
                            </div>
                            <p class="text-stone-500 text-xs leading-relaxed">
                                Llévate tres bolsas de nuestro exquisito café gourmet y ahorra al máximo. Una excelente opción familiar para nunca quedarte sin el puro aroma de los Andes.
                            </p>
                        </div>
                    </div>
                    <div class="p-6 sm:p-8 pt-0 space-y-4">
                        <div class="flex justify-between items-center border-t border-stone-100 pt-4">
                            <span class="text-stone-400 text-xs font-medium">Precio Especial Trío</span>
                            <div class="text-right">
                                <span class="text-sm line-through text-stone-400 font-mono mr-1">S/. 90</span>
                                <span class="text-2xl font-bold font-serif text-emerald-600">S/. 89.00</span>
                            </div>
                        </div>
                        <button onclick="requestProduct('Trío Pack Familiar (3 Bolsas juntas - 1.5Kg)', '89.00')" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-3.5 rounded-xl transition duration-300 flex items-center justify-center gap-2 text-xs uppercase tracking-wider shadow-sm">
                            <i class="fa-brands fa-whatsapp text-base"></i> Pedir por WhatsApp
                        </button>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Sección Destacada de Métodos de Pago Seguro (Yape/Plin) -->
    <section id="pago" class="py-16 bg-white border-t border-b border-stone-200/50 relative overflow-hidden">
        <div class="absolute right-[-40px] top-[-40px] text-stone-100 pointer-events-none">
            <i class="fa-solid fa-receipt text-[200px]"></i>
        </div>
        <div class="max-w-4xl mx-auto px-4 sm:px-6 relative z-10">
            <div class="bg-gradient-to-br from-espresso to-stone-900 text-white rounded-3xl p-8 sm:p-12 shadow-xl border-l-8 border-gold">
                <div class="grid grid-cols-1 md:grid-cols-12 gap-8 items-center">
                    
                    <!-- Información de Pago -->
                    <div class="md:col-span-7 space-y-4">
                        <span class="text-gold text-xs font-bold uppercase tracking-widest block"><i class="fa-solid fa-lock text-gold mr-1.5"></i> Pago Directo y Seguro</span>
                        <h3 class="text-2xl sm:text-3xl font-serif font-bold text-cream">Cancela al Instante con Yape o Plin</h3>
                        <p class="text-stone-300 text-xs sm:text-sm leading-relaxed">
                            Para agilizar tu entrega, puedes pagar mediante transferencia móvil al mismo número de atención directa. Al finalizar tu pedido por WhatsApp, solo envíanos la captura de tu pago.
                        </p>
                        
                        <!-- Tarjeta con Datos de Pago Directo -->
                        <div class="bg-white/5 border border-white/10 rounded-2xl p-4 sm:p-5 space-y-3">
                            <div class="flex items-center gap-3">
                                <span class="bg-gold/20 text-gold p-2 rounded-lg text-sm"><i class="fa-solid fa-phone"></i></span>
                                <div>
                                    <p class="text-[10px] text-stone-400 uppercase font-semibold">Número de Celular para Yape/Plin</p>
                                    <p class="text-lg font-mono font-bold tracking-wider text-gold">939 801 761</p>
                                </div>
                            </div>
                            <div class="flex items-center gap-3 border-t border-white/5 pt-2">
                                <span class="bg-gold/20 text-gold p-2 rounded-lg text-sm"><i class="fa-solid fa-user"></i></span>
                                <div>
                                    <p class="text-[10px] text-stone-400 uppercase font-semibold">Titular del Servicio</p>
                                    <p class="text-xs font-medium text-cream">W&F Aroma Café</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Botones de Pago Interactivo -->
                    <div class="md:col-span-5 flex flex-col gap-4">
                        <div class="bg-yape/10 border border-yape/30 rounded-2xl p-4 flex items-center justify-between gap-4">
                            <div class="flex items-center gap-2">
                                <span class="w-10 h-10 rounded-xl bg-yape flex items-center justify-center text-white text-lg font-extrabold font-serif">Y</span>
                                <span class="text-sm font-bold text-cream">Pagar con Yape</span>
                            </div>
                            <i class="fa-solid fa-check text-yape"></i>
                        </div>
                        <div class="bg-plin/10 border border-plin/30 rounded-2xl p-4 flex items-center justify-between gap-4">
                            <div class="flex items-center gap-2">
                                <span class="w-10 h-10 rounded-xl bg-plin flex items-center justify-center text-white text-lg font-extrabold font-serif">P</span>
                                <span class="text-sm font-bold text-cream">Pagar con Plin</span>
                            </div>
                            <i class="fa-solid fa-check text-plin"></i>
                        </div>
                        <div class="text-center">
                            <p class="text-[10px] text-stone-400 italic">Precios no incluyen costo de envío a domicilio.</p>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Origen -->
    <section id="origen" class="py-20 bg-cream">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <div class="lg:col-span-5 rounded-3xl overflow-hidden aspect-square relative shadow-lg">
                    <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?q=80&w=600&auto=format&fit=crop" alt="Granos de Café Lonya Grande" class="w-full h-full object-cover">
                </div>
                <div class="lg:col-span-7 space-y-6">
                    <span class="text-gold text-xs font-bold uppercase tracking-widest block">Nuestra Identidad</span>
                    <h2 class="text-3xl sm:text-4xl font-serif font-bold text-espresso">El Secreto de Lonya Grande, Amazonas</h2>
                    <p class="text-stone-600 text-sm sm:text-base leading-relaxed">
                        Nuestro café crece bajo la sombra de frondosos árboles nativos a más de 1600 metros de altitud. La combinación perfecta de suelos húmedos de la selva alta, microclimas únicos de los Andes orientales y un esmero familiar artesanal cosechado grano a grano garantizan un sabor selecto excepcional para paladares refinados.
                    </p>
                    <div class="grid grid-cols-2 gap-4 pt-4">
                        <div class="border-l-4 border-gold pl-4">
                            <h4 class="text-lg font-bold font-serif text-espresso">Altitud Superior</h4>
                            <p class="text-xs text-stone-500 mt-1">Cosechado a más de 1,600 m.s.n.m para un dulzor natural inigualable.</p>
                        </div>
                        <div class="border-l-4 border-gold pl-4">
                            <h4 class="text-lg font-bold font-serif text-espresso">Tueste Medio</h4>
                            <p class="text-xs text-stone-500 mt-1">Preserva todas las notas aromáticas de flores silvestres y cacao.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Pie de Página (Footer) -->
    <footer class="bg-espresso text-cream border-t-4 border-gold py-12 px-4 sm:px-6 lg:px-8 mt-auto">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8 pb-8 border-b border-white/5">
            <div class="space-y-4">
                <span class="text-xl font-bold font-serif tracking-widest text-gold block">W & F AROMA CAFÉ</span>
                <p class="text-xs text-stone-400 leading-relaxed max-w-xs">
                    Café Premium Selecto 100% de origen peruano directo de las fincas ecológicas más prestigiosas de Lonya Grande, Amazonas.
                </p>
            </div>
            <div class="space-y-4">
                <h4 class="text-sm font-semibold tracking-wider text-gold uppercase">Atención Especializada</h4>
                <p class="text-xs text-stone-400 leading-relaxed">
                    <i class="fa-regular fa-clock mr-2 text-gold"></i>Lunes a Domingo: 8:00 AM - 10:00 PM<br>
                    <i class="fa-solid fa-location-dot mr-2 text-gold"></i>Envíos rápidos a todo el Perú
                </p>
            </div>
            <div class="space-y-4">
                <h4 class="text-sm font-semibold tracking-wider text-gold uppercase">Contacto y Soporte</h4>
                <p class="text-xs text-stone-400">
                    ¿Tienes consultas corporativas o compras al por mayor?<br>
                    <a href="https://wa.me/51939801761" class="text-gold font-bold hover:underline block mt-2 text-sm">
                        <i class="fa-solid fa-phone mr-1"></i> +51 939 801 761
                    </a>
                </p>
            </div>
        </div>
        <div class="max-w-7xl mx-auto pt-8 flex flex-col sm:flex-row justify-between items-center gap-4 text-[10px] text-stone-500">
            <p>© 2026 W&F Aroma Café. Todos los derechos reservados. Lonya Grande, Amazonas, Perú.</p>
            <p>Hecho con amor y pasión cafetera ☕</p>
        </div>
    </footer>

    <!-- Botón Flotante Directo de WhatsApp -->
    <a href="https://wa.me/51939801761?text=Hola,%20vengo%20de%20la%20p%C3%A1gina%20web%20y%20quisiera%20pedir%20su%20Caf%C3%A9%20Gourmet%20Premium." target="_blank" class="fixed bottom-6 right-6 bg-emerald-500 hover:bg-emerald-600 text-white w-14 h-14 rounded-full flex items-center justify-center shadow-2xl z-50 transition duration-300 hover:scale-105" title="Chatear con un especialista de café">
        <i class="fa-brands fa-whatsapp text-3xl"></i>
    </a>

    <!-- Script del Negocio -->
    <script>
        function requestProduct(productName, price) {
            const phoneNumber = "51939801761"; 
            const message = `¡Hola W&F Aroma Café! Deseo realizar un pedido:\n\n` +
                            `☕ *Producto:* ${productName}\n` +
                            `💵 *Precio:* S/. ${price}\n\n` +
                            `📱 *Forma de pago:* Realizaré el depósito por Yape o Plin al número 939801761.\n\n` +
                            `Quedo a la espera de sus datos para enviar el comprobante de pago.`;
            
            const encodedMessage = encodeURIComponent(message);
            const whatsappUrl = `https://wa.me/${phoneNumber}?text=${encodedMessage}`;
            
            window.open(whatsappUrl, '_blank');
        }
    </script>

</body>
</html>
