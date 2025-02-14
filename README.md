# SanValentin-
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            background-image: url('https://www.xtrafondos.com/wallpapers/rosas-rojas-y-corazones-6566.jpg'); /* Fondo decorado */
            background-size: cover;
            background-position: center;
            text-align: center;
            font-family: Arial, sans-serif;
            color: white;
        }
        .container {
            margin-top: 20%;
            background: rgba(0, 0, 0, 0.6);
            padding: 20px;
            border-radius: 15px;
            display: inline-block;
        }
        h1 {
            font-size: 36px;
        }
        .btn {
            display: inline-block;
            margin: 10px;
            padding: 15px 25px;
            font-size: 20px;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 10px;
            transition: 0.3s;
        }
        .btn-si {
            background-color: red;
        }
        .btn-si:hover {
            background-color: darkred;
        }
        .btn-no {
            background-color: gray;
            position: absolute;
        }
    </style>
    <script>
        function moverBoton() {
            let botonNo = document.getElementById('btnNo');
            botonNo.style.position = "absolute";
            botonNo.style.top = Math.random() * window.innerHeight + "px";
            botonNo.style.left = Math.random() * window.innerWidth + "px";
        }
        function aceptar() {
            alert("¡Sabía que dirías que sí! ❤️");
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>¿Quieres ser mi San Valentín? ❤️</h1>
        <button class="btn btn-si" onclick="aceptar()">Sí</button>
        <button class="btn btn-no" id="btnNo" onmouseover="moverBoton()">No</button>
    </div>
</body>
</html>
