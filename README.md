# Arreglo de calificaciones en EmailJS

## Qué está pasando
El correo sí se envía, pero el contenido que llega es el de una plantilla genérica de EmailJS.
Por eso no aparecen ni las notas ni el resumen de los 6 ejercicios.

## Solución
1. Entra en EmailJS.
2. Abre la plantilla `template_3df56cg`.
3. Cambia los campos así:
   - To Email: `{{to_email}}`
   - Subject: `{{subject}}`
   - Reply To: `{{reply_to}}`
   - From Name: `{{from_name}}`
4. En el contenido HTML pega exactamente:

```html
{{{body_html}}}
```

5. Guarda la plantilla.
6. Vuelve a probar el ejercicio 6.

## URL del logo
El proyecto ya usa esta URL pública del logo:

```text
https://dcorcha735.github.io/movimientos-geometria-plana/moto-mates.png
```

## Resultado esperado
El email debe llegar con:
- logo Moto-Mates en cabecera
- Departamento de Matemáticas
- David Cortés Chaparro
- alumno/a, grupo y correo
- nota total
- porcentaje
- detalle de los 6 ejercicios
