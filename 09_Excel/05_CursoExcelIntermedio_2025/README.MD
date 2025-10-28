# Curso de Excel Intermedio 🚀

> Aprende a generar análisis precisos, automatizar tareas con Power Query, construir dashboards con controles interactivos y aplicar funciones avanzadas para limpiar y analizar grandes volúmenes de datos. Toma decisiones ágiles y confiables basadas en información bien estructurada.

| Detalle | Información |
| :--- | :--- |
| **Publicado el** | Publicado el 09 de octubre de 2025 |
| **Profesor** | Daniela Tellez |
| **Fecha de Inicio** | 06/10/2025 |
| **Fecha de Fin** | 30/10/2025 |

## CLASE 01: Tablas dinámicas y dashboards interactivos en Excel

**¿Qué aprenderás en Excel para análisis de datos profesional?**
Este entrenamiento te enfoca en resultados concretos: convertir datos en decisiones. Verás cómo pasar de lo básico a un uso estratégico de Excel con técnicas que conectan análisis, visualización y automatización.

- Convertir archivos desordenados en tablas estructuradas listas para análisis.
- Usar tablas dinámicas para responder preguntas de negocio reales.
- Identificar productos que están creciendo y dónde se pierde dinero.
- Crear rankings por márgenes y crecimiento.
- Construir un dashboard interactivo con segmentadores y escalas de tiempo.
- Ejecutar simulaciones con Solver para tomar decisiones informadas.
- Implementar automatizaciones con Power Query para actualizar en segundos.

## CLASE 02:  Cómo importar archivos CSV, texto y web en Excel


**PASOS**
- Paso 1: Desde la pestaña de datos podemos acceder las funcionalidades de obtener y transformar datos 
![alt text](image.png)

- Paso 2: Podemos indicar que datos podemos establecer  

![alt text](image-1.png)

- Paso 3: Aceptar y tenemos los datos en nuestra hoja de manera ordenado ya que la podemos validar previamente 


**¿Qué palabras clave y habilidades fortaleces?**
- Obtener y transformar datos: conectar orígenes y actualizar datos.
- Texto/CSV: importar con delimitador y validar vista previa.
- Texto en columnas: separar datos con delimitados o ancho fijo.
- Atajos: control E, control A, control C para seleccionar y copiar rápido.
- De la web y URL: traer tablas específicas y mantenerlas al día.

>[!NOTE]
> Podemos usar Pestaña Datos / De la Web / Establercer el enlace y nos traera de manera opcional que queremos usar de esa web 
> PD: si la web es privada es decir usa credenciales podemos indicarselas y nos dara acceso al portal que necesitamos  obtener los datos que se especifiquen  

![alt text](image-2.png)

## CLASE 03: Referencias dinámicas en tablas de Excel con nombres de columna
> Convierte tus datos en una tabla de Excel y acelera cálculos y actualizaciones. Aquí verás cómo crearla con Ctrl+T, activar encabezados, usar referencias dinámicas con arroba (@), nombrar la tabla como ventas y sumar columnas como importe. Además, aprenderás a traer toda la tabla o una columna específica con corchetes y a preparar el reto del IVA.


**¿Cómo crear formato de tabla con ctrl+t y encabezados?**

Transforma tu rango en una tabla para ganar velocidad y claridad. Selecciona los datos y usa Ctrl+T. En “crear tabla”, marca la tabla tiene encabezados y acepta. No es solo estética: la tabla habilita funciones prácticas y hace que las actualizaciones de archivo sean más rápidas cuando recibes nuevos datos.

- Selecciona el rango y presiona Ctrl+T.
- Marca la casilla la tabla tiene encabezados.
- Acepta para aplicar formato de tabla.
- Obtén estructura, filtros y estilos automáticos.
- Facilita actualizaciones al llegar nuevos archivos.

**Como cambiar el nombre de tabla**

![alt text](image-3.png)

