<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Algoritmo de Cajero Automático</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
            background-color: #f4f4f4;
            color: #333;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2 {
            color: #0056b3;
            border-bottom: 2px solid #0056b3;
            padding-bottom: 10px;
        }
        pre {
            background: #f8f9fa;
            border: 1px solid #ddd;
            padding: 15px;
            border-radius: 5px;
            overflow-x: auto;
        }
        .diagram-image {
            max-width: 100%; /* Make the image responsive */
            height: auto;
            display: block; /* Remove extra space below the image */
            margin: 20px auto; /* Add some spacing around the image and center it */
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Algoritmo de Cajero Automático</h1>

        <h2>Pseudocódigo en PSeInt</h2>
        <pre><code>Proceso CajeroAutomatico
    // Declaración de variables
    Definir saldo, retiro Como Real;

    // Asignación de saldo inicial
    saldo &lt;- 500;

    // Solicitar la entrada del usuario
    Escribir "Bienvenido. Su saldo actual es: ", saldo;
    Escribir "Por favor, ingrese el monto que desea retirar:";
    Leer retiro;

    // Estructura de decisión: verifica si hay fondos suficientes
    Si retiro &lt;= saldo Entonces
        // Acciones si el saldo es suficiente
        saldo &lt;- saldo - retiro;
        Escribir "Retire su dinero";
        Escribir "Su nuevo saldo es: ", saldo;
    SiNo
        // Acciones si el saldo es insuficiente
        Escribir "Fondos insuficientes";
    FinSi

    Escribir "Gracias por su visita.";

FinProceso
</code></pre>

        <h2>Diagrama de Flujo (Mermaid)</h2>
        <p>Este es el código que representa la lógica del algoritmo de forma visual. Para visualizarlo, necesitarías una librería de Mermaid o un editor compatible.</p>
        <pre><code>flowchart TD
    INICIO ([Inicio])
    ENTRADA [/Solicitar al usuario el monto a retirar/]
    PROCESO1 [[Definir saldo = 500]]
    DECISION {¿retiro &lt;= saldo?}
    PROCESO2 [[Descontar retiro del saldo]]
    SALIDA1 ["Retire su dinero"]
    SALIDA2 ["Fondos insuficientes"]
    FIN ([Fin])

    INICIO -> PROCESO1 -> ENTRADA
    ENTRADA -> DECISION
    DECISION -- Sí -> PROCESO2 -> SALIDA1 -> FIN
    DECISION -- No -> SALIDA2 -> FIN
</code></pre>

        <h2>Diagrama de Flujo (Imagen)</h2>
        <img src="DIAGRAMA.png" alt="Diagrama de flujo del cajero automático" class="diagram-image">
    </div>

</body>
</html>