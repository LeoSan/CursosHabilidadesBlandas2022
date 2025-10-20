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

## CLASE 01: 


## CLASE 01: 