<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>W&F Aroma Café</title>
    <!-- Iconos FontAwesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --color-principal: #3d2514;
            --color-secundario: #bf9456;
            --color-fondo: #fcfbfa;
            --color-texto: #333333;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--color-fondo);
            color: var(--color-texto);
        }

        /* Barra de Navegación */
        header {
            background-color: #ffffff;
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo-container {
            text-align: center;
        }

        .logo-main {
            font-size: 24px;
            font-weight: bold;
            letter-spacing: 2px;
            color: var(--color-principal);
        }

        .logo-sub {
            font-size: 12px;
            color: var(--color-secundario);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--color-texto);
            font-size: 15px;
            transition: color 0.3s;
        }

        nav ul li a:hover, nav ul li a.active {
            color: var(--color-secundario);
            font-weight: 600;
        }

        .cart-icon {
            font-size: 18px;
            color: var(--color-principal);
            cursor: pointer;
            position: relative;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1507133750040-4a8f57021571?auto=format&fit=crop&q=80&w=1500') no-content center/cover;
            height: 450px;
            display: flex;
            align-items: center;
            padding: 0 10%;
            color: #ffffff;
        }

        .hero-container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .hero-mockup {
            width: 30%;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .mockup-bag {
            background-color: #e6cbac;
            padding: 30px 20px;
            border-radius: 5px;
            box-shadow: 5px 5px 15px rgba(0,0,0,0.3);
            text-align: center;
            color: var(--color-principal);
            width: 180px;
            border: 2px solid #c9a67a;
        }

        .mockup-bag .brand {
            font-size: 28px;
            font-weight: bold;
        }

        .mockup-bag .desc {
            font-size: 10px;
            margin-top: 10px;
            border-top: 1px solid var(--color-principal);
            padding-top: 5px;
        }

        .hero-text {
            width: 65%;
        }

        .hero-text h1 {
            font-size: 38px;
            margin-bottom: 15px;
            font-weight: 500;
        }

        .hero-text p {
            font-size: 16px;
            margin-bottom: 25px;
            opacity: 0.9;
        }

        .btn-premium {
            background-color: #ffffff;
            color: var(--color-principal);
            padding: 12px 25px;
            border: none;
            border-radius: 4px;
            font-weight: bold;
            cursor: pointer;
            text-decoration: none;
            transition: background-color 0.3s;
        }

        .btn-premium:hover {
            background-color: var(--color-secundario);
            color: white;
        }

        /* Productos */
        .main-content {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 5%;
            display: flex;
            gap: 40px;
        }

        .products-section {
            flex: 1;
        }

        .products-section h2 {
            color: var(--color-principal);
            margin-bottom: 30px;
            font-size: 24px;
        }

        .grid-productos {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
            gap: 20px;
        }

        .card-producto {
            background: #ffffff;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .product-img-box {
            background-color: #f7f5f2;
            padding: 20px;
            border-radius: 6px;
            margin-bottom: 15px;
        }

        .product-img-box i {
            font-size: 50px;
            color: var(--color-secundario);
        }

        .card-producto h3 {
            font-size: 15px;
            color: var(--color-texto);
            margin-bottom: 10px;
            min-height: 40px;
        }

        .btn-add {
            background-color: var(--color-principal);
            color: #ffffff;
            border: none;
            padding: 10px;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
            transition: background-color 0.3s;
            font-size: 14px;
        }

        .btn-add:hover {
            background-color: var(--color-secundario);
        }

        /* Info Lateral */
        .info-sidebar {
            width: 350px;
            background: #ffffff;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
            height: fit-content;
        }

        .info-sidebar h3 {
            color: var(--color-principal);
            margin-bottom: 15px;
            border-bottom: 2px solid var(--color-secundario);
            padding-bottom: 5px;
        }

        .info-sidebar p {
            font-size: 14px;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        .info-link {
            color: var(--color-principal);
            text-decoration: none;
            font-weight: bold;
            font-size: 14px;
        }

        .info-link:hover {
            color: var(--color-secundario);
        }

        /* Footer */
        footer {
            background-color: var(--color-principal);
            color: #ffffff;
            padding: 20px 5%;
            text-align: center;
            margin-top: 50px;
        }

        .footer-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            flex-wrap: wrap;
            gap: 15px;
        }

        .social-icons a {
            color: #ffffff;
            margin: 0 10px;
            font-size: 18px;
            transition: color 0.3s;
        }

        .social-icons a:hover {
            color: var(--color-secundario);
        }

        .secure-payment {
            font-size: 13px;
            opacity: 0.8;
        }

        /* Botón Flotante WhatsApp */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #25d366;
            color: white;
            padding: 12px 20px;
            border-radius: 50px;
            box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
            z-index: 1000;
            display: flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
            font-weight: bold;
            font-size: 15px;
        }

        .whatsapp-float:hover {
            background-color: #128c7e;
        }

        /* Carrito flotante de referencia */
        .cart-badge {
            position: absolute;
            top: -8px;
            right: -10px;
            background: red;
            color: white;
            border-radius: 50%;
            padding: 2px 6px;
            font-size: 10px;
        }

        @media (max-width: 768px) {
            .hero-container { flex-direction: column-reverse; text-align: center; }
            .hero-text, .hero-mockup { width: 100%; }
            .hero-mockup { display: none; }
            .main-content { flex-direction: column; }
            .info-sidebar { width: 100%; }
            header { flex-direction: column; gap: 15px; }
        }
    </style>
