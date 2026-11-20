# Dominicanos X El Mundo · Noticias

Este repositorio guarda las noticias que se muestran solas en la página de **Dominicanos X El Mundo** (GoHighLevel → Websites).

- `pagina-ghl.html` es la página completa que se pega en GoHighLevel. Llena la portada, "Lo que debes saber hoy" y cada sección con las notas más recientes de `noticias.json`; si una nota no trae foto, usa la ilustración de su sección.
- `noticias.json` es el único archivo que lee la página. La tarea diaria lo actualiza cada mañana con notas reescritas a partir de Zabala al Día.
- La nota con `"destacada": true` (la más reciente) va a la portada. Las demás se colocan arriba de su sección (`politica`, `inmigracion`, `economia`, `comunidad`, `rd`).
- Para quitar una nota, bórrala de la lista `notas` y guarda el archivo. Para corregir un texto, edítalo aquí mismo en GitHub.

## Formato de cada nota

| Campo | Qué es |
|---|---|
| `id` | Identificador único: fecha + palabras del título |
| `fecha` | AAAA-MM-DD |
| `seccion` | `politica`, `inmigracion`, `economia`, `comunidad` o `rd` (noticias de República Dominicana) |
| `destacada` | `true` solo en la nota de portada |
| `destacada_hasta` | Opcional. Fecha AAAA-MM-DD: la nota es principal solo hasta ese día; después la portada pasa sola a la siguiente |
| `credito_foto` | Opcional. Crédito de las fotos, por ejemplo "Fotos: Hodelpa Hospitality" |
| `galeria` | Opcional. Lista de `{url, alt}` con más fotos para la nota principal (fotos guardadas en `img/`) |
| `kicker` | Etiqueta corta sobre el título |
| `titulo`, `bajada` | Título y resumen |
| `cuerpo` | Lista de párrafos |
| `autor`, `lugar` | Firma y ciudad |
| `imagen`, `imagen_alt` | Foto de la nota (siempre). Se toma de `img/fotos.json` (fotos con licencia libre de Wikimedia Commons) o de la carpeta `img/` |
| `credito_url` | Enlace a la página de la foto en Wikimedia Commons (autor y licencia) |
| `fuentes` | Lista de `{nombre, url}` |
