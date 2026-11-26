# INIT — Portafolio de Isabel Cock

Este archivo es el contexto permanente del repo. Léelo antes de tocar `index.html`, las imágenes o los textos.

## Qué es este proyecto

Portafolio web de una sola página para **Isabel Cock**, artista visual (animación experimental, pintura, grabado, ilustración). Sustituye al portafolio genérico del taller por una pieza editorial con identidad propia: **NÁCAR / SEÑAL**.

- Repo: `pomme019/pomme019.github.io` (GitHub Pages).
- URL publicada: <https://pomme019.github.io/> (GitHub Pages, 26 nov 2026).
- Es un repo independiente dentro de `Pagina/`. El `AGENTS.md` padre del TFM dice “aquí no hay código”: **eso no aplica dentro de esta carpeta**.
- No hay build, Node, npm ni frameworks. Todo vive en `index.html` (CSS y JS inline) + `imagenes/`.
- Git está instalado en `C:\Program Files\Git\cmd\git.exe`, pero no en PATH; `gh` no está. Se puede commitear/pushear con esa ruta o publicar desde la web de GitHub / Netlify Drop.

## Guía del taller

`Pagina/Guia_alumnado_portafolio_con_IA.docx` pide:

- 5 secciones: **Inicio, Obra, Sobre, CV, Contacto**, con menú fijo.
- 8–20 imágenes de obra; máximo 1600 px de lado largo y menos de 500 KB por imagen.
- Fichas: título, año, técnica, dimensiones y una frase.
- **Statement de 120 palabras** y **bio de 80 palabras**.
- CV artístico ordenado.
- **4 colores**, **2 tipografías de Google Fonts** y **3 adjetivos**.
- Un solo `index.html` con CSS incluido, responsive, accesible y con metadatos.
- Publicación en Netlify Drop o GitHub Pages.
- Entrega final: enlace, **5 prompts clave** y media página de reflexión sobre IA.

## Identidad: NÁCAR / SEÑAL

La web parte de la investigación de Isabel: animación experimental, redes que se ramifican, células, metamorfosis, nácar, color y sinestesia. Formal en la estructura; experimental en la superficie.

- **Paleta:** negro `#08070A`, hueso `#F2EFE6`, violeta `#6C4BFF`, verde ácido `#C6FF3D`. Cian, rosa y naranja solo dentro de las imágenes y los degradados.
- **Tipografías:** `Syne` (títulos) + `DM Sans` (texto).
- **3 adjetivos:** sinestésico, riguroso, luminoso.
- **Motivos:** redes de nodos, líneas dibujadas a mano, grano/scanline sutil, tipografía grande, mucho aire.
- **Movimiento:** red animada en el hero (se desactiva con `prefers-reduced-motion`), flipbook de fotogramas y reproducción de GIF/MP4 como secuencias optimizadas en las fichas de animación.
- **Tono:** sobrio y preciso; nada de “explora la relación entre”, “invita a la reflexión”, degradados morados genéricos ni tarjetas de cristal.

## Estructura del sitio

- **Inicio:** nombre, disciplina, retrato/fotograma y una frase; red animada y marquesina de conceptos.
- **Obra:** 8 piezas en cuadrícula editorial, con ficha y lightbox accesible.
- **Reel:** extracto de *Rotoscopia de la lluvia* en flipbook de 12 fotogramas.
- **Sobre:** statement, bio y disciplinas, con un detalle de obra como imagen.
- **CV:** formación, experiencia, proyectos, habilidades e idiomas; botón de impresión.
- **Contacto:** email, ubicación y footer con crédito de IA.

## Contenido

`CONTENIDO.md` es la fuente de verdad de los textos y las fichas. Si cambias un texto, actualízalo allí y luego en `index.html`.

Estado:

- Statement y bio: borrador escrito, pendiente de aprobación de la artista.
- CV: armado con datos reales del CV; institución y año del Grado pendientes.
- Obras: 8 seleccionadas; títulos, años, técnicas y dimensiones son **títulos de trabajo** hasta que la artista los confirme.
- Instagram: pendiente de facilitar el usuario; el enlace está oculto.
- Exposiciones, premios y residencias: no inventar. Si no hay datos, omitir la sección.

## Assets

Originales (no mover ni renombrar):

