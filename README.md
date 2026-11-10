# Avisos de OmniSales

La campana de OmniSales consulta `announcements.json` cuando se abre la app, al volver a ella y al abrir o refrescar la bandeja. GitHub Pages publica los cambios guardados en la rama `main`.

Para publicar un aviso, agrega un objeto al principio del arreglo. Usa un identificador nuevo y estable por aviso. Los dispositivos guardan ese identificador al leerlo.

```json
[
  {
    "id": "mejora-inventario-2026-11",
    "translations": {
      "es": {
        "title": "Mejoras en el inventario",
        "body": "Consulta el avance y el resultado al importar productos y fotos."
      },
      "en": {
        "title": "Inventory improvements",
        "body": "Track progress and review the result when importing items and photos."
      }
    }
  }
]
```

Idiomas admitidos en los avisos: `es`, `en`, `pt`, `fr`, `it`, `de`, `ja`. La app busca primero el idioma de la empresa, luego inglés y después español. El canal admite hasta 50 avisos y debe pesar menos de 128 KB. El ejemplo de arriba describe el formato.

El contenido es público. Publica solo mensajes destinados a todos los usuarios de OmniSales.
