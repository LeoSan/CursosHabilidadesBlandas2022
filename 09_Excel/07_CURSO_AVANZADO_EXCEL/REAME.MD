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

¿Qué es el editor de Power Query y cómo organizarse?
El editor se abre desde datos > obtener datos > iniciar editor de Power Query. A la izquierda verás las consultas (archivos o tablas que cargas). A la derecha, propiedades y pasos aplicados para renombrar y auditar cada transformación. En la cinta superior están Inicio, Transformar, Agregar columna y Vista; puedes anclar la barra para trabajar con todas las herramientas a la vista.

Panel izquierdo: lista de consultas cargadas.
Panel derecho: propiedades y pasos aplicados con icono de tuerca para editar.
Cinta: Inicio, Transformar, Agregar columna, Vista.
Vista previa: primeras 1000 filas; puede mostrar “La lista puede estar incompleta”.
¿Cómo renombrar y revisar pasos aplicados?
Cambia el nombre desde propiedades o con clic derecho > cambiar nombre.
Revisa cada paso aplicado; usa la tuerca para ajustar parámetros sin rehacer todo.
Ejemplo: si te equivocaste en un divisor (1.16 vs 1.17), edítalo desde la tuerca.
¿Qué significan la vista previa y el origen de datos?
La vista previa acelera el trabajo mostrando una muestra. Afecta solo la visualización, no el resultado final.
En Origen puedes cambiar la ruta del archivo con la tuerca y examinar, sin repetir el proceso de limpieza.
¿Cuándo usar transformar y cuándo agregar columna?
La decisión clave: Transformar modifica la columna existente. Agregar columna crea una nueva basada en otra. La lógica es simple: si el resultado debe sustituir, transforma; si debe convivir, agrega.

¿Cómo calcular IVA y descuentos sin dañar la columna original?
Selecciona la columna monto en gastos.
Ve a Agregar columna > estándar > dividir y escribe 1.16 para obtener monto sin IVA. Renombra la nueva columna.
En ventas, para un precio con descuento, usa Agregar columna > estándar > multiplicar por 0.8.
Observa los pasos aplicados: división insertada, columna agregada, etc.
¿Cómo combinar texto de año y mes sin perder columnas?
El orden de selección importa: primero Año y luego Mes (usa tecla control para selección múltiple).
Si quieres unificar y reemplazar: Transformar > Combinar columna > separador guion.
Si quieres conservar las originales: Agregar columna > Combinar columna.
Renombra el resultado según tu convención.
¿Cómo redondear valores con control?
Si no necesitas columna nueva: Transformar > Redondeo > elige a la alza, a la baja o número de decimales.
Si prefieres mantener el original: Agregar columna > Redondeo.
¿Cómo filtrar, duplicar, referenciar y agrupar datos?
Los filtros, duplicados, referencias y agrupaciones te ayudan a construir consultas reutilizables que preparan la tabla exacta para tu modelo.

¿Cómo filtrar filas por cliente y entender el registro del filtro?
Usa los filtros de columna para excluir, por ejemplo, un cliente específico.
Confirma que se registra el paso Filas filtradas. Puedes abrir la tuerca para editar el criterio.
Recuerda: la vista previa puede ser incompleta, pero el filtro se aplicará al conjunto total.
¿Cuándo duplicar y cuándo crear referencia?
Duplicar: crea una copia independiente de la consulta.
Referencia: crea una nueva consulta basada en otra, un copy paste ligado que hereda cambios de la original (ejemplo: Ventas > Ventas 1).
Útil para ramificar transformaciones sin repetir pasos.
¿Cómo agrupar por cliente y calcular promedio de precio?
Selecciona la columna objetivo y ve a Transformar > Agrupar por.
Modo Básico: agrupa por cliente, Operación: Promedio, Columna: precio.
Modo Uso avanzado: agrega múltiples niveles, nuevas operaciones y recuentos según tus columnas disponibles.
También puedes quitar duplicados cuando sea necesario dentro del flujo de preparación.