>[!NOTE]
> Nomeclatura luego de transformar una hoja en una tabla usando el insertar podemos usar la siguiente nomeclatura para acceder a nuesteos valores en nuestras formular ejemplo 1 :  NombreTabla[@campo] =>´Ventas[@cliente]´
> Usando Nomeclatura podemos importar los datos existentes en una tabla con esta formular ´=Error_001[#Datos]´ viene ya con un mini menu desplegable para que podemos elegir 
> Usando Nomeclatura podemos traer los valores de una columna ´=Error_001[[#Datos], [Precio de la oferta]]´

## CLASE 04: Limpieza avanzada de datos en Excel con funciones anidadas

> Impulsa la calidad de tus datos en Excel con técnicas de limpieza avanzadas y fórmulas anidadas. Aquí verás cómo estandarizar texto, validar correos, marcar duplicados, unir campos y contar con comodines para tu dashboard actualizado de forma automática. Todo con referencias de tabla para trabajar con precisión y velocidad.


## CLASE 04: Limpieza avanzada de datos en Excel con funciones anidadas
> Impulsa la calidad de tus datos en Excel con técnicas de limpieza avanzadas y fórmulas anidadas. Aquí verás cómo estandarizar texto, validar correos, marcar duplicados, unir campos y contar con comodines para tu dashboard actualizado de forma automática. Todo con referencias de tabla para trabajar con precisión y velocidad.

**FORMULAS**
- HALLAR            => ´=HALLAR("@",Tabla1[@Correo])´ Siempre devuelve un número 
- valida dubplicado => ´=SI(CONTAR.SI(Tabla1[Correo],Tabla1[@Correo])>1,"DUPLICADO","OK")´
- UNIR CADENAS      => ´=UNIRCADENAS("-",VERDADERO,Tabla1[@[ID_Cliente]],Tabla1[@Nombre],Tabla1[@Segmento],Tabla1[@País])´
- CONTAR PALABRAS usando comodin   => ´=CONTAR.SI(Tabla1[Correo],"*.mx")´ * (Comodines )
- CONTAR PALABRAS usando comodin   => ´=CONTAR.SI(Tabla1[Nombre],"G*")´ * (Comodines ) que empiece con G
- CONTAR PALABRAS usando comodin   => ´=CONTAR.SI(Tabla1[Correo],"*gmail*")´ * (Comodines ) que tenga gmail 
- sustituir   => ´=SUSTITUIR(Tabla1[@Correo],",",".")´  

**RETO**
👉 Crea una columna que combine el Nombre_Limpio y el Correo_Limpio en un solo campo. => ´=LIMPIAR(UNIRCADENAS("-", ,ESPACIOS([@Nombre]), ESPACIOS([@Correo])))´
👉 Usa CONTAR.SI para saber cuántos correos terminan en Hotmail => ´=CONTAR.SI([NombreYCorreo], "*hotmail*")´
---
👉 Encuentra en la tabla un correo que no tenga “@” y corrígelo con SUSTITUIR agregando la arroba antes del dominio. => 

Aplique dos pasos YA QUE EL PROBLEMA ES GRANDE Y APLIQUE DIVIDE Y VENCERAS
- Paso 1: primero queria realizar LA FORMULA BÁSICA ´=SI(ESNUMERO(HALLAR("@",[@Correo])),"SI",SUSTITUIR([@NombreYCorreo],"yahoo", "@yahoo"))´ Me funciono con los yahoo 
- Paso 2: Luego de validar y ver las clase de nuevo pues sustituir no acepta multiples textos por lo que es valido hacer condicionales anidados y quedo la formula así, en las secciones del NO del condicional =SI reaplique la formula para los distintos casos encontrados quedando así 

´=SI(ESNUMERO(HALLAR("@",[@Correo])),[@Correo]
,SI(ESNUMERO(HALLAR("yahoo",[@Correo])),SUSTITUIR([@Correo],"yahoo","@yahoo")
,SI(ESNUMERO(HALLAR("hotmail",[@Correo])),SUSTITUIR([@Correo],"hotmail","@hotmail")
,SI(ESNUMERO(HALLAR("gmail",[@Correo])),SUSTITUIR([@Correo],"gmail","@gmail"),[@Correo])))
)´

- Paso 3: aplique formula antes de saber cuales no tenian arroba y estudiar el patrón para luego sustituirlo 
´=SI(ESNUMERO(HALLAR("@",[@Correo])),"SI","NO")´

## CLASE 05: Filtros avanzados y funciones SUMAR.SI.CONJUNTO en Excel

**¿Cómo aplicar filtros avanzados de forma rápida?**
Aplicar un filtro es inmediato: control l, luego menú de inicio > ordenar y filtrar > filtro. También puedes usar el atajo control shift l. Verás el ícono de embudo en las columnas con filtros activos, útil para reconocer si alguien más ya filtró la hoja.

Filtra por varios criterios. Ejemplo: segmento PYME y país México o España.
Usa filtro personalizado para combinar reglas en una misma columna.
Aplica filtros en una o varias columnas al mismo tiempo.

**¿Cómo sumar si conjunto y contar si conjunto para múltiples criterios?**
Cuando necesitas sumar o contar con varios criterios simultáneos, usa estas funciones. Ejemplo típico: país México, segmento retail y una categoría específica al mismo tiempo.

**¿Qué significan rango suma y rango de criterios?**
En sumar si conjunto:

- Escribe “= sumar si conjunto”.
- Define el rango suma: los datos a sumar, por ejemplo, el campo de importe.
- Usa F4 para fijar el rango si es un rango matriz.
- Elige rango de criterios 1: donde es posible encontrar “México” (por ejemplo, la columna país).
- Especifica criterio 1: “México” entre comillas.
- Elige rango de criterios 2: donde es posible encontrar “retail” (por ejemplo, la columna segmento).
- Especifica criterio 2: “retail”, también entre comillas.
- Repite el patrón para más criterios si los necesitas.
- Consejo práctico: aplica control shift cuatro para formato moneda después de obtener el resultado.

**¿Cuál es la diferencia entre sumar si conjunto y contar si conjunto?**

sumar si conjunto: devuelve la suma del importe que cumple los criterios.
contar si conjunto: devuelve el número de transacciones que cumple los criterios. No requiere “rango suma”, solo rangos de criterios y sus criterios.

**¿Cómo ordenar con orden personalizado y varios niveles?**
El orden personalizado te ayuda a presentar datos con estructura clara. Ve a orden personalizado, amplia la selección y agrega niveles para ordenar por varias columnas a la vez.

Ordena por país de a a z si es texto.
Agrega un nivel por importe de mayor a menor o de menor a mayor.
Verás cada país agrupado y, dentro, los importes ordenados de más a menos (o al revés).
Atajos clave para agilizar:

control shift l: activar/desactivar filtros.
f4: fijar rangos en fórmulas.
control shift cuatro: formato moneda.
control shift + flechas: seleccionar rangos rápidamente.


```Formulas
#Formula es RangoSuma, RangoCriterior1, "CaracterComparar",RangoCriterior2, "CaracterComparar2", RangoCriterior3, "CaracterComparar3"

=SUMAR.SI.CONJUNTO($T$2:$T$20001,$J$2:$J$20001,"Pyme",P2:P20001,"Gorra")
=SUMAR.SI.CONJUNTO(T2:T20001, F2:F20001, 3, K2:K20001, "México")
``` 

## CLASE 06: Listas desplegables anidadas en Excel con índice y coincidir

¿Qué es una lista desplegable anidada y por qué mejora tu reporte?
Una lista anidada conecta dos menús: eliges una categoría y, automáticamente, el segundo menú muestra sus subcategorías. Por ejemplo: hogar, moda u oficina activan opciones distintas. Esto evita mostrar todo a la vez y facilita el análisis.

Reduce el ruido visual y el error humano.
Acelera la selección al mostrar solo opciones válidas.
Hace tu reporte más interactivo y usable.


¿Qué hace coincidir y por qué devuelve 5?
Coincidir busca un valor dentro de un encabezado y regresa su posición. Ejemplo: buscar “software” en la fila de cabeceras con coincidencia exacta (0) devuelve 5 porque es la quinta columna. Ese resultado reemplaza el número de columna en índice, volviéndolo dinámico.

Valor buscado: la categoría elegida en la primera lista, como “moda” o “software”.
Rango de búsqueda: solo las cabeceras, fijadas con F4.
Tipo de coincidencia: 0 para coincidencia exacta.
Integración práctica: índice usa la matriz completa; coincidir calcula la columna según la categoría seleccionada. Si cambias de “software” a “moda”, las subcategorías cambian en automático.

¿Cómo convertirlo en una lista desplegable?
Copia la fórmula dinámica que devuelve la columna de subcategorías.
Selecciona la celda donde irá la segunda lista.
Abre validación de datos y elige lista.
En origen, pega la fórmula y confirma.
Prueba: al elegir “oficina”, verás opciones como “cuaderno”; si cambias a “moda”, aparecerá “jeans”.

## CLASE 07:Agrupaciones de fecha, texto y número en tablas dinámicas

¿Cómo agrupar por fecha, texto y número en Excel?
La clave está en el tipo de dato: fecha, texto o número. Cada uno permite agrupaciones distintas y complementarias para análisis más profundos.

¿Cómo agrupar por fecha en meses, trimestres o años?
Arrastra un campo con formato de fecha a la tabla dinámica y haz clic derecho > Agrupar. Verás opciones como comenzar en y terminar en, que representan el periodo disponible, y podrás elegir meses, trimestres o años. También están horas, minutos y segundos para granularidad fina.

Prácticas rápidas: - Si solo necesitas años, selecciónalos y acepta: verás el total del periodo seleccionado. - Para quitar días y quedarte con meses, marca meses y desmarca días. - Agrega Importe al área de valores para obtener totales por periodo.

Beneficio: obtienes una visión temporal clara, útil para tendencias, estacionalidad y cortes ejecutivos sin fórmulas adicionales.

¿Cómo agrupar por texto con grupos personalizados?
Cuando el campo es texto (por ejemplo, “Nombre de producto”), puedes crear grupos manuales: - Copia la tabla dinámica para mantener la anterior intacta. - Selecciona varios ítems, clic derecho > Agrupar. - Renombra el grupo (ejemplo: “Hogar”) para hacerlo más legible.

Ventajas: - Consolidas ítems dispersos en categorías hechas a tu medida. - Obtienes totales por grupo para comparar familias de productos o segmentos.

¿Cómo agrupar números en rangos fijos?
Con campos numéricos (por ejemplo, “Importe”), puedes definir rangos: - Coloca el número en filas y/o valores. - Clic derecho > Agrupar. - Define: comenzar en, terminar en y por cada (tamaño del intervalo, por ejemplo, 5000).

Qué obtienes: - Rangos como 5–5000, 10000–15000, 15000–20000, con el total de ventas o conteos en cada segmento. - Detección rápida de concentraciones y outliers.

Aplicaciones directas: - Rangos de edades para análisis demográfico. - Rangos salariales para compensaciones. - Años en la empresa para rotación o antigüedad. - Errores en líneas de producción para medir volumen por severidad.

Tip operativo: si necesitas rehacer el criterio, usa Desagrupar y vuelve a definir los rangos.

>[!NOTE]
> Recuerda podemos generar grupos durante las tablas dinamicas, el tipo de agrupado depende del tipo de datos 
> Si es fecha tiene un formato
> si tiene numeros tiene un formato 
> si tienes texto tiene im formato 

![alt text](image-4.png)

## CLASE 08:  Creación de tops y KPIs con tablas dinámicas en Excel


>[!NOTE]
> Podemos copiar y pegar el mismo valor cuantas veces queramos y darle otro tipo de resumenes checa imagen 
> CLIC normal buscar [Configuración de campo valor ] sobre el tablero dinamico 
> CLIC derecho buscar [Resumir valores por > ] sobre la celda 
> CLIC derecho buscar [Mostrar valores como  > ] sobre la celda - Me Permite saber el pocentaje  
![alt text](image-5.png)


## CLASE 09: Campos calculados y gráficos dinámicos para comparar periodos 

¿Cómo preparar la tabla dinámica para comparar por periodo?
Configura la estructura antes de calcular diferencias. La orientación define la lectura del reporte.

Inserta una tabla dinámica en nueva hoja o hoja existente. Selecciona la ubicación y Aceptar.
Coloca nombre del producto en filas. Coloca fecha en columnas para ver meses.
Asegúrate de que la fecha esté agrupada en mes. También puedes agrupar por día o año según la comparación que busques.
Agrega importe a Valores. Aplica formato de moneda con Control + Shift + 4.
Selecciona rápido el rango: Control + Shift + Flecha abajo y derecha, o Control + E.
Tip clave: puedes arrastrar el mismo importe varias veces a Valores para calcular métricas distintas.
¿Cómo organizar horizontal o vertical?
Horizontal: meses en columnas y productos en filas. Útil para comparar periodos lado a lado.
Vertical: meses en filas y productos en columnas. Ideal si prefieres leer de arriba hacia abajo.
Copia y pega tu tabla dinámica para crear variantes sin empezar desde cero.
¿Cómo obtener la diferencia y el porcentaje vs mes anterior?
El cálculo se logra desde “Mostrar valores como”, sin escribir fórmulas.

Duplica el campo importe en Valores. Clic derecho > Configuración de campo de valor.
Ve a Mostrar valores como > Diferencia de.
Define campo base: fecha (agrupada en mes si comparas por mes).
Define elemento base: anterior para comparar contra el mes previo. También existe “siguiente”.
Cambia el nombre del campo para identificarlo, por ejemplo: “diferencia vs mes anterior”.
Observa que el primer periodo no muestra dato porque no tiene periodo anterior.


>[!NOTE]
> CLIC normal buscar [Configuración de campo valor ] sobre el tablero dinamico 
> Apuntes MOSTRAR VALORES COMO > 
![alt text](image-6.png)
![alt text](image-7.png)
![alt text](image-8.png)

## CLASE 10: Creación de gráficos avanzados para tableros de control

¿Cómo preparar datos con tablas dinámicas para gráficos?
Antes de graficar, organiza la base y crea rangos limpios a partir de tus tablas dinámicas. Así evitas choques y habilitas gráficos que no salen directo desde la tabla dinámica.

Duplica tu tabla dinámica y ubícala en vertical u horizontal según tamaño para que no choquen entre sí.
Limpia campos y conserva solo lo necesario: por ejemplo, país y ventas para el mapa coroplético.
Escribe = y selecciona el dato en la tabla dinámica para activar importar datos dinámicos. Trae el valor correcto del campo.
Evita valores fijos: sustituye “Colombia” por la celda con el país y arrastra la fórmula para que sea dinámico.
Aplica formato de moneda y agrega cabeceras: país y venta.
Recuerda: algunos gráficos requieren este paso intermedio, no salen directo desde “gráfico dinámico”.
¿Cómo crear gráficos potentes en Excel?
Con los datos preparados, construye visualizaciones que respondan preguntas del negocio. Prioriza claridad, proporciones y lectura rápida para tu dashboard.

¿Cómo construir un mapa coroplético desde tabla dinámica?
Selecciona el rango limpio con país y venta generado con importar datos dinámicos.
Ve a insertar > mapas > mapa coroplético.
Si trabajas con varios países, el mapa se verá global; si es un país específico, se concentrará esa región.
Úsalo cuando necesites resaltar distribución geográfica de ventas.
¿Cuándo usar un gráfico de dona para proporciones?
Copia la tabla dinámica y selecciona los datos relevantes.
Analizar tabla dinámica > gráfico dinámico > circular > gráfico de dona.
Mejora lectura de proporciones: procura no más de ocho categorías.
Ideal para mostrar distribución por categoría de forma clara.
¿Cómo armar un velocímetro con dona y porcentaje?
Cambia la dimensión a segmento y muestra valores como porcentaje sobre total general.
Crea un rango con importar datos dinámicos para el valor del segmento seleccionado.
Calcula el complementario: 1 menos ese porcentaje, debe sumar 100 con el valor principal.
Inserta un gráfico de dona con ambas series: valor y complementario.
Ajusta el ángulo inicial a 270 para rotar el arco.
Oculta la parte baja: sin relleno y sin contorno para crear el arco del velocímetro.
Ajusta el tamaño del agujero del anillo para el grosor deseado.
¿Cómo dejar lista la estructura de tu dashboard?
Prepara una tarjeta de resultados y organiza las hojas para que el armado final sea ágil, coherente y fácil de mantener.

¿Cómo crear una tarjeta de resultados con importe?
Toma una tabla dinámica sencilla con solo importe.
Vincula el valor con = a una celda limpia para usarlo como tarjeta.
Mantén solo el dato necesario para el diseño final.
¿Qué estructura mínima debe tener el dashboard?
Hoja 1: fuente de origen en formato tabla.
Hoja 2: tablas dinámicas y rangos intermedios que responden preguntas del reporte.
Hoja 3: vista del dashboard que integra todo lo anterior.
En esta etapa no importa el diseño final: prioriza que los datos respondan las preguntas clave.


![alt text](image-9.png)

## CLASE 11: Diseño de dashboards profesionales en Excel

¿Cómo preparar el lienzo del dashboard en Excel?
Antes de diseñar, ordena el espacio visual. Duplicar la hoja, aplicar un fondo y añadir contenedores transparentes te ayuda a jerarquizar la información desde el inicio y a lograr un estilo consistente.

¿Cómo duplicar hoja y aplicar fondo desde disposición de página?
Crea una nueva hoja y nómbrala “Dashboard 2”.
Ve a disposición de página > fondo > desde un archivo.
Elige uno de los cuatro fondos disponibles en los recursos.
Quita las líneas para que se aprecie el fondo.
Limita el área útil para que solo quede el dashboard visual.
¿Cómo crear contenedores con formas y transparencia?
Inserta formas > cuadrado o rectángulo.
Asigna relleno negro para resaltar secciones.
Clic derecho > formato de forma > ajusta la transparencia según se necesite.
Copia y pega para replicar contenedores de manera uniforme.
¿Cómo dar estilo y formato profesional a tus gráficos?
Trae todos los gráficos desde tus tablas dinámicas, acomódalos y luego aplícales un formato limpio: sin relleno, sin contorno, tipografía consistente y etiquetas legibles. Esto mejora la lectura y la coherencia visual.

¿Cómo importar y acomodar gráficos del modelo?
Copia gráficos con control C desde tus tablas dinámicas.
Pégalos en el dashboard con control V.
Acomódalos de forma estratégica según tu narrativa visual.
Ajusta tamaños más adelante; ahora solo define espacios.
¿Cómo limpiar y dar formato a cada gráfico?
Clic derecho > ocultar todos los botones de campos en gráfico.
Quita líneas y bordes: sin relleno y sin contorno.
Usa color de fuente blanco para contraste sobre fondos oscuros.
Si aplica, usa contorno blanco para destacar el gráfico.
Agrega etiquetas de datos para mostrar valores.
Aplica formato de número personalizado para cantidades compactas: “signo de pesos, gato, coma, gato, gato, gato, coma”.
Cambia la tipografía a IBM Flex Sans u otra consistente.
Activa línea suavizada en opciones de serie para un efecto más fluido.
¿Qué excepciones aplicar según el tipo de gráfico?
Mapa: selecciona la serie > color de la serie. Ajusta el gradiente de más a menos. Define 2 o 3 secuencias; en el ejemplo se usan tres.
Combinado: oculta botones. Ve a diseño > diseño rápido > opción 2. Ajusta relleno y contorno blanco. Reaplica sin relleno, sin contorno y letra blanca.
Pie: agrega etiquetas de datos. En opciones de etiqueta, usa porcentaje y quita valor. Mantén la paleta y limpieza general.
¿Cómo integrar íconos, logos, tarjetas y segmentadores?
Los detalles visuales claros elevan la lectura. Íconos coherentes, un logo bien colocado y tarjetas de resultados enlazadas a celdas hacen que el tablero comunique mejor. Los segmentadores dan control para filtrar por variables clave.

¿Cómo insertar y estandarizar íconos?
Ve a Insertar > íconos.
Elige íconos útiles: venta, gráfico en crecimiento, trofeo.
Inserta varios a la vez para controlar magnitud uniforme.
Cambia el color a blanco para alto contraste.
Redimensiona seleccionando todos para mantener proporcionalidad.
Acomódalos junto a métricas o secciones clave.
¿Cómo agregar el logo desde imágenes?
Ve a Insertar > imágenes > colocar sobre celda > este dispositivo.
Selecciona el archivo de logo de los recursos.
Ajusta tamaño y posición hasta integrarlo al diseño.
¿Cómo crear tarjetas de resultados y segmentadores?
Inserta un cuadro de texto para la métrica principal.
No escribas dentro: selecciona el borde, ve a la barra de fórmulas y enlaza la celda con el dato dinámico.
Da formato con negritas y tamaño grande para dar peso visual.
Repite el proceso para porcentajes u otros KPIs.
Agrega segmentadores para filtrar por país, categoría y región.
Úsalos para responder preguntas del reporte de forma dinámica.


![alt text](image-10.png)


## CLASE 12: Creación de segmentadores dinámicos en reportes de Excel


¿Cómo activar segmentación de datos en un gráfico dinámico?
Primero, confirma que seleccionas un gráfico dinámico (no uno estático). Luego ve a la pestaña Análisis de gráfico dinámico y elige Insertar segmentación de datos. Selecciona los campos: Nombre producto, País y Categoría. Acepta y organiza los segmentadores donde prefieras.

Ajusta columnas del segmentador desde Segmentación: por ejemplo, en tres columnas para ver más elementos a la vez.
Reubica cada segmentador: país a la izquierda, categoría a la derecha, según convenga.
Selecciona varios segmentadores a la vez para aplicar ajustes comunes.
¿Cómo dar estilo a los segmentadores con tu paleta corporativa?
Desde Segmentación puedes aplicar estilos rápidos, incluido el diseño de Platzi. Si necesitas una paleta específica, usa nuevo estilo de segmentación de datos:

Cambia colores, tipo y tamaño de letra, negritas y bordes.
En relleno, entra a más colores y define HEX o RGB para tu paleta.
Guarda el estilo y aplícalo a todos tus segmentadores.
¿Cómo seleccionar varias opciones y limpiar rápido el filtro?
Aprovecha los controles del segmentador en la parte superior:

Activa la selección múltiple para combinar varios países o categorías.
Usa el filtro de limpieza para quitar todas las selecciones al instante.
¿Cómo conectar segmentadores y controlar tablas dinámicas con conexiones de informes?
Para que todo cambie al mismo tiempo, conecta cada segmentador a las tablas dinámicas que debe gobernar. Selecciona un solo segmentador, clic derecho y entra a Conexiones de informes.

Marca las tablas dinámicas que correspondan, por ejemplo, todas las que estén en la hoja TD2 o las que se llamen Tabla dinámica 2.
Desmarca las que no quieras controlar desde ese segmentador.
Repite el proceso con cada segmentador.
Así, al filtrar por un país como España, todos los elementos vinculados se actualizan: tarjetas, top diez, ventas por país y ventas por región. Si algún gráfico no cambia, revisa su conexión.

¿Qué buenas prácticas aseguran control total?
Nombra y agrupa tus tablas dinámicas en una pestaña clara, como TD2.
Verifica conexiones después de mover o copiar elementos.
Usa un orden lógico: país, categoría y producto para filtrar de lo general a lo específico.
¿Cómo añadir y personalizar una escala de tiempo por fecha?
Colócate en un gráfico dinámico y elige Insertar escala de tiempo. Solo aparecerán campos que sean fecha válida. Si la fecha no tiene formato correcto, no se mostrará ninguna opción.

Acepta y posiciona la escala de tiempo donde aporte claridad.
Aplica el diseño de Platzi u otro estilo. Personaliza:
Encabezado, tipografía, negritas e itálicas.
Tamaños, rellenos y bordes.
Colores con HEX o RGB si necesitas coherencia de marca.
¿Cómo conectar y usar periodos con precisión?
Al igual que con los segmentadores, usa clic derecho y Revisar conexiones de informes para vincular la escala de tiempo a todas las tablas dinámicas relevantes.

Juega con periodos: meses, trimestres o rangos específicos.
Combina con categoría para ver, por ejemplo, moda o solo software en un rango concreto.
Si un periodo no tiene datos, ajusta o limpia el filtro rápidamente.

>[!NOTE]
> Aclaración que acabo de notar, los segmentadores no se conectan a las gráficas, se conectan a las tablas dinámicas y las tablas a los gráficos. Por lo tanto para saber a que tabla se están conectando podemos cambiar el nombre a las tablas.

![alt text](image-11.png)

![alt text](image-12.png)


> vALIDAR QUE TABLAS DINAMICAS PODEMOS VALIDAR 
![alt text](image-13.png)

> Insertar Escala de Tiempo 
![alt text](image-14.png)


> Ejemplo me gusto esta forma 

![alt text](image-15.png)


## CLASE 13: Automatización de actualizaciones de datos en Excel 

¿Qué rol cumple el formato de tabla?
Asegura que el origen se expanda al pegar datos nuevos.
Evita redefinir manualmente el rango en cada actualización.
Permite que “Actualizar” funcione con un clic.
¿Dónde usar actualizar y actualizar todo?
En “Analizar tabla dinámica” tienes ambas opciones.
Actualizar: refresca la tabla dinámica activa.
Actualizar todo: refresca todas las fuentes y tablas dinámicas del libro.
Atajo útil: Alt F5 para acelerar el flujo.
¿Cómo automatizar con macros la actualización de tablas dinámicas?
Una macro es código que ejecuta por ti una acción repetitiva. Aquí, refrescará tu tabla dinámica cada vez que se active la hoja, sin que tengas que presionar actualizar.

¿Qué es una macro y qué necesitas nombrar?
Cambia el nombre de la tabla dinámica: en “Analizar tabla dinámica” → “Nombre de la tabla dinámica”. Ejemplo: Ventas.
Identifica el nombre de la hoja donde está la tabla dinámica. En el editor, el nombre entre paréntesis (p. ej., TD3) es el que importa.
Clic derecho en la hoja → Ver código para abrir Visual Basic.
En el módulo de la hoja, elige Worksheet y el evento Activate.
¿Qué código VBA usar para refrescar?
Pega este snippet y ajusta el nombre de tu tabla dinámica entre comillas.

Private Sub Worksheet_Activate()
    ActiveSheet.PivotTables("Ventas").PivotCache.Refresh
End Sub
Cierra el editor y prueba: al activar la hoja, se actualiza la tabla dinámica automáticamente.
¿Tienes varias tablas dinámicas? Duplica la línea cambiando el nombre: “Ventas”, “Vendedores”, “Agentes”.
Guarda como Libro de Excel habilitado para macros (.xlsm). Al abrir, autoriza las macros. Si ves advertencia de autoguardado, es porque debes habilitar macros.
¿Cómo optimizar el dashboard y el archivo?
Fondos que se repiten en celdas vacías consumen memoria y vuelven lento el archivo. Delimita tu área de trabajo ocultando lo que no usas.

¿Cómo delimitar filas y columnas sin borrar?
Selecciona desde la columna límite → Ctrl + Shift + Flecha derecha → clic derecho → Ocultar.
Repite hacia abajo: Ctrl + Shift + Flecha abajo → clic derecho → Ocultar.
Beneficios: área limpia, navegación clara y archivo más optimizado.

> Paso Sencillo para macro 
![alt text](image-16.png)

![alt text](image-17.png)

> VERSION DE MACROS 

![alt text](image-18.png)

## CLASE 14: Relacionar múltiples archivos Excel con PowerPivot para dashboards 
¿Cómo habilitar PowerPivot en Excel?
Para comenzar, es clave activar el complemento correcto. La habilitación se hace desde las opciones de Excel.

Abre archivo > opciones > complementos.
En administrar, elige Complementos COM y haz clic en ir.
Marca PowerPivot for Excel (y si quieres, Power Map for Excel). Acepta.
Si no aparece la pestaña: cierra y abre Excel, o reinicia el equipo.
¿Dónde encuentro otros orígenes de datos?
En la pestaña PowerPivot, haz clic en administrar.
En la ventana de PowerPivot, elige de otros orígenes.
Puedes conectar archivos de Excel y también sistemas como SAP u Oracle cuando lo requiera tu trabajo.
¿Cómo importar y preparar datos con PowerPivot?
El flujo de importación desde Excel garantiza encabezados correctos y una estructura limpia para relacionar datos.

Selecciona archivo de Excel y haz clic en siguiente.
Define la ruta de acceso con examinar y elige tus archivos (ejemplo: clientes).
Activa usar primera fila como encabezados de columna. Es clave para nombrar campos correctamente.
Finaliza y repite para cada archivo. Verás una pestaña por archivo en la parte inferior.
¿Qué es la vista de datos y cómo validarla?
La vista de datos muestra las tablas importadas con sus columnas tal como fueron cargadas.
Revisa que no aparezcan rótulos genéricos como “columna F” o “columna H”.
Si ves columnas sin nombre: elimina la tabla y vuelve a cargarla activando la opción de encabezados.
¿Cómo relacionar tablas y crear dashboards con tablas dinámicas y segmentadores?
La vista de diagrama facilita unir tablas con campos comunes y construir reportes sin fórmulas como buscarv.

Cambia a vista de diagrama: verás cada tabla como una caja con sus campos.
Identifica un campo llave (por ejemplo, ID cliente) que se repite entre tablas.
Arrastra para crear relaciones. Verás un 1 hacia una tabla y una estrella hacia la otra: es una relación de uno a muchos.
Puedes usar varios campos llave según el caso: ID país, ID transacción, etc.
¿Cómo generar tablas y gráficos dinámicos integrados?
Inserta tabla dinámica desde PowerPivot y elige la plantilla de cuatro gráficos.
Crea visualizaciones cruzando tablas: por ejemplo, ventas por segmento, ventas por preferencias o suma de compras.
Cambia el tipo de visual: gráfico circular, gráfico de anillos u otros formatos según el análisis.
¿Cómo usar segmentadores y controlar conexiones?
Agrega segmentadores de datos desde análisis del gráfico o diseño.
Usa segmentadores en distintos niveles para filtrar varias tablas a la vez.
Ajusta conexiones de informes para que los segmentadores controlen todos los gráficos que necesites.
¿Qué ventajas ofrece PowerPivot al rendimiento?
PowerPivot actúa como un espejo de la información: concentra lo necesario sin duplicar archivos pesados.
Tus libros de Excel se vuelven más ligeros y rápidos, incluso con múltiples fuentes.
Ideal cuando un reporte de ventas o compras se compone de varios archivos y necesitas relacionar datos sin procesos manuales.

![alt text](image-19.png)
![alt text](image-20.png)
![alt text](image-21.png)







## CLASE 01: 


## CLASE 01: 


## CLASE 01: 


## CLASE 01: 


## CLASE 01: 

## CLASE 01: 


## CLASE 01: 


## CLASE 01: 

## CLASE 01: 

## CLASE 01: 



## CLASE 01: 

