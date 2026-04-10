# semana3
Actividad: Implementación de codigo con 2 metricas y loss.

**Objetivo**: Crear un programa en python en donde se evidencia la implementación de una red nuronal con funciones de activación 2 metricas y loss.

**A continuación se da a conocer como se implemento el desarrollo del código:**
1. Se importo las librerias de numpy para con arreglos, matplotlib para la representación de gráficas,Keras para crear redes neuronales, tensorflow.keras para aplicar las capas de las redes neuronales y sklearn.model_selection para importar funciones para divudir los datos.
2. Se crean los arreglos para la variable X y Y teniendo en cuenta las compuertas lógica del AND.
3. se divide los datos para el entrenamiento y prueba tener en cuenta que se debe agregar el valor del porcentaje de validación
4. se crea el modelo mediante la creacion de una función que contiene una variable que almacena un modelo capa tras capa, adicional se crea la primera caoa que contiene 8 neuronas activa el metodo del Relu y con 2 variables, posteriormente se crea la segunda cpa con 4 neuronas y tambien se activa el metodo del Relu, en continuación se crea la capa salida teneindo en cuenta solo una neurona de resultado y la activación del metodo de la clasificación binaria y por último retorna el modelo.
5. Se crea un diccionario con los metodos de optimización en donde en la primera linea se crea el SGD el cual se carcteriza por el aprendizaje del gradiente descente, ademas se crea Adam el cual se caracteriza por ajustarse automaticamente del aprendizaje y el RMSprop con el objetivo de ser alamacenados para el entrenamiento de cada modelo.
6. se crea un ciclo en donde se evidencia el recorrido de cada optimizador y se evidencia en pantalla ya cuando estan listos, ademas se crea un modelo nuevo en donde se optiza segun lo actual, define la función de error, las metricas para evaluar lo cual son por precisión.
7. Se entrena el modleo dandolo los arreglos, la cantidad de veces que se recorre, se activa los datos de validación para ver el rendimiento y almacena los resultados del entrenamiento.
8. se gráfica en donde se crea un ciclo para que muestre el recorrido de cada modelo entrenado con su respectiva de error de entrenamiento y error de validación.

**conclusiones**
<img width="1264" height="590" alt="image" src="https://github.com/user-attachments/assets/993608e7-6797-4b88-aa93-47134b4a81cd" />

Teniendo en cuenta el resultado se puede identificar que de 30 interacciones y un porcenje de 20% de validación el mas efectivo es el de Adam debido a que mas o menos en inyteracicion 28 se esta aproximando a 0 y en el entrenamiento gana SGD que busca bajar a 1.

<img width="736" height="385" alt="image" src="https://github.com/user-attachments/assets/b747f2ee-362f-40c9-a03b-869aab41eef3" />
Teniendo en cuenta el resultado se puede identificar que de 90 interacciones y un porcenje de 20% de validación el mas efectivo es el de Adam debido a que mas o menos en inyteracicion 70 se esta aproximando a 0 y en la validación  gana SGD que busca bajar a 1.

En conclusión en mas eficiente es el Adam debido a clasificación evidencia de entrenamiento debido que SGD tarda para poder bajar a 0.



