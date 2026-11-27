# Amneggsia — sitio del proyecto académico Eggventure

Página de presentación del juego **Amneggsia** (memoria y ritmo en 3D), desarrollada con datos reales del proyecto. Todo el CSS y el JS están embebidos en `index.html`.

## Estructura

```
EggventureWeb/
├── index.html                    ← página completa
├── assets/
│   └── huevos-amneggsia.svg      ← los cuatro huevos con su color y dirección
├── Build/                        ← coloca aquí la exportación WebGL de Unity
│   └── index.html                ← ruta esperada por el iframe
├── GDD.pdf                       ← coloca aquí el GDD final
└── README.md
```

## Tres valores que sí o sí debes completar

1. **Build de Unity:** el iframe apunta a `Build/index.html`. Si tu exportación tiene otra ruta, edita el `src` del comentario `REEMPLAZAR: URL del build de Unity WebGL`.
2. **Tráiler:** en `<!-- AQUÍ PEGA LA URL DEL TRÁILER -->` sustituye `VIDEO_ID` por el ID real del video (30–90 s). También puedes usar `<video src="trailer.mp4" controls>`.
3. **GDD:** el botón apunta a `GDD.pdf`. Coloca el PDF final junto al HTML.

El resto del contenido (mecánica, reglas, dificultades, huevos, escenario, ficha técnica, créditos, recursos y estado) ya está escrito con la información que proporcionaste.

## Contenido incluido

- **Hero:** proyecto Eggventure, juego Amneggsia, género y concepto.
- **Juego:** WebGL 16/9, pantalla completa, fallback de WebGL e instrucciones completas:
  - Juego: flechas o WASD por huevo; P o Escape para pausar.
  - Menús: flechas/WASD para moverse; Enter, Espacio o Enter numérico para confirmar; Escape o Borrar para regresar.
- **Tráiler:** reproductor incrustado y créditos de cierre.
- **GDD:** botón de descarga del PDF.
- **Sobre el juego:** sinopsis, público objetivo (Valeria Mamani, 18), reglas, victoria/derrota, Tierno/Hervido/Quemado, los cuatro huevos, escenario de cocina y ficha técnica.
- **Equipo y créditos:** estudiante, docente, paralelo, gestión, ubicación y fecha.
- **Producción:** recursos propios/externos y lista de componentes integrados, incluidos pose T (rig en Blender) y animaciones con Mixamo.
- **Footer:** créditos académicos y de recursos.

## Paleta

Fondo azul oscuro (`#0E1420`) con superficies `#162132` y acentos pastel: menta `#A7E8D2`, peach `#F3C3A7`, lila `#C8BEF5`, celeste `#A8CFED`, mantequilla `#F2D79A` y coral `#F2A3A3`. Se editan en `:root` al inicio del CSS.

## Prueba local

```bash
python -m http.server 8080
```

Luego abre `http://localhost:8080`. Evita abrir el WebGL directamente con `file://` por las restricciones del navegador.
