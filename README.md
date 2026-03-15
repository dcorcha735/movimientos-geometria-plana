# Web HTML para GitHub + EmailJS

## Qué hace
- Presenta los ejercicios 1 al 6 de movimientos en geometría plana.
- Solo muestra un ejercicio cada vez.
- Corrige cada ejercicio al terminarlo.
- Enseña la nota y la solución antes de pasar al siguiente.
- En el ejercicio 6 intenta enviar el resumen final por correo con EmailJS.
- Guarda el progreso en el navegador del dispositivo.

## Archivo principal
- `index.html`

## Qué debes editar
Dentro de `index.html`, busca este bloque:

```js
const EMAILJS_CONFIG = {
  publicKey: 'PON_AQUI_TU_PUBLIC_KEY',
  serviceId: 'PON_AQUI_TU_SERVICE_ID',
  templateId: 'PON_AQUI_TU_TEMPLATE_ID',
  toEmail: 'tu_correo@centro.es',
  teacherName: 'David Cortés Chaparro'
};
```

Sustituye esos valores por los tuyos.

## Variables que conviene usar en la plantilla de EmailJS
En la plantilla puedes usar, por ejemplo:

- `{{to_email}}`
- `{{teacher_name}}`
- `{{student_name}}`
- `{{student_group}}`
- `{{student_email}}`
- `{{score_total}}`
- `{{max_total}}`
- `{{percent_total}}`
- `{{subject}}`
- `{{exercise_summary}}`
- `{{detail_html}}`
- `{{response_json}}`
- `{{timestamp}}`

## Ejemplo sencillo de asunto
```text
{{subject}}
```

## Ejemplo sencillo de cuerpo
```html
<p><strong>Alumno/a:</strong> {{student_name}}</p>
<p><strong>Grupo:</strong> {{student_group}}</p>
<p><strong>Correo del alumno/a:</strong> {{student_email}}</p>
<p><strong>Resultado:</strong> {{score_total}} / {{max_total}} ({{percent_total}}%)</p>
<pre>{{exercise_summary}}</pre>
```

## Para subirlo a GitHub
1. Renombra `index.html` si hace falta, pero lo ideal es dejarlo como `index.html`.
2. Súbelo a tu repositorio.
3. Activa GitHub Pages para ese repositorio.
4. Abre el enlace público y pruébalo desde móvil y ordenador.

## Consejo
Primero prueba con tu propio nombre y completa hasta el ejercicio 6 para verificar que el correo llega bien.


## Configuración ya rellenada

El archivo `index_con_tu_correo.html` ya lleva puesto el correo del profesor: `dcorcha735@g.educaand.es`. Solo falta rellenar `publicKey`, `serviceId` y `templateId` de EmailJS.


## Configuración ya puesta

Este archivo ya lleva estos datos cargados:

- Correo del profesor: `dcorcha735@g.educaand.es`
- Public Key: `WsygDmLij8TCHTJj2`
- Service ID: `service_540t7za`
- Template ID: `template_3df56cg`

## Variables que conviene tener en la plantilla de EmailJS

En tu plantilla de EmailJS, usa estas variables para que el correo salga completo:

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

## Sugerencia de asunto

```
{{subject}}
```

## Sugerencia de cuerpo

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

## Publicación en GitHub Pages

Sube `index_emailjs_configurado.html` al repositorio como `index.html` o renómbralo allí. Después activa GitHub Pages desde la rama principal.
