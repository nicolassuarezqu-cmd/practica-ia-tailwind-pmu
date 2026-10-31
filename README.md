# Diana Quintero PMU Studio & Barbería

Landing page para un estudio de barbería y micropigmentación en Neiva, Huila. Trabajo individual de Ingeniería de Software (FET): investigación y desarrollo de un sitio web con Tailwind CSS e inteligencia artificial.

**Sitio publicado:** https://nicolassuarezqu-cmd.github.io/practica-ia-tailwind-pmu/

## Descripción
- **Temática:** barbería (corte de cabello, corte de barba, afeitado) y micropigmentación (microblading, eyeliner, lip blush, scalp micropigmentation).
- **Público objetivo:** hombres y mujeres de 18 a 45 años.
- **Propósito:** mostrar los servicios y recibir solicitudes de cita.

## Tecnologías
HTML, Tailwind CSS 4 (Play CDN) y JavaScript puro, sin otras librerías.

## Paleta (regla 60-30-10) y fuentes
- 60 %: negro #121212 · 30 %: crema #F5EDE3 · 10 %: dorado #C8955A
- Éxito #22B573 · Error #E5484D · Advertencia #F5A524
- Fuentes: Playfair Display (títulos) e Inter (textos)

## Funcionalidades
Navbar con menú hamburguesa, modo claro y oscuro, filtro de servicios, preguntas frecuentes en acordeón, formulario con validación y toast de confirmación.

## Bitácora de prompts
| # | Prompt de ajuste enviado | Problema que buscaba resolver | Resultado obtenido | ¿Funcionó? |
|---|---|---|---|---|
| 1 | "Corrige la ortografía en español de todos los textos visibles, agregando tildes y signos de apertura ¿ ¡, sin cambiar el diseño" | Faltaban tildes ("intencion", "atencion", "micropigmentacion") | Corrigió tildes y signos de apertura en textos, preguntas, etiquetas y mensajes del formulario (18 pasos, 3 min) | Sí |
| 2 | "Hay una tarjeta sola en otra fila. Se puede pasar a 2 columnas, o a 4 en pantallas grandes" | La tarjeta de Scalp micropigmentation quedaba huérfana | El grid pasó a 4 columnas en escritorio | Sí |
| 3 | "La imagen de Nosotros sobresale a la izquierda del contenedor… alinéala con el mismo ancho máximo" | La imagen de "Nosotros" se salía del margen | Copilot dijo que la alineó, pero la foto seguía recortada | Parcial |
| 4 | "Las imágenes de micropigmentación no corresponden… reemplázalas por fotos del collage que te subí" | Fotos de maquillaje y de una mujer con sombrero en vez de cada servicio | Copilot pidió las fotos como archivos individuales porque no podía extraerlas del collage | No a la primera |
| 5 | "Crea una función hoyLocal()… úsala en la validación y en el atributo min" | La fecha de hoy se rechazaba después de las 7 p. m. (UTC) | Creó hoyLocal() y la usa en la validación y en min (30 pasos, 6 min) | Sí |
| 6 | "Simplifica el filtro: solo cambie aria-pressed y define el estilo activo en CSS" | El botón activo quedaba ilegible en modo oscuro y se perdía al pasar el mouse | El filtro solo actualiza aria-pressed y el estado activo se define en CSS | Sí |
| 7 | "Agrega el logo oficial en navbar, footer y favicon" | El sitio no tenía el logo del negocio | Agregó el logo en la navbar y el footer, recortado en círculo (9 pasos, 53 s) | Sí |

## Cambios manuales (sin IA)
1. (cambio 1)
2. (cambio 2)
3. (cambio 3)

## Nota de uso de IA
Usé GitHub Copilot (agente en Visual Studio Code) para generar y ajustar el código, y Claude como apoyo para planificar, revisar el código y preparar los prompts. Revisé y probé el resultado y realicé tres cambios manuales sin IA.

## Imágenes
- **Hero (img/hero.jpg):** generada con ChatGPT.
- **Logo (img/logo.jpg):** logo oficial del negocio, usado con permiso de su dueña.
- **Fotos de servicios:** imágenes de Unsplash (https://unsplash.com), agregadas por Copilot. Licencia de Unsplash: uso libre.
