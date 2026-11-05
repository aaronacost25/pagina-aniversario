# Aaron & Julieta · 3 años 💜

Página de aniversario con portada, historia, contador en tiempo real desde el **6 de noviembre de 2023**, galería de fotos y **tres juegos interactivos** con una sorpresa final. Incluye detalles de BTS: morado, "Borahae" y referencias en los juegos.

## Estructura

1. **Portada** — nombres, fecha y dedicatoria.
2. **Historia y contador** — relato de estos tres años + contador en vivo.
3. **Galería de fotos** — se arma sola desde la carpeta `fotos/`.
4. **Tres desafíos**:
   - 💞 **¿Cuánto me conocés?** — quiz de 6 preguntas.
   - 🧩 **Memoria** — 8 parejas de cartas con movimientos y tiempo.
   - 🗝️ **Encontrá la sorpresa** — 4 pistas que revelan una carta y un vale final.
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
| Historia y dedicatorias | `index.html`, sección `HISTORIA` y `CIERRE` |
| Preguntas del quiz | `index.html`, busca `var QUIZ = [` |
| Pistas y respuestas | `index.html`, busca `var CLUES = [` |
| Sorpresa final y vale | `index.html`, busca `var SORPRESA = {` |
| Nombres y textos | `index.html`, busca el texto y cámbialo |
| Títulos de las fotos | `fotos/fotos.js` |

### Editar el quiz

Cada pregunta tiene esta forma:

```js
{
  q: "¿Qué día empezamos a escribir nuestra historia?",
  options: ["6 de noviembre de 2023", "14 de febrero de 2023", "6 de diciembre de 2023", "6 de noviembre de 2024"],
  answer: 0, // posición de la respuesta correcta (0 = primera)
  hint: "Una pista opcional."
}
```

Puedes agregar o quitar preguntas: el marcador se ajusta solo.

### Editar las pistas

```js
{
  text: "La pista que va a leer ella.",
  answers: ["bts", "bangtan"], // se aceptan varias formas de escribirla
  hint: "Una ayudita.",
  fragment: "El pedacito de carta que se revela."
}
```

Las respuestas no distinguen mayúsculas ni tildes.

### Editar la sorpresa

```js
var SORPRESA = {
  title: "Te espera una noche nuestra",
  text: "La carta o mensaje que aparece al resolver todo.",
  vale: "Una cita sorpresa"
};
```

Ideal si tienes preparada una sorpresa real: cámbiala por la tuya.

## Cómo compartirla

- **En persona:** llévala en el celular o laptop y ábrela.
- **Por WhatsApp/Drive:** comprime la carpeta completa (con `fotos/` dentro) y envíala. La otra persona solo abre `index.html`.
- **En internet (gratis):** arrastra la carpeta a [Netlify Drop](https://app.netlify.com/drop) o súbela a GitHub Pages. Te queda un enlace para enviarle.

> Las tipografías se descargan de Google Fonts. Sin internet, la página sigue funcionando con tipografías elegantes del sistema.

---

Hecho con cariño para celebrar tres años. Borahae 💜
