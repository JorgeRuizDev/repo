# 🛰️ Proyecto: Reentrenamiento de modelos al detectar Concept Drift

![Cabecera del Proyecto](https://i.imgur.com/HsXeKDB.png)

## 📌 Descripción

Se desarrolló un prototiopo para la realización de mantenimiento predictivo seguro.

Este protitotipo era capaz de actualizar un modelo de manera activa cuando detectava una deriva de concepto (Concept Drift) en los datos.

La detección del Concept Drift se realizaba monitorizando constantemente los sensores con el Ground Truth / Golden y la prediccón de los modelos. 

Si se detecta CD, se recupera de la BBDD un dataset dinámico con los últimos datos capturados del sistema con el cual se intenta re-entrenar el modelo.

Una vez entrenado el modelo, se valida, y si este no tien concept drift, se actualiza el modelo en tiempo real. 

Este proyecto estaba enfocado en entornos industriales, por lo que se decidió añadir una fase de optimización de modelos para dispostivos edge de bajo consumo. 

## 🧰 Tecnologías y Herramientas

- Python
- Numpy
- Docker
- MQTT
- Tensorflow
- Pandas
- PostgreSQL
- Nvidia Jetson Nano

## 👤 Mi rol

- Desarrollador principal de la herramienta en python.
- Desarrollar un sistema de microservicios.


## 🧠 Retos técnicos

- Detectar Concept Drift
- Comunicar distintos módulos asíncronos mediante MQTT
- Re-entrenar los modelos en una Jetson Nano

## 🔗 Referencias externas

- [Paper donde se usa la herramienta](https://annals-csis.org/proceedings/2023/drp/pdf/7674.pdf)


