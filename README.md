# Dominicanos X El Mundo · Noticias

Este repositorio guarda las noticias que se muestran solas en la página de **Dominicanos X El Mundo** (GoHighLevel → Websites).

- `noticias.json` es el único archivo que lee la página. La tarea diaria lo actualiza cada mañana con notas reescritas a partir de Zabala al Día.
- La nota con `"destacada": true` (la más reciente) va a la portada. Las demás se colocan arriba de su sección (`politica`, `inmigracion`, `economia`, `comunidad`).
- Para quitar una nota, bórrala de la lista `notas` y guarda el archivo. Para corregir un texto, edítalo aquí mismo en GitHub.

## Formato de cada nota

| Campo | Qué es |
|---|---|
| `id` | Identificador único: fecha + palabras del título |
| `fecha` | AAAA-MM-DD |
| `seccion` | `politica`, `inmigracion`, `economia` o `comunidad` |
| `destacada` | `true` solo en la nota de portada |
| `kicker` | Etiqueta corta sobre el título |
| `titulo`, `bajada` | Título y resumen |
| `cuerpo` | Lista de párrafos |
| `autor`, `lugar` | Firma y ciudad |
| `imagen`, `imagen_alt` | Enlace a una foto con permiso de uso (opcional) |
| `fuentes` | Lista de `{nombre, url}` |
