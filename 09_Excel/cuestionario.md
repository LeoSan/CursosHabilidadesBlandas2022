1.
¿Cuál de las siguientes afirmaciones es cierta para las funciones pero no para las subrutinas?
Tiene un valor de retorno.
2.
¿Cuál es la sintaxis correcta de una función?
Public/Private - Function - Nombre - (parámetros) - as Tipo de dato

3.
¿Qué es Message Box?
Es una función que muestra un mensaje en un cuadro de diálogo.
4.
Hablando de Input Box, ¿Cuál de las siguientes afirmaciones es falsa?

Se escribe Input.Box
5.
¿Cuándo utilizarías Ciclos For - Next?

Cuando se busca repetir una instrucción un número específico de veces.

6.
¿A dónde iremos para eliminar errores de cálculo de nuestra base de datos?
F5 -> Especial -> Celdas con fórmulas -> Errores

7.
¿Cómo podemos prevenir la realización de errores al llenar una tabla?
Listas de validación
8.
¿Cuántas condiciones podemos poner a la fórmula CONTAR.SI?

1 condición

9.
¿Cuántas condiciones podemos poner a la fórmula CONTAR.SI.CONJUNTO?
Más de 1 condición
10.
¿Para qué sirve la segmentación de datos?
Crear botones interactivos para filtrar datos.
11.
En el formato condicional. ¿Qué formato nos permite agregar un tono diferente dependiendo del valor que contenga una celda a una lista de datos?

Escala de color
12.
Tomando como base los principios de 'prompt engineering' explicados en la clase, ¿cuál de los siguientes prompts sería el más efectivo para que un estudiante analice su presupuesto y busque ahorrar para un viaje de 25,000 MXN en 4 meses?
Analiza mi presupuesto adjunto. Mi meta es ahorrar 25,000 en 4 meses. Identifica patrones, sugiere reducciones y crea un plan mensual. Estructura tu respuesta en: Resumen, Oportunidades de Ahorro y Plan Mensual.


13.
Un gerente de contabilidad quiere asegurarse de que sus empleados solo puedan ingresar "Fijo" o "Variable" en la columna "Tipo de Gasto", bloqueando completamente cualquier otro valor para mantener la integridad de los datos. ¿Qué estilo de mensaje de error debe configurar en la Validación de datos para lograr este objetivo?
Información
**REPASAR**

14.
¿Cuál es la principal restricción de la función BUSCARV que la función BUSCARX soluciona de manera nativa?
No puede devolver valores de columnas ubicadas a la izquierda de la columna de búsqueda.
15.
Si utilizas la fórmula =BUSCARV(A2, H5:J50, 2, 0), ¿qué representa el número '2' en esta sintaxis específica?
La segunda columna del rango H5:J50, que corresponde a la columna I.


16.
Si un informe de Excel es demasiado ancho para caber en una página al imprimirlo en orientación vertical, ¿cuál sería la combinación de ajustes más eficaz para presentarlo correctamente sin perder información?
Utilizar la vista 'Ver saltos de página' para arrastrar manualmente el límite de la página hacia la derecha.
**REPASAR**

17.
Un analista de ventas ha organizado los datos de sus tiendas en pestañas separadas, una para cada mes del año. Según los principios de estructuración de datos vistos en clase, ¿qué problema principal enfrentará al intentar calcular las ventas totales del trimestre?
Tendrá dificultades para consolidar y sumar la información de todas las pestañas de manera eficiente.
18.
¿Cuál es el principal indicador visual en la interfaz de Excel que confirma que un rango de datos se ha convertido correctamente a formato de tabla?
La aparición de la pestaña contextual 'Diseño de tabla' al seleccionar cualquier celda dentro del rango.

