# Regresion_Lineal
Brahamn Alexander Duque Guzman - 202016908_15

Importa las bibliotecas necesarias:

pandas para el manejo de datos.
matplotlib.pyplot para crear gráficos.
sklearn.linear_model para realizar la regresión lineal.
Carga un archivo CSV llamado "data.csv" en un DataFrame llamado lineal desde la ubicación "C:\date\lineal\data.csv".

Muestra las primeras 5 filas del DataFrame lineal con lineal.head(5).

Crea un gráfico de dispersión (scatter plot) con "metro" en el eje x y "precio" en el eje y utilizando lineal.plot.scatter(x="metro",y="precio").

Muestra el gráfico utilizando plt.show().

Crea una instancia de un modelo de regresión lineal usando linear_model.LinearRegression() y lo almacena en la variable regresion.

Extrae la columna "metro" del DataFrame lineal y la almacena en la variable metros, asegurándose de que tenga la forma adecuada para ser usada en la regresión lineal (una matriz de una sola columna).

Ajusta el modelo de regresión lineal a los datos utilizando regresion.fit(metros, lineal["precio"]).

Imprime los resultados de la regresión:

La intersección (también conocida como el término constante o "b") se imprime con modelo.intercept_.
La pendiente (también conocida como el coeficiente "m") se imprime con modelo.coef_.
Define una lista entrada que contiene cuatro valores de "metro" para los cuales se desean hacer predicciones.

Realiza predicciones utilizando el modelo de regresión lineal con modelo.predict(entrada) y almacena las predicciones en la variable predicciones.

Imprime las predicciones.

Crea otro gráfico de dispersión con los datos originales usando lineal.plot.scatter(x="metro",y="precio", label='Datos originales').

Agrega puntos rojos en el gráfico en las coordenadas definidas en entrada y predicciones usando plt.scatter(entrada, predicciones, color='red').

Dibuja la línea de regresión utilizando plt.plot(entrada, predicciones, color='black', label='Línea de regresión').

Agrega etiquetas de ejes x e y al gráfico.

Agrega una leyenda al gráfico para indicar los elementos que se están representando.

Muestra el gráfico final con plt.show().
