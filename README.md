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