</head>
<body>

    <!-- Encabezado -->
    <header>
        <div class="logo-container">
            <div class="logo-main">W&F</div>
            <div class="logo-sub">Aroma Café</div>
        </div>
        <nav>
            <ul>
                <li><a href="#" class="active">Inicio</a></li>
                <li><a href="#">Tienda</a></li>
                <li><a href="#">Origen</a></li>
                <li><a href="#">Recetas</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </nav>
        <div class="cart-icon">
            <i class="fa-solid fa-cart-shopping"></i>
            <span class="cart-badge" id="cart-count">0</span>
        </div>
    </header>

    <!-- Héroe -->
    <section class="hero">
        <div class="hero-container">
            <div class="hero-text">
                <h1>Amazonas Premium WF | Directo desde Lonya Grande, Perú</h1>
                <p>Café Gourmet, 100% Peruano. Sabor, Cuerpo y Aroma Inigualables.</p>
                <button class="btn-premium" onclick="agregarAlCarrito('Café de Especialidad')">Comprar Café Premium</button>
            </div>
            <div class="hero-mockup">
                <div class="mockup-bag">
                    <div class="brand">W&F</div>
                    <div class="desc">Aroma Café<br>Amazonas Premium</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contenido Principal -->
    <main class="main-content">
        <!-- Sección Productos -->
        <section class="products-section">
            <h2>Nuestros Cafés de Especialidad</h2>
            <div class="grid-productos">
                <!-- Producto 1 -->
                <div class="card-producto">
                    <div class="product-img-box"><i class="fa-solid fa-mortar-pestle"></i></div>
                    <h3>W&F - Café Molido Premium</h3>
                    <button class="btn-add" onclick="agregarAlCarrito('Café Molido Premium')">Añadir al carrito</button>
                </div>
                <!-- Producto 2 -->
                <div class="card-producto">
                    <div class="product-img-box"><i class="fa-solid fa-seedling"></i></div>
                    <h3>W&F - Café en Grano Entero</h3>
                    <button class="btn-add" onclick="agregarAlCarrito('Café en Grano Entero')">Añadir al carrito</button>
                </div>
                <!-- Producto 3 -->
                <div class="card-producto">
                    <div class="product-img-box"><i class="fa-solid fa-boxes-stacked"></i></div>
                    <h3>Degustación Amazonas Pack</h3>
                    <button class="btn-add" onclick="agregarAlCarrito('Degustación Amazonas Pack')">Añadir al carrito</button>
                </div>
            </div>
        </section>

        <!-- Barra Lateral Informativa -->
        <aside class="info-sidebar">
            <h3>Ingredientes e ingrdientes:</h3>
            <p>W&F - Café Molido Premium, monoocina, amante, W&F - Café café en Grano entero, loute surmeta, chila, coca, sugarme, café, Amazona tuell, onlocinas y aromis, and menoemilzatles ex grano entero.</p>
            <a href="#" class="info-link">Saber más sobre Gran Vilaya →</a>
        </aside>
    </main>

    <!-- Pie de página -->
    <footer>
        <div class="footer-content">
            <div class="social-icons">
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-youtube"></i></a>
            </div>
            <div class="secure-payment">
                <i class="fa-solid fa-lock"></i> Pagara a cor pago de seguro seguro
            </div>
        </div>
    </footer>

    <!-- Botón de WhatsApp Integrado -->
    <a href="#" class="whatsapp-float" id="whatsapp-btn" onclick="enviarPedido(event)">
        <i class="fa-brands fa-whatsapp" style="font-size: 22px;"></i> WhatsApp
    </a>

    <script>
        // Gestión básica del carrito para enviar por WhatsApp
        let carrito = [];
        let contador = 0;

        function agregarAlCarrito(producto) {
            carrito.push(producto);
            contador++;
            document.getElementById('cart-count').innerText = contador;
            alert('¡' + producto + ' añadido correctamente!');
        }

        function enviarPedido(e) {
            e.preventDefault();
            if(carrito.length === 0) {
                alert('El carrito está vacío. Añade algún producto antes de enviar.');
                return;
            }
            
            // Reemplaza con tu número de WhatsApp real (Ejemplo: 51999999999)
            let telefono = "51999999999"; 
            let texto = "Hola W&F Aroma Café, me gustaría realizar un pedido de:\n" + carrito.map(p => "- " + p).join("\n");
            let url = "https://api.whatsapp.com/send?phone=" + telefono + "&text=" + encodeURIComponent(texto);
            
            window.open(url, '_blank');
        }
    </script>
</body>
</html>
