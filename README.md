# primerep-MA
repositorio de vuelos
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Consulta Avanzada</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Consulta Avanzada de Reservas</h1>
    </header>
    <main>
        <section>
            <h2>Reservas Registradas</h2>
            <?php include 'mostrar_reservas.php'; ?>
        </section>
        Paris<br>
         Roma <br>
          Isla de Pascua <br> Nueva york <br> Brasil <br> Florianopolis <br>Tokio <br>Punta cana <br>

        <section>
            <h2>Hoteles con más de 2 Reservas</h2>
            <?php include 'consulta_avanzada.php'; ?>
            Hotel Paquete de Tokio <br>
            Hotel Paquete de Paris 
        </section>
    </main>
</body>
</html>
