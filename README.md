# Paso a Paso

Aplicación web de acompañamiento para reducir y dejar de fumar. Incluye registro de consumo, metas, disparadores, respiración, acompañamiento y reporte semanal.

## Desarrollo local

1. Instala Node.js 20 o superior.
2. Ejecuta `npm install`.
3. Copia `.env.example` como `.env.local` y agrega tu `GEMINI_API_KEY`.
4. Ejecuta `npm run dev`.

## Publicar en GitHub y Vercel

Sube este directorio a un repositorio GitHub y en Vercel selecciona el framework **Vite**. Vercel detectará el comando `npm run build` y la carpeta `dist`. En Project Settings → Environment Variables agrega `GEMINI_API_KEY` para Production, Preview y Development.

La clave de Gemini se utiliza exclusivamente en `api/ai.js`; no se expone al navegador. La aplicación es de apoyo y no reemplaza atención médica o psicológica profesional.
