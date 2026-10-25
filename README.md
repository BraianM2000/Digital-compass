# Brújula Digital

Recurso educativo multimedia bilingüe (ES/EN) sobre bienestar digital para estudiantes universitarios. Cinco módulos (Atención, Sueño, Movimiento, Redes y Gestión del tiempo), diez pantallas y una interacción en cada una.

## Estructura

```text
/
├── index.html
├── creditos.html
├── README.md
├── assets/
│   ├── app.js
│   ├── styles.css
│   ├── compass.svg, compass-light.svg
│   └── *.svg            (ilustraciones)
└── pages/
    ├── 01-atencion-foco.html
    ├── 02-atencion-notificaciones.html
    ├── 03-sueno-pantalla.html
    ├── 04-sueno-ritual.html
    ├── 05-movimiento-pantalla.html
    ├── 06-movimiento-pausa.html
    ├── 07-redes-conexion.html
    ├── 08-redes-privacidad.html
    ├── 09-organizacion-tiempo.html
    └── 10-organizacion-contrato.html
```

## Uso

Abre `index.html` en un servidor web estático para ejecutar la experiencia completa.

## Criterios de diseño

- **Tipografía única:** se define en `--font` (`assets/styles.css`).
- **Paleta monocromática:** variaciones del morado base `#6849df` (`--purple`, `--purple-dark`, `--purple-mid`, `--purple-soft`, `--purple-tint`) y neutros con matiz morado.
- **Sin emojis** en ilustraciones ni interfaz; los módulos se identifican por nombre, número e ilustración.
- **Bilingüe:** cada texto lleva `data-es` y `data-en`; el idioma se guarda entre visitas.
- **Referencias:** formato autor, año, título y enlace o DOI, igual en las pantallas y en `creditos.html`.

## Cómo agregar o ajustar interacciones

- Control deslizante: `data-range` con `data-range-kind="noise"` o `"movement"` define los mensajes (`setupRange` en `assets/app.js`).
- Cuestionarios, tarjetas, temporizador, lista y contrato: ver las funciones `setup*` de `assets/app.js`.
