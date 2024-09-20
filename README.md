<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    Calculadora de Valor de Acciones
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Calculadora de Valor de Acciones (DCF)</h1>
        <form id="calculadora">
            <label for="fcf">Flujo de Caja Libre Inicial (FCF):</label>
            <input type="number" id="fcf" placeholder="Introduce el FCF inicial" required>

            <label for="crecimiento">Tasa de Crecimiento (% anual):</label>
            <input type="number" id="crecimiento" placeholder="Introduce la tasa de crecimiento" required>

            <label for="wacc">Tasa de Descuento (WACC %):</label>
            <input type="number" id="wacc" placeholder="Introduce el WACC" required>

            <label for="años">Años de Proyección:</label>
            <input type="number" id="años" placeholder="Introduce los años de proyección" required>

            <label for="acciones">Número de Acciones en Circulación:</label>
            <input type="number" id="acciones" placeholder="Introduce el número de acciones" required>

            <button type="button" onclick="calcularValor()">Calcular</button>
        </form>

        <div id="resultado">
            <h2>Valor Intrínseco por Acción:</h2>
            <p id="valorAccion"></p>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
