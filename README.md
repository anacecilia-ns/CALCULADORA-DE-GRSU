<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora de Índice</title>
    <style>
        /* Adicione estilos CSS conforme necessário */
    </style>
</head>
<body>
    <h1>Calculadora de Índice</h1>

    <form id="calculadoraForm">
        <label for="valorA">Valor para A:</label>
        <input type="text" id="valorA" required>

        <label for="valorB">Valor para B:</label>
        <input type="text" id="valorB" required>

        <label for="valorC">Valor para C:</label>
        <input type="text" id="valorC" required>

        <button type="button" onclick="calcularIndice()">Calcular Índice</button>
    </form>

    <p id="resultado"></p>

    <script>
        function calcularIndice() {
            var valorA = parseFloat(document.getElementById('valorA').value);
            var valorB = parseFloat(document.getElementById('valorB').value);
            var valorC = parseFloat(document.getElementById('valorC').value);

            // Adicione a lógica de cálculo aqui
            var indice = (valorA * 0.4) + (valorB * 0.3) + (valorC * 0.3);

            document.getElementById('resultado').innerHTML = "O Índice de Desempenho é: " + indice;
        }
    </script>
</body>
</html>
