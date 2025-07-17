# Shopify Theme: Shapes Modificado

Este repositorio contiene una versión personalizada del tema **Shapes** para Shopify. Se ha adaptado con estilos, secciones y lógica personalizada para cumplir con los requerimientos del proyecto.

## 🚀 Requisitos

- [Shopify CLI](https://shopify.dev/docs/themes/tools/cli)
- Node.js (v16+ recomendado)
- Cuenta de Shopify con una tienda habilitada para desarrollo

## 📦 Instalación

1. **Clonar el repositorio:**

```bash
git clone https://github.com/joanC0492/tio-saji.git
cd tio-saji
```

2. **Instalar dependencias:**

```bash
npm install
```

3. **Crear el archivo `.env` con tus credenciales:**

```env
SHOPIFY_CLI_THEME_TOKEN=tu_token_privado
SHOPIFY_FLAG_STORE=tu-tienda.myshopify.com
SHOPIFY_THEME_ID=123456789
```

> ⚠️ No compartas este archivo públicamente ni lo subas al repositorio.

4. **Iniciar el servidor de desarrollo:**

```bash
npm run dev
```

Esto abrirá una vista previa del tema y sincronizará los cambios en tiempo real.

## 🧩 Estructura del proyecto

```
.
├── assets/              # Archivos CSS, JS, imágenes, fuentes
├── config/              # settings_data.json y settings_schema.json
├── layout/              # theme.liquid y otros layouts
├── locales/             # Traducciones del tema (ej: es.json)
├── sections/            # Secciones personalizadas
├── snippets/            # Fragmentos reutilizables
├── templates/           # Templates para páginas, productos, etc.
├── .env                 # Variables de entorno para Shopify CLI
├── package.json         # Dependencias del proyecto y scripts CLI
└── README.md
```

## ⚙️ Scripts disponibles

En `package.json` tenés los siguientes scripts listos para usar con `dotenv-cli`:

| Script        | Comando                                       | Descripción                                          |
|---------------|-----------------------------------------------|------------------------------------------------------|
| `dev`         | `npm run dev`                                 | Inicia el servidor local con hot reload              |
| `push`        | `npm run push`                                | Sube el tema a Shopify con el ID indicado            |
| `pull`        | `npm run pull`                                | Descarga cambios desde Shopify al entorno local      |
| `safe-pull`   | `npm run safe-pull`                           | Primero sube cambios, luego hace pull                |
| `list`        | `npm run list`                                | Lista los temas disponibles en la tienda conectada   |

## 🛠 Recomendaciones

- Usá `safe-pull` antes de `pull` para evitar sobrescribir cambios locales.
- Siempre verificá que tu `.env` esté correctamente configurado antes de ejecutar scripts.

## 📚 Recursos útiles

- [Documentación oficial de Shopify CLI](https://shopify.dev/docs/themes/tools/cli)
- [Referencia de Liquid](https://shopify.github.io/liquid/)
- [Guía para personalizar temas](https://shopify.dev/docs/themes)

---

> Este tema está en desarrollo. Si tenés sugerencias o mejoras, ¡hacé un PR o abrí un issue!
