# Cintatransportadorafabrica

Modelo 3D de una cinta transportadora (4 m largo × 1 m ancho × 0.8 m alto) construido con [Babylon.js](https://www.babylonjs.com/), pensado como pieza reutilizable para una aplicación de simulación.

## Ver la demo

Abre `index.html` en un navegador (o sírvelo con un servidor local, por ejemplo `python3 -m http.server`, y visita la URL indicada). No requiere conexión a internet: Babylon.js está incluido localmente en `vendor/babylon/`.

## Qué incluye

- Banda transportadora modelada como un lazo real alrededor de dos rodillos (perfil tipo "pista de atletismo" extruido), con textura de rayas animada para dar sensación de movimiento.
- Rodillos que giran de forma sincronizada con la velocidad de la banda.
- Bastidor metálico: 4 patas, largueros longitudinales y traviesas transversales.
- Guías laterales para evitar que los objetos se caigan de la banda.
- Cajas de ejemplo que viajan sobre la cinta, para visualizar el flujo de una simulación.
- Panel de control HTML: iniciar/detener la cinta y ajustar la velocidad (m/s).
- Cámara orbital (arrastrar para rotar, rueda para zoom, clic derecho para desplazar).

## Estructura

- `index.html` — escena completa (HTML + CSS + JS de Babylon.js) en un único archivo.
- `vendor/babylon/` — build de Babylon.js (`babylon.js`, `babylonjs.loaders.min.js`) vendorizado localmente.

## Personalizar dimensiones

Las medidas de la cinta se definen en el objeto `CONVEYOR` al inicio del script en `index.html` (`length`, `width`, `topHeight`, `rollerRadius`, etc.), por si se necesita ajustar el tamaño para otra simulación.