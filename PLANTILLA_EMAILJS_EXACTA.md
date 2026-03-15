# Plantilla exacta para EmailJS

El problema no está en la web: está en la plantilla de EmailJS.

Tu captura demuestra que EmailJS está usando todavía una plantilla automática genérica en inglés.
Para que llegue la calificación de los 6 ejercicios, en **EmailJS > Email Templates > template_3df56cg** debes sustituir TODO el contenido por esto.

## Campos de la plantilla

### To Email
```text
{{to_email}}
```

### Subject
```text
{{subject}}
```

### Reply To
```text
{{reply_to}}
```

### From Name
```text
{{from_name}}
```

## Content
Pulsa en el editor de código `<>` y pega exactamente esto:

```html
{{{body_html}}}
```

## Qué hace
La web ya envía un bloque HTML completo con:
- logo Moto-Mates
- Departamento de Matemáticas
- David Cortés Chaparro
- alumno/a y grupo
- nota total
- detalle de los 6 ejercicios

Si pones `{{{body_html}}}`, EmailJS insertará el HTML tal cual.

## Si quieres además una versión en texto
En la parte de texto plano, si tu plantilla la tiene, pega:

```text
{{message}}
```

## Muy importante
No dejes el texto por defecto de EmailJS en inglés.
Si el contenido de la plantilla sigue poniendo algo parecido a:

```text
Thank you for reaching out to us! We have received your request...
```

entonces nunca se verá la calificación, porque esa plantilla no está usando las variables que envía tu página.
