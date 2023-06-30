# Proyecto MOOC-**Henry** 

<p align="center">
<img src=http://www.codlearningtech.org/wp-content/uploads/2015/11/mooc.jpg
</p>

 ## **Mauro Ferrera**


 <hr>  

# INTRODUCCION
## Proyecto basado en plataformas educativas (Mooc)
### Para este proyecto, elegi estudiar el mercado de los cursos on line e identificar como es el progreso y comportamiento de las academias que ofrecen estos servicios de educacion virtual, para dar mejor entendimiento a una nueva organizacion que busca entrar a este mercado .para eso utilizamos tablas con informacion de las empresas Udemy, Cousera y edX .mas adelante podran ver un listado de columnas indicando sus descripciones

<hr>  

# OBJETIVOS DEL PROYECTO 
### Hacer un analisis y diagnostico general de los comportamientos y oportunidades que se presentan en este sector de los cursos on line de los ultimos años de 2011 a 2020 para interpretar comportamientos que ocurren en este sector

<hr>  

# Paso 1: Hacemos un Analisis EDA(Analisis Exploratorio de lo Datos) de los datasets brindados por la academia Henry:
### **Coursera_courses:** Tenemos datos sobre la plataforma Coursera .datos proporcionados por Henry
### **Coursera_reviews:** Tenemos datos especificando la opinion de las personas que hicieron los cursos en Coursera .datos brindados por Henry
### **edx_courses:** Tenemos datos sobre la plataforma edX, fuente original: https://www.kaggle.com/datasets/imuhammad/edx-courses
### **udemy_courses:** Datos sobre la plataforma Udemy, fuente original: https://www.kaggle.com/datasets/andrewmvd/udemy-courses

                     El codigo EDA de estos datasets se puede encontrar en el archivo llamado 'EDA_y_ETL.ipynb'
#### **Para hacer este proceso utilizamos Python**

# Paso 2: Creamos un dashboard en Power BI, plateamos objetivos, hacemos analisis con graficos y sacamos conclusiones:
<hr>  
 
## OBJETIVOS

### **Objetivos en Coursera:** Nuestro objetivo es aumentar en un 20% la cantidad de inscriptos para el año que viene en la plataforma. Nuestro KPI nos indica que hay 158,951 inscriptos y el objetivo es llegar a 200,000 .siendo asi que nos faltan 41,049 inscriptos para llegar al objetivo

<hr>  

### **Objetivos de edX**: Nuestro objetivo es hacer que 4 millones de estudiantes lleguen hasta el nivel avanzado del curso para el año proximo .nuestro medidor nos indica que hay 3 millones solamente en cursos avanzados de los 45 millones de estudiantes que hay .siendo asi que faltan 1 millones de estudiantes que lleguen a nivel avanzado para cumplir con el objetivo

<hr>

### **Objetivos de Ucademy:** Nuestro objetivo es que la tasa de conversion calculada con la cantidad de inscritos que pasan de gratis a inscripciones pagas aumente un 15% para el proximo año, teniendo asi un 344% total de la tasa de conversion y 396% como objetivo a llegar, faltandonos un 13% para cumplirlo

<hr>  

## CONCLUSIONES

### **Coursera:** 
### Las instituciones con mayor cantidad de cursos para ofrecer son universidades. 
### Vemos que el promedio de calificacion de todos los cursos que ofrece esta plataforma es de un 5 de 5. 
### El curso con mayor cantidad de usuarios es el curso de Programacion en Python. 
### Faltan 41 mil nuevos usuarios para aumentar en un 20% la cantidad de usuarios.

<hr>  

### **EdX:** 
### El curso con mayor demanda es computer Science y el curso con menos demanda es Ethics. 
### El curso Energy & Earth Sciences es el mas costoso con un precio promedio de 147 dolares la inscripcion. 
### Los institutos con mayor cantidad de inscriptos son universidades. 
### La cantidad de personas que llegan hasta el curso avanzado del que estan haciendo es de 3 millones

<hr>  

### **Udemy:** 
### El %69.59 de los inscriptos pagaron por el curso.
### En 2015 se genero la mayor cantidad de ganancias en la historia.
### Web Development es la categoria de cursos con mayor inscriptos. 
### Del 2015 al 2016 los estudiantes fueron mas activos al  reportar su reviews. 
### El curso con mayor demanda es Learn HTML5 Programming From Scratch. 
### El año 2015 fue el año con mayor inscriptos en los cursos. 
### Un 28% de estudiantes estan en cursos para principiantes, mientras que el 0.61% esta en cursos avanzados y el 64% estan en cursos principiantes,intermedios y avanzados.

#### **Para hacer todo este analisis y proceso utilizamos la herramienta de Power BI**

                                El analisis graficado de cada plataforma lo pueden ver en el archivo 'Pi_02_PowerBi.pbix' que es un dashboard interactivo

