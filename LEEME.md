# Cómo publicar felipetamara.com

Este paquete trae un único archivo, `index.html`, con todo el sitio ya
terminado (código, textos, fotos e íconos incluidos dentro del mismo
archivo). No necesita build, no necesita `npm install`, no depende de
ningún otro archivo — así que el despliegue es directo.

## Opción recomendada: subirlo a GitHub y conectarlo en Vercel

1. **Crea un repositorio en GitHub** (puede llamarse `felipetamara-com`),
   o usa uno vacío que ya tengas reservado para este sitio.
2. Sube `index.html` a la raíz de ese repositorio (arrastrar y soltar
   funciona en la web de GitHub, o `git add`, `git commit`, `git push` si
   trabajas desde terminal).
3. Entra a **Vercel → Add New → Project** e importa ese repositorio.
   Como es un archivo estático, Vercel lo detecta solo — no hace falta
   elegir framework ni configurar comando de build (déjalo en "Other" si
   lo pregunta).
4. Dale a **Deploy**. En segundos vas a tener una URL de prueba tipo
   `felipetamara-com.vercel.app` funcionando.
5. Entra a ese proyecto → **Settings → Domains** y agrega
   `felipetamara.com` (y `www.felipetamara.com` si lo quieres también).
   Como el dominio ya está comprado y conectado a tu cuenta de Vercel,
   solo hace falta apuntarlo a este proyecto nuevo — Vercel te avisa si
   hay que mover el dominio desde otro proyecto vacío donde haya quedado
   reservado.

Listo: `felipetamara.com` queda sirviendo este archivo.

## Si prefieres arrastrar y soltar (sin GitHub)

Vercel también permite subir una carpeta directamente sin pasar por
GitHub: **Add New → Project → Deploy** y arrastras la carpeta que
contiene `index.html`. Funciona igual de bien, solo que no queda
historial de cambios en un repositorio — para actualizaciones futuras
tendrías que volver a arrastrar la carpeta completa cada vez.

## Actualizaciones futuras

Cualquier cambio de foto, texto o diseño que hagamos después se entrega
igual: un `index.html` nuevo que reemplaza a este en el repositorio (o
se vuelve a arrastrar), y Vercel republica solo.
