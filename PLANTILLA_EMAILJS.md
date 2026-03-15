# Variables recomendadas para la plantilla de EmailJS

Usa estas variables en tu plantilla:

- `{{subject}}`
- `{{to_email}}`
- `{{teacher_name}}`
- `{{student_name}}`
- `{{student_group}}`
- `{{student_email}}`
- `{{score_total}}`
- `{{max_total}}`
- `{{percent_total}}`
- `{{exercise_summary}}`
- `{{detail_html}}`
- `{{response_json}}`
- `{{timestamp}}`

## Asunto sugerido

```text
{{subject}}
```

## Cuerpo sugerido

```html
<p>Hola {{teacher_name}},</p>
<p>Se ha enviado una nueva entrega del cuestionario de movimientos en geometría plana.</p>
<p><strong>Alumno/a:</strong> {{student_name}}<br>
<strong>Grupo:</strong> {{student_group}}<br>
<strong>Correo:</strong> {{student_email}}<br>
<strong>Resultado:</strong> {{score_total}} / {{max_total}} ({{percent_total}}%)<br>
<strong>Fecha:</strong> {{timestamp}}</p>
{{detail_html}}
<pre>{{exercise_summary}}</pre>
```
