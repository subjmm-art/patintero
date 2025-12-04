<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Patintero - El Juego Tradicional Filipino</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>PATINTERO</h1>
        <p class="subtitle">¡El Desafío Filipino de Correr y Evadir!</p>
    </header>

    <main>
        <section id="introduccion">
            <h2>🇵🇭 Origen e Historia</h2>
            <p>Patintero (también conocido como *Tubigan*) es uno de los juegos al aire libre más populares y queridos en Filipinas. Este juego comunitario, que se practica habitualmente en parques y calles, fomenta la cohesión social, la estrategia y el trabajo en equipo entre distintas generaciones. Aunque sus orígenes exactos son inciertos, ha sido una parte integral del tejido cultural filipino durante décadas.</p>
        </section>

        <section id="campo-simulacion">
            <h2>Diagrama del Campo de Juego</h2>
            <p class="instruccion">El campo es un rectángulo dividido en celdas por líneas que actúan como barreras para los corredores.</p>
            
            <div class="patintero-court">
                <div class="cell start-line">LÍNEA DE INICIO / META</div>
                <div class="cell">CELDA 1</div>
                <div class="cell center-line">GUARDIA CENTRAL</div>
                <div class="cell">CELDA 2</div>
                <div class="cell">CELDA 3</div>
                <div class="cell">CELDA 4</div>
                <div class="cell">CELDA 5</div>
            </div>
            </section>

        <section id="reglas-detalladas">
            <h2>📝 Reglas Detalladas</h2>
            <ol>
                <li>**Equipos:** Se forman dos equipos de 3 a 5 jugadores: **Guardias (Defensores)** y **Corredores (Atacantes)**.</li>
                <li>**Guardias:** Cada Guardia se asigna a una línea. Solo pueden moverse hacia adelante y hacia atrás sobre la línea asignada. ¡No pueden salir de ella!</li>
                <li>**Corredores:** Los Corredores entran al campo de uno en uno, intentando pasar las líneas sin ser tocados.</li>
                <li>**Captura (Taya):** Si un Guardia toca a un Corredor, los equipos inmediatamente **cambian de rol**.</li>
                <li>**Puntuación:** Si un Corredor logra cruzar todas las líneas y regresa a la Línea de Inicio/Meta **sin ser tocado**, su equipo anota un punto.</li>
            </ol>
        </section>
    </main>

    <footer>
        <p>Proyecto Patintero | Desarrollado por un entusiasta de los juegos filipinos.</p>
    </footer>
</body>
</html>/* Estilos Generales y Tipografía */
body {
    font-family: 'Verdana', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f9; /* Fondo muy claro */
    color: #333;
    line-height: 1.6;
}

/* Colores inspirados en Filipinas: Verde, Amarillo y Azul */
header {
    background-color: #004d40; /* Verde oscuro */
    color: white;
    padding: 30px 20px;
    text-align: center;
    border-bottom: 5px solid #ffcc00; /* Amarillo brillante */
}

header h1 {
    font-size: 3.5em;
    margin: 0;
}

main {
    max-width: 800px;
    margin: 30px auto;
    padding: 0 20px;
}

section {
    background-color: white;
    padding: 25px;
    margin-bottom: 25px;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1); /* Sombra suave */
}

section h2 {
    color: #004d40;
    border-bottom: 3px solid #0099cc; /* Azul para el subrayado */
    padding-bottom: 5px;
}

.instruccion {
    font-style: italic;
    color: #555;
    text-align: center;
    margin-bottom: 20px;
}

/* --- ESTILOS DEL CAMPO DE PATINTERO (GRID) --- */
.patintero-court {
    display: grid;
    /* 3 columnas iguales */
    grid-template-columns: repeat(3, 1fr);
    /* 3 filas */
    grid-template-rows: 60px 100px 100px; 
    width: 90%;
    max-width: 500px;
    margin: 20px auto;
    border: 5px solid #333; /* Borde exterior de la cancha */
    box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.2);
}

.cell {
    border: 2px solid #333; /* Líneas del campo */
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 0.8em;
    text-align: center;
    background-color: #d1ffd1; /* Verde muy claro para el césped */
}

/* Líneas Especiales */
.start-line {
    background-color: #007bff; /* Azul vibrante */
    color: white;
    grid-column: 1 / span 3; /* Ocupa las tres columnas en la fila superior */
    border-color: #007bff;
    font-size: 1em;
    letter-spacing: 1px;
}

.center-line {
    background-color: #ffcc00; /* Amarillo */
    color: #333;
    font-weight: bold;
    border-color: #333;
}

/* Estilos para las Reglas */
#reglas-detalladas ol {
    list-style-type: none; 
    padding: 0;
}

#reglas-detalladas li {
    background: #e6f0ff; /* Azul muy claro para las viñetas */
    margin-bottom: 12px;
    padding: 15px;
    border-left: 6px solid #007bff;
    border-radius: 5px;
}

#reglas-detalladas li strong {
    color: #004d40;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: #ccc;
    margin-top: 30px;
    font-size: 0.8em;
}
