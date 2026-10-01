# MediaPipe Task Vision

Experimentos interactivos que reaccionan a tus manos y a tu cuerpo frente a la cámara, en tiempo real y directo en el navegador.

**Demo:** abre la página de GitHub Pages de este repositorio, elige un experimento y permite el acceso a la cámara.

## Experimentos

- **Tela**: pellizca con pulgar e índice una lámina transparente y deforma lo que hay detrás.
- **Agua**: la yema de tu dedo índice toca una superficie de agua; entre más rápido, más oleaje.
- **Auroras**: tus manos encienden auroras boreales sobre un lago congelado.
- **Hombre de arena**: tu cuerpo se cubre de arena tornasol que se desprende al moverte.
- **Plancton**: un mar oscuro de plancton bioluminiscente que se enciende en azul con tu movimiento.
- **Fluido**: tu cuerpo empuja un líquido brillante simulado en tiempo real (Navier-Stokes en la GPU).

## Cómo está hecho

- [MediaPipe Tasks Vision](https://ai.google.dev/edge/mediapipe/solutions/vision) para detectar manos (HandLandmarker) y personas (ImageSegmenter).
- WebGL2 con shaders GLSL escritos a mano para la deformación, el agua, la aurora y las partículas de arena.
- JavaScript puro, sin frameworks ni build: cada experimento es un solo archivo HTML.

## Correr en local

```bash
python3 -m http.server 8080
```

Luego abre `http://localhost:8080`. Funciona mejor en Chrome o Edge.

Hecho por Neo Yzmaya · MAYAM
