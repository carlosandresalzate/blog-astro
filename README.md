# # 🚀 Guía práctica: Construcción de un blog usando Astro

## 🎯 Objetivo

Crear un blog estático con [Astro](https://astro.build/) para compartir conocimientos sobre desarrollo, herramientas y proyectos propios.

## 🤔 ¿Por que Astro?

Los dos venimos del mundo Javascript, y tras analizar alternativas como jekyll ( Ruby ), hugo ( Hugo ) y otras soluciones, me parece que la mejor opcion es optar por Astro ya que tiene la compatibilidad que necesitamos con las herramientas que conocemos. Elegimos un stack amigable con JavaScript, aprovechando lo que ya dominamos. 😉

## 🧱 Plan inicial

Antes de crear el blog como tal, debemos establecer ciertos fundamentos clave:

- **¿Miembros fundadores?:** (Solo es un borrador, de ejemplo)

   - 🧑‍💻 ¿? – Rol principal: Frontend/Arquitectura | Secundario: Contenido técnico
   - 🧑‍💻 ¿? – Rol principal: Documentación | Secundario: UI/UX

- **Roles posibles:**
   - Desarrollo
   - Contenido técnico
   - Documentación
   - Diseño UI/UX
      > Nota: los roles al ser solo dos personas pueden ser compartidos.

1. **Primera entrada del blog**
   _Prioridad maxima._ Necesitamos un articulo inicial para tener contenido base y darle idea a la identidad al proyecto.

   > ✍ Tema propuesto: "¿Cual es el tema?"
   > 📄 Formato: Markdown (`.md`)
   > 📂 Ubicacion `/src/content/blog/por-que-usamos-astro.md`
   > 📅 Fecha limite: [Definir fecha].

2. 📚**Estructura tecnica y** _Roadmap_ **con Astro**

### 1. Fundamentos Iniciales (_Siguiendo el camino sugerido por la documentacion oficial_)

- [ ] ¿Que es Astro y por que usarlo?
- [ ] Arquitectura HTML-first y redenring parcial (Arquitectura de islas)
- [ ] Diferencias con Next.js, SvelteKit, Vue/Nuxt, Hugo
- [ ] Cuando usar astro y cuando no

📍 **Recurso oficial:**[Why Astro?](https://docs.astro.build/en/concepts/why-astro/)

### 2. Configuracion del proyecto

- [ ] Crear proyecto: `npm create astro@latest`
- [ ] Elegir plantilla o usar `minimal` (Recomendado para aprender)
- [ ] Entender la estructura del proyecto (archivos, carpetas, convenciones)

📍 **Recurso oficial:**[Instalacion](https://docs.astro.build/en/install-and-setup/#cli-installation-flags)
📍 **Recurso oficial:**[Syntax Highlighting](https://docs.astro.build/en/guides/syntax-highlighting/#setting-a-default-shiki-theme)

> 💡 Recomendacion: Documente cada paso, como si estuviera escribiendo para otros (Eso refuerza el aprendizaje)

### 3. Configuracion

- [ ] `astro.config.mjs`: rutas, basePath, integraciones
- [ ] Agregar `.env` y variables de entorno
- [ ] Configuraciones del editor (VSCode y extensiones recomendadas)
- [ ] Integracion con TypeScript (Lo podemos hacer gradual o mantenerlo en vanilla Javascript)
- [ ] Dev toolbar y live reload

📍 **Recurso oficial:**[Referencia de configuracion](https://docs.astro.build/en/reference/configuration-reference/)
📍 **Recurso oficial:**[Variables de entorno](https://docs.astro.build/en/guides/environment-variables/)

> 🧠 Meta: Sentirte cómodo trabajando con Astro a diario

### 4. Estructura tecnica

- [ ] Componentes en Astro y layouts reutilizables
- [ ] Slots y props, alcance de los estilos
- [ ] Uso de componentes client-side solo donde hace falta (`client:only`, `client:visible`, etc)
- [ ] CSS global vs scoped

📍 **Recurso oficial:**[Componentes en astro](https://docs.astro.build/en/basics/astro-components/)
📍 **Recurso oficial:**[CSS y estilos](https://docs.astro.build/en/guides/styling/)

> ⚙️ Cómo usar componentes Astro .astro, pero también React, Vue o Svelte si querés

### 5. Estilos y diseño

- [ ] Integrar tailwindCSS ⚠Importancia baja solo por saber como se integra
- [ ] Crear un sistema de diseño simple y legible
- [ ] Evitar colores brillantes o estilos recargados ¿⚠ Vale la pena tokenizar los estilos para este proyecto?

📍 **Recurso oficial:**[CSS y estilos](https://docs.astro.build/en/guides/styling/)

### 6. Contenido dinamico con Markdown y MDX

- [ ] Uso de markdown(`.md`) y MDX (`.mdx`)
- [ ] Que es un slug dinamico y para que se usa
- [ ] Contenido y rutas dinamicas (`src/content`, `[slugs].astro` slugs dinamicos)
- [ ] Frontmatter y metadatos (`title`, `date`, `tags`)
- [ ] Paginacion de entradas

📍 **Recurso oficial:**[Markdown](https://docs.astro.build/en/guides/markdown-content/#frontmatter-layout-property)

> 📚 Ideal para un blog

### 7. Integraciones y funcionalidades extra

- [ ] `astro:assets` Optimizacion de imagenes
- [ ] `@astrojs/mdx` para usar JSX dentro de post
- [ ] **Repaso**: Tailwind, Sass o PostCSS
- [ ] RSS feed automatico (@astrojs/rss)
- [ ] Analytics, SEO y metadatos sociales

📍 **Recurso oficial:**[CSS Preprocessors](https://docs.astro.build/en/guides/styling/#css-preprocessors)
📍 **Recurso oficial:**[RSS feed](https://docs.astro.build/en/recipes/rss/)
📍 **Recurso Externo:**[Mejora el seo en astro](https://www.omargaxiola.com/posts/mejora-seo-astro/) (_Contenido basico_)

> 🔌 Agregarle superpoderes al blog (Solo por aprender, la idea es usar lo necesario)

### 8. Deploy y automatizacion

- [ ] Despliegue en Github Pages, Vercel, Netlify, etc
- [ ] CI/CD Automatizacion con Github Actions
- [ ] Scripting para automatizar, compilar o validar

**Avanzado:**

- [ ] Validación de accesibilidad (a11y) para todas las personas
- [ ] Revisión de performance (Lighthouse) por decir una

Notas:

si seguimos esta ruta base, mas nuestro conocimientos deberiamos poder seguir buenas practicas de desarrollo y mantenimiento tales como:

## ✅ Buenas prácticas recomendadas

- Usar una separación clara entre componentes visuales (UI) y lógica del proyecto.
- Mantener una estructura ordenada en carpetas (`/pages`, `/components`, `/layouts`, `/content`).
- Minimizar el uso de JavaScript innecesario (Astro es HTML-first).
- Asegurarse de que el blog funcione sin React o JS (SSR por defecto).
- Documentar cada componente de manera clara.
- Estilos sobrios, sin colores brillantes ni interfaces recargadas.
- Tener en cuenta accesibilidad (a11y) y performance como prioridades desde el inicio.
