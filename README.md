# Proyecto GitHub Pages · Moto-Mates · versión corregida de reintentos

Esta versión corrige dos cosas importantes:

1. **Nuevo intento real al terminar el ejercicio 6**: al finalizar, la app vacía respuestas y correcciones para empezar desde el ejercicio 1.
2. **Bloqueo de nombre repetido**: conserva en este dispositivo los nombres ya usados, así que para repetir hay que escribir el nombre con número de intento, por ejemplo `DAVID 2`.

## Muy importante

- Esta versión usa una clave nueva de almacenamiento local: `motomates_movimientos_v2_retryfix`.
- Así se evita que el navegador siga cargando estados antiguos donde los ejercicios aparecían ya corregidos.

## Cómo actualizar en GitHub

Sustituye en tu repositorio estos archivos:

- `index.html`
- `moto-mates.png`
- `.nojekyll`
- `README.md`
- `PLANTILLA_EMAILJS.md`
- `PLANTILLA_EMAILJS_EXACTA.md`

## Qué hace el botón "Borrar todo"

Borra:
- respuestas,
- correcciones,
- intento actual,
- y también el historial de nombres usados en ese dispositivo.

## Qué pasa al acabar el ejercicio 6

- se envía el correo final si EmailJS está bien configurado,
- se avisa de que el siguiente intento debe llevar número,
- y se prepara automáticamente un nuevo intento vacío.

## Plantilla de EmailJS

Para que llegue la calificación de los 6 ejercicios, usa la plantilla exacta del archivo:

- `PLANTILLA_EMAILJS_EXACTA.md`

Si en EmailJS sigue apareciendo el texto automático en inglés, el problema está en la plantilla, no en la web.
