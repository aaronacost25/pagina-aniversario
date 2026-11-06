# Aaron & Julieta · 3 años 💜

Página de aniversario con portada, contador en tiempo real desde el **6 de noviembre de 2023**, galería de fotos tipo presentación y **un juego de memoria** con los personajes de BT21. Incluye detalles de BTS: morado y personajes BT21.

## Estructura

1. **Portada** — nombres y fecha.
2. **Contador** — tiempo juntos en vivo.
3. **Galería de fotos** — presentación de a una foto, con flechas, puntos y deslizamiento; se arma sola desde la carpeta `fotos/`.
4. **Memoria BT21** — 8 parejas con los personajes (Koya, RJ, Shooky, Mang, Chimmy, Tata, Cooky y Van), movimientos y tiempo.
5. **Cierre** — dedicatoria y firma.

## Cómo verla

Abre `index.html` con doble clic (Chrome, Edge, Firefox…). No necesita instalar nada.

## Cómo agregar las fotos

1. Copia tus fotos dentro de la carpeta `fotos/`.
2. Renómbralas en orden:

   ```
   1.jpg
   2.jpg
   3.jpg
   ```

   También sirven `.jpeg`, `.png`, `.webp`, `.avif`, `.gif` y `.svg`.
3. Abre `index.html`: la galería las detecta sola.

> Consejo: usa entre 8 y 15 fotos, de menos de 2 MB cada una, y no dejes números saltados.

### Ponerles título (opcional)

Abre `fotos/fotos.js` y descomenta el ejemplo:

```js
window.FOTOS = [
  { archivo: "1.jpg", titulo: "Nuestro primer día" },
  { archivo: "2.jpg", titulo: "Esa tarde de risas" }
];
```

Si lo dejas vacío, la página usa la numeración automática.

## Cómo personalizar

| Qué cambiar | Dónde |
|---|---|
| Fecha del contador | `index.html`, busca `var START = new Date(2023, 10, 6, 0, 0, 0);` (mes 10 = noviembre) |
| Dedicatorias | `index.html`, sección `CIERRE` |
| Nombres y textos | `index.html`, busca el texto y cámbialo |
| Títulos de las fotos | `fotos/fotos.js` |

### Editar el juego de memoria

Los personajes están definidos en `index.html`:

- Busca `var ICONS = [` para cambiar el orden de las parejas.
- Busca `id="bt21-...` para editar los dibujos SVG de cada personaje.

## Cómo compartirla

- **En persona:** llévala en el celular o laptop y ábrela.
- **Por WhatsApp/Drive:** comprime la carpeta completa (con `fotos/` dentro) y envíala. La otra persona solo abre `index.html`.
- **En internet (gratis):** arrastra la carpeta a [Netlify Drop](https://app.netlify.com/drop) o súbela a GitHub Pages. Te queda un enlace para enviarle.

> Las tipografías se descargan de Google Fonts. Sin internet, la página sigue funcionando con tipografías elegantes del sistema.

---

Hecho con cariño para celebrar tres años. Borahae 💜