<hr>

## HERRAMIENTAS
### Python
### Power BI 

<hr>

## ¿ A QUIEN VA DESTINADO?
### En este caso de simulacro el proyecto va diriido para una empresa que esta tratando de entender las tendencias de los cursos virtuales y el mercado en genreal

<hr>

## MEDIDAS CALCULADAS
### **COURSERA**
#### º **promedio_calificaciones_totales**: Esta medida calcula el promedio de calificacion de todos los cursos de Cursera.
#### º **cantidad_total_users**: Esta medida calcula la cantidad total de usuarios que hay en Coursera
#### º **KP1**: Esta medida nos calcula el objetivo planteado para nuestro KPI en coursera, que es de aumentar a 200 mil persoan inscriptas
### **EDX**
#### º **Inscriptos_cursos_avanzados**: Esta medida nos indica la cantidad de inscriptos que estan haciendo los cursos avanzados
#### º **KPI2**: Esta medida nos indica el objetivo a llegar en el KPI2 de EDX que es llegar a 4 millones de personas que llegan a los cursos avanzados
### **UDEMY**
#### º **Porcentaje_suscriptores_pagos**: Esta medida nos indica el porcentajes de los inscriptos pagos de la cantidad total de inscriptos 
#### º **Suscriptorespagos**: Medida que indica la cantidad de suscriptores pagos
#### º **Tasa_conversion**: Esta medida nos indica el porcentajes de inscriptos que pasaron de cursos gratuitos a cursos pagos

<hr>

## DESCRIPCION DE LOS DATOS
### **COURSERA**
### **name**: Nombre del curso
### **institution**: Instituto que ofrece el curso
### **course_id**: Nombre unico del curso
<hr>

### **COURSERA_RATING**
### **reviews**: Opinion de gente que hizo el curso
### **reviewers**: Nombre de cada persona que hizo el review
### **date_review**: Fecha en la que se realizo el review
### **sentimiento**: Columna extraida de la columna raviews haciendo un analisis de sentimiento al texto .se mide de 0 a -1 negativo y de 0 a 1 en positivo
<hr>

### **EDX**
### **title**: Mombre del titulo del curso 
### **summary**: Resumen de lo que se trata el curso
### **n_enrolled**: Cantidad de inscriptos en el curso
### **course_type**: Tipo de curso, si es dirijido por un instructor con sus clases en horarios o a ritmo y tiempo propio
### **institution**: Nombre del instituto que ofrece el curso
### **instructor**: Nombre del instructor del curso
### **level**: Nivel de dificultad del curso
### **subject**: Categoria de cursos
### **languague**: Lenguague del curso
### **subtitles**: Idioma de los subtiulos
### **course_effort**: Cuanto hay que dedicarle por semana en promedio
### **course_length**: Duracion del curso en semanas
### **price**: Precio del certificado del curso
<hr>

### **UDEMY**
### **course_id**: ID del curso
### **course_title**: Titulo del curso
### **is_paid**: Indica si los suscriptores pagaron el curso o no
### **price**: Precio del curso
### **num_subscribers**: Numero de subcriptores por curso
### **num_reviews**: Numero de reviews hechas por curso
### **num_lectures**: Numero de conferencias 
### **level**: Niveles de los cursos
### **content_duration**: Duracion del contenido
### **published_timestamp**: Marca de tiempo publicada
### **subject**: Categoria de cursos
### **ganancias_generadas**: Columna obtenida de la cantidad de inscriptos por curso con el precio del curso
### **año_suscripcion**: Año de los suscriptos
<hr>

## FUTURAS LINEAS

### Calcular el precio promedio dependiendo del nivel de los cursos para conocer el precio si baja o sube dependiendo del nivel del curso
### Cantidad de conferencias dependiendo de la categoria de cursos, para ver a que categoria se le invierte mas
### Cantidad de reviews por categoria de cursos, me sirve para conocer en que categoria estan mas activos los estudiantes
### Promedio de duracion de cursos y su cantidad de estudiantes, me sirve para conocer si los estudiantes prefieron cursos cortos o largos
### cantidad de estudiantes que pagan por categoria de curso, me sirve para conocer cual categoria esta obteniendo mas ganancia
### cantidad de estudiantes pagos en cursos para principiantes, intermedios y avanzados, para saber que curso conviene ofrecer
### precio promedio de cada categoria de cursos, para conocer que precios valen en el mercado
### Cantidad de inscriptos por lenguajes, sirve para conocer si la demanda varia dependiendo del lenguague del curso
### promedio de calificacion de los cursos ofrecidos por las plataformas, me sirve para conocer la calidad de los cursos segun los estudiantes de la competencia

#### Gracias por ver!.
https://www.linkedin.com/in/mauro-ferrera/
