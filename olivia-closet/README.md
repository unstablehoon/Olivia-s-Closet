# Olivia’s closet — primera versión

App web en español para un clóset personal y collages, sin dependencias ni servicios de pago. El archivo index.html incluye las cuatro referencias aportadas por Olivia. No son prendas de su inventario.

## Funciona

- Añadir fotos PNG, JPEG y WebP; editar nombre, categoría, color, estado y notas.
- Buscar y filtrar prendas. Solo las disponibles aparecen en el selector del collage.
- Añadir prendas al collage, arrastrar, cambiar tamaño y posición con controles accesibles, traer delante y quitar.
- Guardar y volver a abrir outfits.
- Añadir y anotar referencias, guardar preferencias.
- Guardar datos en IndexedDB del navegador; exportar e importar un respaldo JSON con fotos.
- Prueba real de permiso de micrófono; no graba ni transmite audio.

## Todavía no implementado

- Conversación, análisis de imágenes o recomendaciones con Gemini.
- Sincronización entre dispositivos, cuentas o base de datos alojada.
- Eliminación automática del fondo de fotos, exportación del collage como imagen.
- Importación automática de Pinterest, Canva o redes sociales.

No hay respuestas falsas de IA, claves de API ni conexiones externas dentro de esta versión.

## Abrir

Abre index.html en un navegador moderno. Algunas funciones de almacenamiento dependen del navegador y de cómo se abra el archivo; usa una dirección HTTPS estable para el uso habitual y para probar el micrófono. La compatibilidad con la Huawei concreta todavía requiere una prueba en ese dispositivo. Haz respaldos: los datos no se sincronizan ni viven en GitHub.

## GitHub Pages

1. Sube el contenido de esta carpeta a un repositorio tuyo. No subas respaldos personales ni claves.
2. En Settings → Pages, elige GitHub Actions como fuente de publicación.
3. En Actions, ejecuta manualmente el flujo “Publicar clóset”.
4. Abre la dirección que entregue GitHub Pages.

El flujo no se ejecuta automáticamente al subir cambios. GitHub Pages sirve la interfaz; las fotos añadidas desde la app permanecen en el navegador. Las cuatro referencias iniciales sí están incorporadas al HTML y serán accesibles a quien pueda ver el sitio. Si quieres retirarlas antes de publicar, cambia INITIAL_REFS a [] en index.html.

## Siguiente fase: Gemini

Probar Gemini Live en la tablet y conectar un servicio de emisión de credenciales temporales. La clave permanente debe estar en un servidor protegido, nunca en el HTML, el repositorio o un respaldo. Añadir autenticación, límites de consumo y continuidad de sesiones antes de habilitar voz prolongada. No se ha elegido ni activado facturación.

La lógica de datos y collages es independiente del proveedor de IA. Las funciones WebMCP, si el navegador las admite, exponen lectura de metadatos del clóset y añadir una prenda existente al collage. Esa compatibilidad todavía no se ha validado en un navegador con WebMCP.

## Validación realizada

Comprobación sintáctica del JavaScript y pruebas de validación de respaldos: formato correcto, fotos inválidas, referencias a prendas inexistentes y posiciones fuera de rango. No se ha realizado una prueba visual ni de persistencia en navegador, ni una sesión real de Gemini o prueba de hardware Huawei.
