# KNN y metricas de clasificacion

Analisis de clasificacion KNN que permita desarrollar un modelo predictivo para analizar por qué los empleados deciden irse con la competencia.

Primero realizamos limpieza de datos y convertir la información en datos que podemos utilizar
<br>![image](https://github.com/user-attachments/assets/067cd228-7be2-4b10-b1dc-d7ddeaa33020)

Separamos el factor objetivo del resto de los datos y aplicamos normalización debido a las diferencias entre magnitudes para poder analizar de forma más optima

<br>![image](https://github.com/user-attachments/assets/bc49bc02-7f47-4ed8-99e9-e9fa204cfec0)

Buscamos obtener el valor optimo para K, en este caso con validacion cruzada, obteniendo la K optima de 1 para este caso

<br>![image](https://github.com/user-attachments/assets/a6f79e69-1b7d-45df-bff5-bdf464c903ac)

Respaldado visualmente con la grafica de los valores y su precisión

<br>![image](https://github.com/user-attachments/assets/2fe93413-c810-40a8-8835-0e689a655f4e)

Definimos las bases de entrenamiento y prueba y obtenemos el valor de precision

<br>![image](https://github.com/user-attachments/assets/c1ab7f10-2a02-4646-9593-aee7698ecb79)

Con ayuda de la matriz de confusion obtenemos una representacion grafica de la prueba realizada
<br>![image](https://github.com/user-attachments/assets/6b5be406-f701-4bf3-b43c-daf5cf4739b7)

Con una precision global de 91.4% podemos observar que efectivamente hace una prediccion acertada entre las personas que no han dejado su trabajo (3149) y las personas que lo dejaron (966); El valor pronosticado para gente que se iria pero realmente se quedo no representa tanto problema y es mayor al pronosticado de gente que se quedaria pero realmente se fue el cual es el resultado que mas afecta a la compañia

Podemos corroborar con la curva ROC la precision
<br>![image](https://github.com/user-attachments/assets/16b14769-e91f-4c27-ad8a-abd0f7d27b7b)

***Conclusion***

Debido a que la curva no muestra un cambio gradual podemos determinar que el modelo podria ser optimizado un poco mas o quiza otro modelo seria el mas adecuado para este caso, aun asi, los valores obtenidos nos proveen de suficiente precision para poder ser utilizados y el AUC corresponde con el score de KNN obtenido previamente.
