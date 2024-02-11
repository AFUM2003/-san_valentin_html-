<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
</head>
<body>
    <h1>¿Quieres ser mi San Valentín?</h1>
    <img src="https://www.andiar.com/1739-large_default/vinilo-oso-corazones.jpg" alt="">
    <button onclick="decidir('SI')">SI</button>
    <button onclick="decidir('NO')">NO</button>

    <div id="respuesta"></div>

    <script>
        var respuestas = [
            "PIENSALO POR FAVOR",
            "MIRA QUE YO TE QUIERO",
            "PORFI, ERES ESPECIAL PARA MI",
            "PIENSALO BIEN",
            "ES QUE QUIERO QUE SEAS TU",
            "YO TE PUEDO DAR MUCHO AMOR",
            "PROMETO TRATARTE COMO PRINCESA",
            "YO LE DOY MI VIDA, AJAJAJAJA",
            "BUENO, ESTA BIEN, YA NO MAS, ELIJE",
            "JAAJJAAJ, LA CREISTE, YA PIENSALO UNA ULTIMA VEZ"
        ];
        var contador = 0;

        function decidir(respuesta) {
            if (respuesta === 'SI') {
                document.getElementById('respuesta').innerHTML = "<p>TE AMO NIÑA BONITA</p>";
            } else if (respuesta === 'NO') {
                if (contador < respuestas.length) {
                    document.getElementById('respuesta').innerHTML = "<p>" + respuestas[contador] + "</p>";
                    contador++;
                } else {
                    document.getElementById('respuesta').innerHTML = "<p>¿Quieres ser mi San Valentín?</p>";
                    contador = 0;
                }
            }
        }
    </script>
</body>
</html>