- `C:\Users\Juliana\Pictures\Mis cosas\grado\` — GIFs de animación experimental (2023).
- `C:\Users\Juliana\Pictures\Master Granada\1. Materias\2. Medios Audiovisuales II\Trabajos\Final\` — storyboard, color, videos.
- `C:\Users\Juliana\Pictures\Mis cosas\14.PNG`, `IMG_3040.PNG`, `sombras.jpg` — pinturas e ilustración propias.
- `C:\Users\Juliana\Pictures\Mis cosas\2.mp4` — rotoscopia de la lluvia.
- `C:\Users\Juliana\Pictures\Mis cosas\Grabado\` — serie de grabado.
- `C:\Users\Juliana\Pictures\Mis cosas\Animaciones\` — contexto de animación.

Copias optimizadas en `imagenes/`:

| Archivo | Origen | Uso |
|---|---|---|
| `hero.jpg` | `grado/1A.gif`, frame 4 | Hero |
| `obra-01.jpg` | `grado/3.png` | Estudio de manos |
| `obra-02.jpg` | `Mis cosas/14.PNG` | El payaso |
| `obra-03.jpg` | `Mis cosas/2.mp4`, frame 0.8 s | Rotoscopia de la lluvia (fotograma) |
| `obra-04.jpg` | `Grabado/FinalMesa de trabajo 15.jpg` | Figuras sentadas |
| `obra-05.jpg` | `Mis cosas/IMG_3040.PNG` | El laberinto |
| `obra-06.jpg` | `Mis cosas/sombras.jpg` | Sombras |
| `obra-07.jpg` | `grado/1A.gif`, frame 7 | Pintar el tiempo |
| `obra-08.jpg` | `Medios Audiovisuales II/.../story.png` | Investigación visual |
| `motion-pintar-01…16.jpg` | `grado/1A.gif`, frames 0–11 + 4 fundidos suaves | Ficha Pintar el tiempo |
| `rain-01…12.jpg` | `Mis cosas/2.mp4`, frames 0.2/0.5/0.8/1.2/1.8/2.1/2.5/2.8/3.2/5.8/6.2/6.5 s | Flipbook y ficha Rotoscopia |
| `sobre.jpg` | detalle de `grado/3.png` | Sobre |
| `og.jpg` | recorte de `hero.jpg` | Open Graph |

Reglas de imagen: máximo 1600 px de lado largo, JPEG calidad 84–90, menos de 500 KB. No subir originales de varios MB.

## Reglas para agentes

- No inventes títulos, años, técnicas, dimensiones, exposiciones, premios ni instituciones. Si falta un dato, usa `[PENDIENTE]` en `CONTENIDO.md` y un texto neutro en la web.
- No cambies la paleta ni las tipografías sin pedirlo.
- No introduzcas frameworks, build steps, dependencias ni imágenes externas.
- Mantén el HTML semántico, el foco visible, el contraste, los `alt`, el `prefers-reduced-motion` y el lightbox por teclado.
- No muevas los archivos originales de `Pictures`. Solo copias optimizadas a `imagenes/`.
- No publiques el teléfono del CV. Solo email y, cuando exista, Instagram.
- Si añades una obra: optimiza la imagen, añade un `<figure class="work">` con sus `data-*` y actualiza `CONTENIDO.md`.

## Publicar

### GitHub Pages (recomendado)

1. Entrar en <https://github.com/pomme019/pomme019.github.io>.
2. Subir `index.html`, `imagenes/`, `favicon.svg`, `robots.txt` y `sitemap.xml` a la raíz de `main` (Add file → Upload files).
3. En Settings → Pages, comprobar que publica desde `main` / root.
4. Abrir <https://pomme019.github.io/> y verificar en móvil.

### Netlify Drop (plan B)

Arrastrar la carpeta completa `pomme019.github.io` (con `index.html` e `imagenes/`) a <https://app.netlify.com/drop>, reclamar el sitio y guardar el enlace.

## Pendientes

- [ ] Confirmar autoría de El payaso, El laberinto y Sombras.
- [ ] Confirmar año, técnica y dimensiones de las obras nuevas.
- [ ] Facilitar Instagram.
- [ ] Institución y año del Grado en Bellas Artes.
- [ ] Títulos, años, técnicas y dimensiones definitivos.
- [ ] Exposiciones, premios o residencias (si existen).
- [ ] Aprobar statement y bio.
- [ ] Escribir los 5 prompts clave y la reflexión de IA para la entrega.
