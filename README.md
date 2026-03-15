# Proyecto Moto-Mates · Movimientos en geometría plana

Esta versión incluye:

- ejercicios 1 al 6 en una sola web para GitHub Pages
- retroalimentación inmediata al terminar cada ejercicio
- indicación del punto inicial y del orden cuando el ejercicio es ordenado
- envío final por EmailJS con calificaciones en el cuerpo del correo
- cabecera del correo con la imagen de Moto-Mates
- nombre del profesor debajo de `Departamento de Matemáticas`
- reinicio automático al terminar para preparar un nuevo intento
- bloqueo si se intenta repetir exactamente el mismo nombre

## Archivos

- `index.html` → web principal
- `moto-mates.png` → logo para la web y para el correo
- `.nojekyll` → recomendado para GitHub Pages
- `PLANTILLA_EMAILJS.md` → texto exacto para pegar en tu plantilla de EmailJS

## Subida a GitHub

1. Entra en tu repositorio.
2. Pulsa **Add file** o **uploading an existing file**.
3. Sube `index.html`, `moto-mates.png`, `.nojekyll` y este `README.md`.
4. Haz **Commit changes**.
5. En **Settings > Pages** deja:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/(root)`

## URL esperada del sitio

Si el repositorio se llama `movimientos-geometria-plana`, la web pública será:

`https://dcorcha735.github.io/movimientos-geometria-plana/`

## Muy importante en EmailJS

Debes abrir la plantilla `template_3df56cg` y sustituir el contenido por la plantilla del archivo `PLANTILLA_EMAILJS.md`.

Si no cambias la plantilla, seguirá llegando el correo genérico de prueba.

## Variables ya configuradas en el proyecto

- Public Key: `WsygDmLij8TCHTJj2`
- Service ID: `service_540t7za`
- Template ID: `template_3df56cg`
- Correo del profesor: `dcorcha735@g.educaand.es`

## Cómo funciona el nuevo intento

Al terminar el ejercicio 6:

- se intenta enviar el correo final
- se guarda el nombre usado en ese intento
- la app se reinicia para otro intento completo
- el siguiente alumno debe escribir el nombre con número al final si repite, por ejemplo `DAVID 2`

Si se vuelve a escribir exactamente el mismo nombre, la app no deja corregir.
