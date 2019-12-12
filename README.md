# https://tiiselam.github.io

- PERU	pe01	  PER POP Generación de asiento adicional en la recepción de compras. Incluye costo descargado.
- PERU	pe04		PER GL Localización Perú - Libros sunat, pcge, correcciones menores a loc andina
- PERU	pe06		PER PM detracciones
- GENERAL dgp07 Función genérica para obtener datos de terceros en Report Writer

# Procedimiento de Puesta en producción

Verificar el último cambio realizado en el repositorio local que no fuese propio y compararlo con el último cambio realizado en el repositorio de TII.
Si no son iguales, se debe volver a cargar en el repositorio local la última versión del repositorio de TII. Luego, se pueden rehacer los cambios en el repositorio local y seguir los siguientes pasos:

Caso 1. Modificación de aplicación y/o objetos sql
1. Indicar la versión de la app en el about
2. Instalar en producción
3. Generar el pull request indicando la versión de la app y de objetos sql al lado de la etiqueta release. Ej: v13.0.0-release.5+GP2013...br01
4. Generar release en Github
5. Actualizar el estado de la implementación en el cliente

Caso 2. Modificación sólo de objetos sql
1. Instalar en producción
2. Ejecutar script de versionamiento
3. Generar el pull request indicando la versión del objeto sql al lado de la etiqueta release. Ej: v13.0.0-release.10+GP2013...br01
4. Generar release en Github