19.
Camila quiere crear una alerta que identifique cualquier gasto clasificado como 'prescindible' O como 'imprevisto' para marcarlo como 'Recortar gasto'. Si ninguna de estas dos condiciones se cumple, debe marcarse como 'Ok'. ¿Qué fórmula anidada debe usar para lograr esto correctamente?
SI(Y(A2="prescindible"; B2="imprevisto"); "Recortar gasto"; "Ok")
**REPASAR**


20.
Estás presentando un dashboard de ventas en una reunión y un director te pide ver el rendimiento combinado de las regiones 'Norte' y 'Este' inmediatamente. ¿Cuál es el método más eficiente para mostrar esta información utilizando un segmentador de datos ya existente?
Hacer clic en 'Norte' y, manteniendo presionada la tecla Ctrl, hacer clic en 'Este'.
21.
¿Qué función cumple un segmentador al ser configurado como un 'control maestro' en un dashboard?
Controla y actualiza simultáneamente múltiples elementos del dashboard, como varias tablas y gráficos.
22.
Has creado un dashboard con una tabla dinámica de ventas por producto y un gráfico dinámico de ventas por región. ¿Cómo puedes configurar el dashboard para que un solo segmentador de 'Año' actúe como un 'control maestro' que filtre ambos elementos simultáneamente?
Haciendo clic derecho en el segmentador de 'Año' y usando la opción 'Conexiones de informe' para vincularlo tanto a la tabla como al gráfico.
23.
¿Cuál es la ventaja principal de utilizar segmentadores de datos en un informe de Excel en lugar de los filtros tradicionales del menú desplegable?
Facilitan un filtrado visual e interactivo, convirtiendo los filtros ocultos en controles accesibles.
24.
Un gerente desea un KPI que muestre las ventas totales en un período específico, pero únicamente de la categoría 'Electrónica' y realizadas por el vendedor 'Juan'. La estructura de datos contiene columnas para Fecha, Vendedor, Categoría y Monto. ¿Qué fórmula permitiría este cálculo de forma directa?
=SUMAR.SI.CONJUNTO(Monto, Fecha, '>='&D1, Fecha, '<='&D2, Vendedor, 'Juan', Categoría, 'Electrónica')
25.
Si el objetivo es preparar datos para un análisis posterior, ¿qué define a Power Query como una herramienta de ETL?
Su capacidad para Extraer datos de fuentes, Transformarlos mediante limpieza y combinación, y Cargarlos en un modelo de datos o una hoja de cálculo.
26.
Una empresa utiliza tanto Microsoft Excel como Power BI. ¿En cuál de estos entornos es posible acceder y utilizar el Editor de Power Query y con qué propósito?
En ambos; en Excel para preparar datos para hojas de cálculo y en Power BI para preparar datos para los modelos y visualizaciones.
27.
Para configurar un dashboard que será utilizado por 50 vendedores, se requiere que solo puedan modificar la celda B5 y usar los segmentadores de datos, pero no alterar nada más. ¿Cuál es la secuencia correcta de pasos para lograr esta configuración de seguridad?
Seleccionar la celda B5, desbloquearla desde 'Formato de celdas', y luego proteger la hoja marcando la opción 'Usar tablas y gráficos dinámicos'.

28.
¿Cuál es la ventaja fundamental de usar referencias dinámicas como `ventas[importe]` en lugar de rangos fijos como `F2:F50` al realizar cálculos en Excel?
Las referencias dinámicas hacen que las fórmulas sean más cortas y fáciles de leer.
**REPASAR**

29.
Al usar la función ÍNDICE, ¿por qué es crucial que la matriz de datos seleccionada excluya los encabezados de fila y columna?
Porque los encabezados suelen ser texto y la función ÍNDICE solo puede devolver valores numéricos.
**REPASAR**

30.
Al insertar segmentadores de datos en un reporte, ¿cuál de los siguientes ajustes mencionados en la clase permite organizar una larga lista de elementos en un formato más compacto y legible?
Ajustar el número de columnas desde la pestaña 'Segmentación'.