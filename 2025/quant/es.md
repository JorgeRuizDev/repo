# 🛰️ Proyecto: Cuantizador de Redes Neuronales en Enteros

![Cabecera del Proyecto](https://miro.medium.com/v2/resize:fit:666/1*HrrY_iSyFBqdzhGlKY1GEw.png)

## 📌 Descripción

Se desarrolló un Cuantizador de Redes Neuronales en enteros para poder evaluar el uso de algoritmos de optimización
para reducir la pérdida de precisión de los modelos. 

El cuantizador está enfocado en la compilación de redes neuronales en Hardware (FPGAs). Las FPGAs, a diferencia de una CPU/GPU tradicional, permiten realizar cálculos sin con longitudes de bits arbitrarias (INT8, INT3, INT5, FP11).

A diferencia de las técnicas de cuantización actuales, donde solo se cuantizan los pesos para **ahorrar memoria de la GPU** pero las operaciones se mantienen en float, este cuantizador seguía una filosofía algo más compleja, donde **también se cuantizaban las operaciones de la red neuronal**, permitiendo realizar la **inferencia sin operaciones en coma flotante**.

Por último, el cuantizador tenía soporte para la integración de algoritmos de optimziación para mejorar la precisión final.


## 🧰 Tecnologías y Herramientas

- Python
- Numpy
- Tensorflow (para la ingesta de modelos)

## 👤 Mi rol

- Desarrollador principal de la herramienta en python.
- Investigación de la cuantizació nde redes neuronales


## 🧠 Retos técnicos

- Cuantizar redes neuronales en distintos tamaños (INT8, INT4, INT3, INT2) 
- Realizar el Feed Forward de cada capa sin usar coma flotante (solo enteros) para maximizar el rendimiento.
- Extensibilidad de capas y optimizadores.
- Investigación su aplicación en redes 

## 🔗 Referencias externas

- [Paper que lo utiliza](https://link.springer.com/chapter/10.1007/978-3-031-21753-1_34)


