# Curso de Excel Avanzado  🚀

> Domina Excel a nivel profesional: automatiza procesos, transforma datos y crea dashboards interactivos con Power Query, Power Pivot, DAX y VBA. Optimiza tus reportes con modelos de datos dinámicos y automatización avanzada..

| Detalle | Información |
| :--- | :--- |
| **Publicado el** | Publicado el 04 de Dic de 2025 |
| **Profesor** |Daniela Tellez |
| **Fecha de Inicio** | 17/02/2026 |
| **Fecha de Fin** |  |

## Clase 1 - 2: Cómo cargar datos en Power Query Excel

¿Qué es Power Query y cuándo usarlo en Excel?
Power Query es una herramienta de Excel para obtener y transformar datos de forma automática. Es ideal cuando necesitas:

Actualizar información con un clic y evitar procesos manuales repetitivos.
Limpiar datos sucios cada vez que recibes archivos nuevos.
Combinar múltiples archivos en un tablero de control o reporte unificado.
Reemplazar tareas como el cruce de tablas o “buscar mes” con un flujo más rápido y automatizado.
Palabras clave útiles: Power Query, actualizar, limpiar datos, combinar archivos, tablero de control, reporte, obtener y transformar datos.

¿Cómo cargar datos con obtener y transformar datos?
Desde la pestaña Datos en Excel, usa el bloque obtener y transformar datos y el botón obtener datos. Primero trae todo por Power Query (no trabajes directo en las hojas) para habilitar la actualización automática.

Elige la fuente: de un archivo (Excel, texto, CSV) u otras como Oracle, SQL, Azure o SharePoint.
Carga los archivos necesarios: por ejemplo, “base”, “ingresos”, “egresos”, “presupuesto”.
Verifica la vista previa y cuántas filas se cargaron para confirmar que llegó lo correcto.
Si hay cambios, al actualizar verás el nuevo conteo de filas (por ejemplo, de mil uno a tres mil).
¿Cómo importar libros de Excel y distinguir hojas y tablas?
Al traer un libro de Excel, Power Query muestra el nombre del archivo y sus objetos: hojas o tablas. Verás un icono distinto para cada uno. La recomendación es trabajar con tablas, ya que son más robustas para transformar y actualizar. Si un archivo trae “gastos” como tabla y otro como hoja, podrás identificarlo por el icono y elegir la opción correcta antes de cargar.

¿Cómo traer texto y CSV con el delimitador adecuado?
Al importar texto o CSV, Power Query muestra una vista previa y sugiere configuración por default, por ejemplo “Europeo Occidental” y el delimitador. Si tu archivo usa otro separador, cámbialo para mantener el orden correcto. La vista previa se basa en las primeras 200 filas. Puedes acceder a texto/CSV desde obtener datos o desde el acceso directo en Datos: es lo mismo.

Selecciona el delimitador sugerido o ajústalo si tu archivo lo requiere.
Confirma que cada columna se vea como esperas en la vista previa.
Repite el proceso con cada archivo para mantener un flujo homogéneo.
¿Cómo administrar consultas, actualizar y mantener todo automático?
Una vez cargadas las fuentes, podrás gestionar tus consultas desde Power Query.

Usa el icono de actualizar para traer cambios y evitar reprocesos manuales.
Revisa la vista previa y la última actualización: fecha y hora para tener trazabilidad.
Elimina lo que no necesites con clic derecho > eliminar (por ejemplo, “hoja 1”).
Ten en cuenta que Power Query sigue funcionando aunque elimines las hojas en el libro: las consultas existen y puedes unir y transformar datos sin verlos en celdas.

## Clase 3: Panel de Power Query: transformar vs agregar columna