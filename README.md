<!-- buscar_vuelos.php -->
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Búsqueda de Vuelos</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Búsqueda de Vuelos</h1>
    </header>
    <main>
        <form action="resultado_busqueda.php" method="post">
            <label for="origen">Origen:</label>
            <input type="text" id="origen" name="origen" required>
            <label for="destino">Destino:</label>
            <input type="text" id="destino" name="destino" required>
            <label for="fecha">Fecha:</label>
            <input type="date" id="fecha" name="fecha" required>
            <input type="submit" value="Buscar Vuelos">
        </form>
    </main>
</body>
</html>
