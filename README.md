# primerep-MA
repositorio de vuelos
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agencia de Viajes</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Agencia de Viajes "El viajero confiable"</h1>
    </header>
    <main>
        <section>
            <h2>Agregar Vuelo</h2>
            <form action="agregar_vuelo.php" method="post" onsubmit="return validateFlightForm()">
                <label for="origen">Origen:</label>
                <input type="text" id="origen" name="origen" required>
                <label for="destino">Destino:</label>
                <input type="text" id="destino" name="destino" required>
                <label for="fecha">Fecha:</label>
                <input type="date" id="fecha" name="fecha" required>
                <label for="plazas">Plazas Disponibles:</label>
                <input type="number" id="plazas" name="plazas" required>
                <label for="precio">Precio:</label>
                <input type="number" step="0.01" id="precio" name="precio" required>
                <input type="submit" value="Agregar Vuelo">
            </form>
        </section>

        <section>
            <h2>Agregar Hotel</h2>
            <form action="agregar_hotel.php" method="post" onsubmit="return validateHotelForm()">
                <label for="nombre">Nombre:</label>
                <input type="text" id="nombre" name="nombre" required>
                <label for="ubicacion">Ubicación:</label>
                <input type="text" id="ubicacion" name="ubicacion" required>
                <label for="habitaciones">Habitaciones Disponibles:</label>
                <input type="number" id="habitaciones" name="habitaciones" required>
                <label for="tarifa">Tarifa por Noche:</label>
                <input type="number" step="0.01" id="tarifa" name="tarifa" required>
                <input type="submit" value="Agregar Hotel">
            </form>
        </section>
        <section>
            <h2>Consultas</h2>
            <form action="consulta_disponibilidad.php" method="get">
                <input type="submit" value="Ver Disponibilidad">
            </form>
        </section>

        <section>
            <h2>Carrito de Compras</h2>
            <div class="paquete" id="paquete1">
                <h3>Paquete a París</h3>
                <p>Disfruta de una semana en París, la ciudad del amor.</p>
                <button onclick="addToCart('Paquete a París', 1000)">Añadir al carrito</button>
            </div>
            <div class="paquete" id="paquete2">
                <h3>Paquete a Nueva York</h3>
                <p>Explora la gran manzana durante 5 días.</p>
                <button onclick="addToCart('Paquete a Nueva York', 1200)">Añadir al carrito</button>
            </div>
            <div class="paquete" id="paquete3">
                <h3>Paquete a Tokio</h3>
                <p>Descubre la cultura japonesa en una aventura de 10 días.</p>
                <button onclick="addToCart('Paquete a Tokio', 1500)">Añadir al carrito</button>
            </div>
            <div id="cart">
                <h2>Carrito de Compras</h2>
                <ul id="cart-items">
                    <!-- Items will be dynamically added here -->
                </ul>
                <button onclick="checkout()">Finalizar Compra</button>
            </div>
        </section>
    </main>
    <script src="scripts.js"></script>
    <!-- Pie de página -->
    <footer>
        <p>© El viajero confiable</p>
    </footer>
</body>
</html>
