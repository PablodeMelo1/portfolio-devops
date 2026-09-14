# Portfolio — Pablo de Melo

Portfolio personal de Pablo de Melo, Software Developer en Telaeris. Presenta su trabajo en automatización de pruebas con Playwright y TypeScript, el proyecto [Blonda Stickers](https://blonda-stickers.vercel.app/) y sus estudios de Analista en Tecnologías de la Información en la Universidad ORT Uruguay.

El sitio está desarrollado con HTML, CSS y JavaScript. Incluye un selector de tema claro/oscuro, pruebas unitarias para esa lógica y configuración para ejecutarlo con nginx en Docker.

## Ejecutar localmente

Con Docker Compose, los cambios en los archivos se reflejan al actualizar el navegador:

```bash
docker compose up
```

Abrí `http://localhost:8080`. Para detenerlo, presioná `Ctrl+C`.

También podés construir la imagen:

```bash
docker build -t portfolio .
docker run --rm -p 8080:80 portfolio
```

O servir los archivos sin Docker:

```bash
python3 -m http.server 8080
```

## Pruebas

```bash
npm install
npm test
```

El contenido del portfolio está en `index.html`, los estilos en `style.css` y la lógica del tema en `theme.js`.
