# Alejandro Cabeza — Portfolio & CV

<div align="center">

![Astro](https://img.shields.io/badge/Astro-7.4-BC52EE?logo=astro&logoColor=fff&style=flat)
![TypeScript](https://img.shields.io/badge/TypeScript-6.0-3178C6?logo=typescript&logoColor=fff&style=flat)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat)

**Portafolio web y currículum interactivo / imprimible** desarrollado con [Astro](https://astro.build/) y [TypeScript](https://www.typescriptlang.org/). Diseñado con enfoque minimalista, arquitectura estática ultraligera y datos desacoplados mediante esquemas estructurados ([JSON Resume](https://jsonresume.org/schema/)).

[🌐 Sitio Web](https://alejandrocabezaoficial.dev) • [💼 LinkedIn](https://www.linkedin.com/in/alejandro-cabeza-ab86661bb/) • [🐙 GitHub](https://github.com/devcabeza)

</div>

---

## ⚡ Características

- **Rendimiento y Zero-JS por defecto**: Generación estática pura (SSG) con CSS crítico inyectado para evitar bloqueos de renderizado.
- **Soporte Multi-idioma (i18n)**: Español como ruta raíz (`/`) e Inglés (`/en/`), alimentados por `cv.json` y `cv_english.json`.
- **Paleta de Comandos**: Atajo global (`Cmd/Ctrl + K`) impulsado por [HotKeyPad](https://github.com/jesubohr/hotkeypad) para navegación rápida, redes sociales e impresión directa.
- **Preparado para Impresión (PDF)**: Reglas `@media print` dedicadas que eliminan elementos interactivos para generar un CV físico o PDF de maquetación limpia.
- **Tema Claro / Oscuro**: Detección de preferencia de sistema operativo con persistencia local.

## 🛠️ Stack Tecnológico

| Componente | Tecnología | Propósito |
| :--- | :--- | :--- |
| **Framework** | [Astro](https://astro.build/) | Generación estática, bundling y enrutamiento |
| **Lenguaje** | [TypeScript](https://www.typescriptlang.org/) | Tipado estático y contratos para los esquemas del CV |
| **Tipografía** | [Mona Sans](https://github.com/github/mona-sans) | Tipografía variable servida en local |
| **Paleta UI** | [HotKeyPad](https://github.com/jesubohr/hotkeypad) | Manejo accesible de atajos de teclado |

## 🚀 Inicio Rápido

### Requisitos

- [Node.js](https://nodejs.org/) v22+
- Gestor de paquetes: `pnpm` (recomendado) o `npm`

### Instalación y Desarrollo

1. **Clonar el repositorio:**

   ```bash
   git clone git@github.com:devcabeza/portfolio.git
   cd portfolio
   ```

2. **Instalar dependencias:**

   ```bash
   pnpm install
   ```

3. **Iniciar el servidor local:**

   ```bash
   pnpm dev
   ```

   El sitio estará disponible en [http://localhost:4321](http://localhost:4321).

## 🧞 Comandos Disponibles

| Comando | Descripción |
| :--- | :--- |
| `pnpm dev` | Inicia el entorno de desarrollo con Hot Reload en `localhost:4321`. |
| `pnpm build` | Ejecuta `astro check` (verificación de tipos) y compila los assets para producción en `./dist/`. |
| `pnpm preview` | Previsualiza localmente el build generado en `./dist/`. |

## 📁 Gestión de Contenido

La información del perfil está desacoplada del código fuente:

- **Español (`/`)**: Editar [`cv.json`](cv.json).
- **Inglés (`/en/`)**: Editar [`cv_english.json`](cv_english.json).
- **Textos de UI**: Administrados en [`src/i18n/ui.ts`](src/i18n/ui.ts) y [`src/i18n/index.ts`](src/i18n/index.ts).
- **Fotografía de perfil**: Ubicada en [`public/me.webp`](public/me.webp).

## 📄 Créditos y Licencia

- **Diseño base**: Inspirado en el diseño minimalista de [Bartosz Jarocki](https://github.com/BartoszJarocki/cv) y la plantilla inicial de [midudev](https://github.com/midudev/minimalist-portfolio-json).
- **Licencia**: Distribuido bajo licencia [MIT](LICENSE.txt).
