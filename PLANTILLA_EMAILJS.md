# Plantilla para EmailJS

Abre tu plantilla `template_3df56cg` y pon estos campos.

## Subject

```text
{{subject}}
```

## To Email

```text
{{to_email}}
```

## Reply-To

```text
{{reply_to}}
```

## From Name

```text
{{student_name}}
```

## Contenido HTML del mensaje

Pega esto en el cuerpo HTML de la plantilla:

```html
<div style="font-family:Arial,Helvetica,sans-serif;background:#f5f7fb;padding:24px;">
  <div style="max-width:760px;margin:0 auto;background:#ffffff;border:1px solid #dbe2ea;border-radius:18px;overflow:hidden;">
    <div style="background:linear-gradient(135deg,#1f4fb2,#3d63d8);padding:22px;color:#fff;">
      <img src="{{logo_url}}" alt="Moto-Mates" style="width:110px;max-width:100%;display:block;margin-bottom:12px;">
      <div style="font-size:20px;font-weight:700;">{{department_name}}</div>
      <div style="font-size:16px;margin-top:4px;">{{teacher_name}}</div>
    </div>

    <div style="padding:22px;">
      <h2 style="margin-top:0;margin-bottom:14px;">{{subject}}</h2>

      <p style="line-height:1.6;margin:0 0 14px;">
        <strong>Alumno/a:</strong> {{student_name}}<br>
        <strong>Grupo:</strong> {{student_group}}<br>
        <strong>Correo del alumno/a:</strong> {{student_email}}<br>
        <strong>Fecha y hora:</strong> {{timestamp}}
      </p>

      <div style="background:#f8fbff;border:1px solid #dbe8f8;border-radius:14px;padding:14px 16px;margin:0 0 16px;">
        <strong>Calificación total:</strong> {{score_total}} / {{max_total}}<br>
        <strong>Porcentaje:</strong> {{percent_total}}%
      </div>

      <h3 style="margin:16px 0 10px;">Detalle de calificaciones</h3>
      <pre style="white-space:pre-wrap;background:#f8fafc;border:1px solid #e2e8f0;border-radius:14px;padding:14px;font-family:Arial,Helvetica,sans-serif;line-height:1.5;">{{exercise_summary}}</pre>

      <p style="margin-top:18px;color:#475569;line-height:1.6;">
        Este correo ha sido generado automáticamente desde la actividad interactiva de Moto-Mates.
      </p>
    </div>
  </div>
</div>
```

## Variables que usa esta plantilla

- `subject`
- `to_email`
- `reply_to`
- `student_name`
- `student_group`
- `student_email`
- `timestamp`
- `score_total`
- `max_total`
- `percent_total`
- `exercise_summary`
- `logo_url`
- `department_name`
- `teacher_name`

