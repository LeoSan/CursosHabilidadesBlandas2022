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


## CLASE 01: 

## CLASE 01: 


## CLASE 01: 


## CLASE 01: 

## CLASE 01: 

## CLASE 01: 



## CLASE 01: 

