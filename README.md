**1. Título:** Base de datos del Titanic
   
**2. Número de instancias:** 889 para el archivo Train_limpia.csv
   
**3. Número de atributos:** 8 + atributo de salida.
   
**4. Información de los atributos**   <br>
&nbsp;&nbsp;*Variables de entrada:*<br>
  	&nbsp;&nbsp;&nbsp;1. Class (categórica): representa si lxs pasajerxs estuvieron en 1ra, 2da o 3ra clase. <br>
	&nbsp;&nbsp;&nbsp;2.  Sex (categórico): donde 0 es masculino y 1 femenino.<br>
	&nbsp;&nbsp;&nbsp;3. Age (numérica): edad de lxs pasajerxs, en el caso que tuviera menos de 1 año, los meses se representan en decimal. <br>
	&nbsp;&nbsp;&nbsp;4. SibSp (numérica): cantidad de hermanxs, esposo y esposa que lxs pasajerxs contaban a bordo. <br>
	&nbsp;&nbsp;&nbsp;5. Parch (numérica): cantidad de padres e hijxs que lxs pasajeros contaban a bordo. <br>
	&nbsp;&nbsp;&nbsp;6. Embarked (categórica): segmenta a lxs pasajerxs según el país desde el cual embarcaron al Titanic. El 0 representa Southampton, Reino Unido; el 1 a Cherbourg, Francia y el 2 a Queenstown, Irlanda. <br>
	&nbsp;&nbsp;&nbsp;7. Comp (numérica): suma de las variables SubSp y Parch, que representa el total de compañía que contaban lxs pasajerxs. <br>
	&nbsp;&nbsp;&nbsp;8. Title: indica el título que representa un estatus social con la siguiente codificación: <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0: Mr&nbsp;&nbsp;4: Don&nbsp;&nbsp;&nbsp;&nbsp;8: Ms&nbsp;&nbsp;&nbsp;&nbsp;12: Mlle&nbsp;&nbsp;&nbsp;&nbsp;16: Jonkheer  <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1: Mrs&nbsp;&nbsp;5: Rev&nbsp;&nbsp;&nbsp;&nbsp;9: Major&nbsp;&nbsp;&nbsp;&nbsp;13: Col  <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2: Miss&nbsp;6: Dr&nbsp;&nbsp;&nbsp;&nbsp;10: Lady&nbsp;&nbsp;&nbsp;&nbsp;14: Capt  <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3: Master&nbsp;7: Mme&nbsp;&nbsp;&nbsp;&nbsp;11: Sir&nbsp;&nbsp;&nbsp;&nbsp;15: the Countess<br>   
&nbsp;&nbsp;*Variables de salida (objetivo):*  <br>
      &nbsp;&nbsp;&nbsp; 9. Survived: indica 0 si no sobrevivió y 1 al contrario.  <br>

**5. Valores faltantes**  <br>
Nuestra base de datos no cuenta con valores faltantes, anteriormente se hizo una limpieza donde se seleccionaron atributos, rellenaron datos faltantes, se transformaron ciertos atributos y agregaron nuevas características. Este proceso se encuentra en este código  <br>

**6. Resumen estadístico**  <br>
		*Min      Max     Mean 	  STD*  <br>
Age		0.42	  80      29.40	  13.52   <br>
SibSp		0	  8	  0.52	  1.10  <br>
Parch		0	  6	  0.38	  0.80  <br>
Comp		0	  10      0.90	  1.61  <br>

**7. Distribución de clase**  
62% para no supervivencia y 38% de supervivencia

