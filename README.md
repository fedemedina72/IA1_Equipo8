# Titanic - Equipo 8
Federico Medina García Corral

Michelle Yareni Morales Ramón

Paola Sofia Reyes Mancheno

María Fernanda Torres Alcubilla

**1. Título:** [Base de datos del Titanic](Datos/Train_limpia.csv) obtenida de [Kaggle](https://www.kaggle.com/competitions/titanic/submissions)
   
**2. Número de instancias:** 889 para el archivo [Train_limpia.csv](Datos/train.csv)
   
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
	&nbsp;&nbsp;&nbsp;8. Title (categórica): indica el título que representa un estatus social con la siguiente codificación: <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;0: Mr<br>
	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1: Mrs<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2: Miss<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3: Master<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4: Don<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5: Rev<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6: Dr<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;7: Mme<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8: Ms<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;9: Major<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;10: Lady<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;11: Sir<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;12: Mlle<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;13: Col<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;14: Capt<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;15: the Countess<br>
   	  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;16: Jonkheer<br>
   
&nbsp;&nbsp;*Variables de salida (objetivo):*  <br>
      &nbsp;&nbsp;&nbsp; 9. Survived: indica 0 si no sobrevivió y 1 al contrario.  <br>

**5. Valores faltantes**  <br>
Nuestra base de datos no cuenta con valores faltantes, anteriormente se hizo una limpieza donde se seleccionaron atributos, rellenaron datos faltantes, se transformaron ciertos atributos y agregaron nuevas características. Dicho proceso se encuentra en [este código](Datos/LimpiezaDatos.ipynb), junto con su justificación. <br>

**6. Distribución de clase**  
62% para no supervivencia y 38% de supervivencia

**7. Documentación**

En la carpeta [Datos](Datos) se encuentra el código [LimpiezaDatos.ipynb](Datos/LimpiezaDatos.ipynb) utilizado para la limpieza de datos, los sets originales de entrenamiento y prueba ([train.csv](Datos/train.csv) y [test.csv](Datos/test.csv) respectivamente) y la base de datos final [Train_limpia.csv](Datos/Train_limpia.csv), de la cual se hará uso en un análisis posterior.


En la carpeta [Modelos](Modelos) se encuentra el código [Modelos.ipynb](Modelos/Modelos.ipynb) donde se realizó la implementación de 4 modelos de clasificicación, los cuales son: *Light Gradient Boosting Machine, Extreme Gradient Boosting, Gradient Boosting Classifier y Random Forest Classifier*, se experimentaron distintos valores para sus hiperparámetros y se escogieron los que mejoraban los valores de las métricas de aprendizaje, considerando el accuracy, precision, recall y F1 score. Además, se realizaron visualizaciones para estas métricas dependiendo de los valores escogidos y de los modelos finales se pueden observar matrices de confusión. Después de la comparación entre estos algoritmos, para cumplir los objetivos de clasificación del problema, se seleccionó el modelo *Light Gradient Boosting Machine*. 

En esta carpeta, también se encuentran los archivos [**Modelo_App**](https://github.com/fedemedina72/IA1_Equipo8/blob/main/Modelos/Modelo_App.ipynb) y [**Titanic_predict.aia**](https://github.com/fedemedina72/IA1_Equipo8/blob/main/Modelos/Titanic_predict2.aia), los cuales se utilizaron en conjunto para crear la interfaz de usuario para y así interactuar con el modelo. El primero se utiliza para exportar los datos y el modelo a una base de datos No-SQL y posteriormente conectarse con la interfaz creada en el MIT APP Creator, es decir, el segundo archivo enlistado. 

Los cambios implementados (*completar en entrega final*).
