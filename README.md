<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Texto aleatorio</title>
<style>
  body {
    margin: 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #1a1a2e;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    padding: 2rem;
    box-sizing: border-box;
  }
  #texto {
    color: #f1f1f1;
    font-size: clamp(1.5rem, 5vw, 3rem);
    text-align: center;
    max-width: 800px;
    line-height: 1.4;
  }
</style>
</head>
<body>
  <div id="texto"></div>

  <script>
    // Lista de textos posibles: edita, añade o quita los que quieras
    const frases = [
      "El caos es solo orden que aún no hemos entendido.",
      "Hoy es un buen día para intentarlo otra vez.",
      "La química también ocurre entre las personas.",
      "Cada equilibrio esconde una constante por descubrir.",
      "A veces la solución precipita cuando menos lo esperas.",
      "Sigue construyendo, molécula a molécula.",
      "Nada se pierde, todo se transforma... incluso las dudas.",
      "El siguiente paso ya está en tu cabeza, solo falta escribirlo."
    ];

    const indice = Math.floor(Math.random() * frases.length);
    document.getElementById("texto").textContent = frases[indice];
  </script>
</body>
</html>
