# Tailwind CSS 4

Versión: 4.1

## Instalación

### Opción 1 (la más fácil):

Usar la CDN:

```html
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
```

* Extensión: Tailwind CSS IntelliSense
* Extensión: Live Server
* Extensión: vscode-icons

### Opción 2 (SPA)

Usar vite

```bash
npm create vite@latest
```

Instalación de Tailwind CSS:

```bash
npm install tailwindcss @tailwindcss/vite
```

Crear archivo vite.config.js

```javascript
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [tailwindcss()],
})
```

Ejecutar en modo desarrollo:

```bash
npm run dev
```


# Guía de clases de utilidad de Tailwind CSS

## 1. Tipografía
  * text-color:
    * text-{color}-{shade}: text-red-500, text-blue-700, text-green-300
    * text-black, text-white
    * text-current, text-transparent
    * text-inherit
    * text-[#FF0000]
  
  * font-size:
    * text-xs, text-sm, text-base, text-lg, text-xl, text-2xl, text-3xl, text-4xl, text-5xl, text-6xl, text-7xl, text-8xl, text-9xl
    * text-[14px], text-[2rem]
  
  * font-weight:
    * font-thin, font-extralight, font-light, font-normal, font-medium, font-semibold, font-bold, font-extrabold, font-black
    * font-[550]
  
  * font-family:
    * font-sans, font-serif, font-mono
    * font-{nombre-personalizado}
  
  * text-align:
    * text-left, text-center, text-right, text-justify, text-start, text-end
  
  * text-decoration:
    * underline, no-underline, line-through, overline
    * decoration-solid, decoration-double, decoration-dotted, decoration-dashed, decoration-wavy
    * decoration-{color}-{shade}: decoration-red-500
    * decoration-[3px]
  
  * line-height:
    * leading-none, leading-tight, leading-snug, leading-normal, leading-relaxed, leading-loose
    * leading-3, leading-4, leading-5, leading-6
    * leading-[3rem]
  
  * letter-spacing:
    * tracking-tighter, tracking-tight, tracking-normal, tracking-wide, tracking-wider, tracking-widest
    * tracking-[0.2em]
  
  * text-transform:
    * uppercase, lowercase, capitalize, normal-case
  
  * text-overflow:
    * truncate, text-ellipsis, text-clip
  
  * white-space:
    * whitespace-normal, whitespace-nowrap, whitespace-pre, whitespace-pre-line, whitespace-pre-wrap
  
  * word-break:
    * break-normal, break-words, break-all
  
  * vertical-align:
    * align-baseline, align-top, align-middle, align-bottom, align-text-top, align-text-bottom, align-sub, align-super
  
  * font-style:
    * italic, not-italic
  
  * font-variant-numeric:
    * normal-nums, ordinal, slashed-zero, lining-nums, oldstyle-nums, proportional-nums, tabular-nums, diagonal-fractions, stacked-fractions

## 2. Borders:
  * border-width: border, border-*
  * border-radius: rounded
  * border-color: border-color-500
  * border-style: border-dotted
  * outline-width: outline outline-offset-1
  * outline-color: outline-red-500
  * outline-style: outline-dotted
  * outline-offset: outline-offset-1, outline-offset-2, outline-offset-4, outline-offset-[5px]

## 3. Paddings y Margins: (Espaciado)
  * Padding: (espaciado interno, por dentro del borde)
    * p-2, p-3, p-4...
    * px-2, px-3, px-4...
    * py-2, py-3, py-4...
    * pt-2, pt-3, pt-4...
    * pb-2, pb-3, pb-4...
    * pl-2, pl-3, pl-4...
    * pr-2, pr-3, pr-4...
    * ps-2, ps-3, ps-4...
    * pe-2, pe-3, pe-4
    * p-[5px]
  * Margin: (espaciado externo, por fuera del borde)
    * m-2, m-3, m-4...
    * mx-2, mx-3, mx-4...
    * my-2, my-3, my-4...
    * mt-2, mt-3, mt-4...
    * mb-2, mb-3, mb-4...
    * ml-2, ml-3, ml-4...
    * mr-2, mr-3, mr-4...
    * ms-2, ms-3, ms-4...
    * me-2, me-3, me-4...
    * m-[5px]
    * m-auto, mx-auto, my-auto
  * Space between (espaciado entre elementos hijos) (preferible usar gap):
    * space-x-2
    * space-y-2
    * gap-2, gap-3, gap-4...
    * gap-x-2, gap-x-3, gap-x-4...
    * gap-y-2, gap-y-3, gap-y-4...
    * gap-[5px]

## 4. Sizing (Dimensionamiento)
  * Width (Ancho):
    * w-0, w-1, w-2... w-12, w-14, w-16...w-96
    * w-1/2, w-1/3, w-2/3, w-1/4, w-3/4, w-1/5...
    * w-full (100%)
    * w-screen (100vw)
    * w-auto
    * w-min, w-max, w-fit
    * w-[200px], w-[50%]
  
  * Min-Width (Ancho mínimo):
    * min-w-0
    * min-w-full
    * min-w-min, min-w-max, min-w-fit
    * min-w-[100px]
  
  * Max-Width (Ancho máximo):
    * max-w-0, max-w-none
    * max-w-xs, max-w-sm, max-w-md, max-w-lg, max-w-xl, max-w-2xl... max-w-7xl
    * max-w-prose
    * max-w-screen-sm, max-w-screen-md, max-w-screen-lg, max-w-screen-xl, max-w-screen-2xl
    * max-w-full
    * max-w-min, max-w-max, max-w-fit
    * max-w-[500px]
  
  * Height (Alto):
    * h-0, h-1, h-2... h-12, h-14, h-16...h-96
    * h-1/2, h-1/3, h-2/3, h-1/4, h-3/4, h-1/5...
    * h-full (100%)
    * h-screen (100vh)
    * h-svh, h-lvh, h-dvh (variantes de viewport height)
    * h-auto
    * h-min, h-max, h-fit
    * h-[200px], h-[50%]
  
  * Min-Height (Alto mínimo):
    * min-h-0
    * min-h-full
    * min-h-screen
    * min-h-svh, min-h-lvh, min-h-dvh
    * min-h-min, min-h-max, min-h-fit
    * min-h-[100px]
  
  * Max-Height (Alto máximo):
    * max-h-0, max-h-none
    * max-h-full
    * max-h-screen
    * max-h-svh, max-h-lvh, max-h-dvh
    * max-h-min, max-h-max, max-h-fit
    * max-h-[500px]
  
  * Size (Ancho y alto simultáneamente):
    * size-0, size-1, size-2... size-12, size-14, size-16...size-96
    * size-auto
    * size-full
    * size-[32px]

## 5. Backgrounds

### Colores de fondo
* `bg-{color}-{intensidad}`: Colores de fondo (ej: `bg-blue-500`, `bg-red-200`)
* `bg-transparent`: Fondo transparente
* `bg-current`: Fondo con color actual
* `bg-black/50`, `bg-blue-500/75`: Fondo con opacidad (50%, 75%)

### Tamaño de fondo
* `bg-auto`: Tamaño original de la imagen
* `bg-cover`: Cubre todo el contenedor manteniendo proporción
* `bg-contain`: Contiene la imagen completa dentro del elemento

### Posición de fondo
* `bg-center`: Centra la imagen de fondo
* `bg-left`, `bg-right`: Alinea a los lados
* `bg-top`, `bg-bottom`: Alinea arriba o abajo
* `bg-left-top`, `bg-right-bottom`, etc.: Combinaciones de alineación

### Repetición de fondo
* `bg-repeat`: Repite la imagen (por defecto)
* `bg-no-repeat`: No repite la imagen
* `bg-repeat-x`: Repite solo horizontalmente
* `bg-repeat-y`: Repite solo verticalmente

### Fijación de fondo
* `bg-fixed`: Fondo fijo durante el scroll
* `bg-local`: Fondo se desplaza con el contenido
* `bg-scroll`: Fondo se desplaza con la página (por defecto)

### Gradientes
* `bg-gradient-to-r`, `bg-gradient-to-t`: Dirección del gradiente (right, top, etc.)
* `from-{color}-{intensidad}`: Color inicial del gradiente
* `via-{color}-{intensidad}`: Color intermedio
* `to-{color}-{intensidad}`: Color final

## 6. Flexbox

### Activación y dirección
* `flex`: Activa flexbox
* `inline-flex`: Activa flexbox con comportamiento inline
* `flex-row`: Dirección horizontal (por defecto)
* `flex-row-reverse`: Dirección horizontal inversa
* `flex-col`: Dirección vertical (columna)
* `flex-col-reverse`: Dirección vertical inversa

### Envoltura (wrap)
* `flex-wrap`: Permite que los elementos pasen a la siguiente línea
* `flex-nowrap`: Mantiene todos los elementos en una línea (por defecto)
* `flex-wrap-reverse`: Envuelve elementos pero en dirección inversa

### Alineación en el eje principal (justify)
* `justify-start`: Alinea al inicio del contenedor
* `justify-end`: Alinea al final del contenedor
* `justify-center`: Centra elementos horizontalmente
* `justify-between`: Distribuye con espacio máximo entre elementos
* `justify-around`: Distribuye con espacio igual alrededor de cada elemento
* `justify-evenly`: Distribuye con espacio exactamente igual entre elementos

### Alineación en el eje secundario (items)
* `items-start`: Alinea elementos al inicio del eje transversal
* `items-end`: Alinea elementos al final del eje transversal
* `items-center`: Centra elementos verticalmente
* `items-baseline`: Alinea elementos por sus líneas base de texto
* `items-stretch`: Estira elementos para ocupar todo el espacio (por defecto)

### Alineación de múltiples líneas (content)
* `content-start`: Alinea líneas al inicio
* `content-end`: Alinea líneas al final
* `content-center`: Centra líneas
* `content-between`: Distribuye líneas con espacio entre ellas
* `content-around`: Distribuye líneas con espacio alrededor
* `content-evenly`: Distribuye líneas con espacio igual

### Espacio entre elementos (gap)
* `gap-{n}`: Espacio uniforme (ej: `gap-4` = 1rem)
* `gap-x-{n}`: Espacio horizontal
* `gap-y-{n}`: Espacio vertical

### Propiedades de elementos individuales
* `flex-1`: Flex grow 1, flex shrink 1, flex basis 0%
* `flex-auto`: Flex grow 1, flex shrink 1, flex basis auto
* `flex-initial`: Flex grow 0, flex shrink 1, flex basis auto (por defecto)
* `flex-none`: Flex grow 0, flex shrink 0, flex basis auto
* `grow`, `grow-0`: Controla si el elemento crece
* `shrink`, `shrink-0`: Controla si el elemento se encoge
* `basis-{n}`: Define el tamaño base del elemento

### Orden de elementos
* `order-{n}`: Cambia el orden de elementos (ej: `order-1`, `order-last`)
* `order-first`: Coloca el elemento primero
* `order-last`: Coloca el elemento último
* `order-none`: Usa el orden del DOM (por defecto)

### Auto-alineación individual
* `self-auto`: Hereda del contenedor padre
* `self-start`: Alinea al inicio (individualmente)
* `self-end`: Alinea al final (individualmente)
* `self-center`: Centra (individualmente)
* `self-stretch`: Estira para llenar (individualmente)
* `self-baseline`: Alinea a la línea base (individualmente)

## 7. Grid

### Activación Grid
* `grid`: Activa CSS Grid
* `inline-grid`: Activa Grid con comportamiento inline

### Columnas y filas (template)
* `grid-cols-{n}`: Define número de columnas (ej: `grid-cols-3` = 3 columnas)
* `grid-cols-none`: Sin definición de columnas
* `grid-rows-{n}`: Define número de filas (ej: `grid-rows-2` = 2 filas)
* `grid-rows-none`: Sin definición de filas

### Columnas/filas automáticas
* `auto-cols-auto`: Tamaño de columnas automático
* `auto-cols-min`: Tamaño mínimo por contenido
* `auto-cols-max`: Tamaño máximo por contenido
* `auto-cols-fr`: Tamaño de fracción (1fr)
* `auto-rows-auto`, `auto-rows-min`, `auto-rows-max`, `auto-rows-fr`: Análogos para filas

### Flujo de elementos
* `grid-flow-row`: Elementos fluyen por filas (por defecto)
* `grid-flow-col`: Elementos fluyen por columnas
* `grid-flow-dense`: Rellena espacios vacíos automáticamente
* `grid-flow-row-dense`, `grid-flow-col-dense`: Combinaciones

### Espacio entre celdas (gap)
* `gap-{n}`: Espacio uniforme (ej: `gap-4` = 1rem)
* `gap-x-{n}`: Espacio horizontal entre columnas
* `gap-y-{n}`: Espacio vertical entre filas

### Posicionamiento de elementos
* `col-auto`: Posición automática
* `col-span-{n}`: Ocupa n columnas (ej: `col-span-2` = 2 columnas)
* `col-span-full`: Ocupa todas las columnas disponibles
* `col-start-{n}`: Comienza en línea n (ej: `col-start-2`)
* `col-end-{n}`: Termina en línea n (ej: `col-end-4`)
* `row-auto`, `row-span-{n}`, `row-span-full`, `row-start-{n}`, `row-end-{n}`: Análogos para filas

### Alineación de ítems en celdas
* `justify-items-start`: Alinea ítems al inicio de la celda (horizontalmente)
* `justify-items-end`: Alinea ítems al final de la celda
* `justify-items-center`: Centra ítems horizontalmente
* `justify-items-stretch`: Estira ítems para ocupar toda la celda (por defecto)

### Alineación de contenido de grid
* `justify-content-start`: Alinea todo el grid al inicio del contenedor
* `justify-content-end`: Alinea todo el grid al final del contenedor
* `justify-content-center`: Centra todo el grid horizontalmente
* `justify-content-between`: Distribuye columnas con espacio máximo entre ellas
* `justify-content-around`: Distribuye columnas con espacio igual alrededor
* `justify-content-evenly`: Distribuye columnas con espacio exactamente igual

### Alineación vertical en celdas
* `items-start`, `items-end`, `items-center`, `items-stretch`, `items-baseline`: Igual que en Flexbox

### Alineación vertical de todo el grid
* `content-start`, `content-center`, `content-end`, `content-between`, `content-around`, `content-evenly`: Igual que en Flexbox

### Alineación individual (para ítems específicos)
* `justify-self-auto`: Hereda del grid padre
* `justify-self-start`: Alinea al inicio horizontalmente (individualmente)
* `justify-self-end`: Alinea al final horizontalmente (individualmente)
* `justify-self-center`: Centra horizontalmente (individualmente)
* `justify-self-stretch`: Estira horizontalmente (individualmente)
* `self-auto`, `self-start`, `self-end`, `self-center`, `self-stretch`, `self-baseline`: Alineación vertical individual

### Grid responsive
* Todas las clases grid pueden ser prefijadas con breakpoints:
  * `sm:grid-cols-2`: 2 columnas en pantallas pequeñas (640px+)
  * `md:grid-cols-3`: 3 columnas en pantallas medianas (768px+)
  * `lg:grid-cols-4`: 4 columnas en pantallas grandes (1024px+)
  * `xl:grid-cols-6`: 6 columnas en pantallas extra grandes (1280px+)
  * `2xl:grid-cols-8`: 8 columnas en pantallas 2xl (1536px+)

## Equivalencias en el espaciado:

  La base del espaciado en Tailwind es una escala numérica configurable. Por defecto:

*   `0` -> `0px`
*   `px` -> `1px`
*   `0.5` -> `0.125rem` (2px)
*   `1` -> `0.25rem` (4px)
*   `1.5` -> `0.375rem` (6px)
*   `2` -> `0.5rem` (8px)
*   `2.5` -> `0.625rem` (10px)
*   `3` -> `0.75rem` (12px)
*   `3.5` -> `0.875rem` (14px)
*   `4` -> `1rem` (16px)
*   ... y así sucesivamente (5, 6, 7, 8, 9, 10, 11, 12, 14, 16, 20, 24, 28, 32, 36, 40, 44, 48, 52, 56, 60, 64, 72, 80, 96).

Tamaños:

`max-w-xs` (`20rem`), `max-w-sm` (`24rem`), `max-w-md` (`28rem`), `max-w-lg` (`32rem`), `max-w-xl` (`36rem`), `max-w-2xl` (`42rem`), `max-w-3xl` (`48rem`), `max-w-4xl` (`56rem`), `max-w-5xl` (`64rem`), `max-w-6xl` (`72rem`), `max-w-7xl` (`80rem`)


## Responsive

* text-red-500 esto aplica a todas las resolutiones

* sm:text-red-500

* sm:text-red-500 md:text-green-500

## Proyecto final

GitHub Pages

Vercel y con algún framework Angular, React

Heroku

Azure Flexible databases for MySQL

Render 

Supabase

OVH, Scaleway, DigitalOcean, AWS