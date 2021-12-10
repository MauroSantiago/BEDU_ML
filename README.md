# BEDU_ML
## :rocket:  Proyecto: Clasificación de riesgo crediticio
**Curso de Ciencia de Datos, BEDU**   
*Mauro Santiago*
  
<![imagen](imagenes/dataset-card.jpg)>
  
---
  
## :capital_abcd: Introducción

​Este proyecto está basado en el reto

Este proyecto está basado en el reto *German Credit Risk* disponible en la plataforma [Kaggle](https://www.kaggle.com/uciml/german-credit).
Este proyecto incluye un conjuntos de datos:

German_credit_data

## Contexto

El Datase contiene 1,000 entradas con 20 categorías. Estos datos fueron preparados por el Prof. Hofmann. En este, cada entrada representa a una persona que recibe un crédito de un banco. Cada persona se clasifica como riesgo crediticio bueno o malo según el conjunto de atributos. El enlace al conjunto de datos original se puede encontrar a continuación

## Contenido

El Dataset original es muy complicado de trabajar debido a su complicado sistema de categorías y símbolos , por tal motivo se trabajó con una Dataset previamente modificado por un tercero. Link[     ]

Los atributos con los que se van a trabajar son :

- Age (Variable numérica en años de los clietes) 
- Sex (Variable categórica)
- - Categorías: (masculino, femenino)
- Job (Variable categórica) 
- - Categorías numéricas: 0 - no calificado y no residente, 1 - no calificado y residente, 2 - calificado, 3 - altamente calificado
- Housing (Variable categórica)
- - Categorías: (own, rent, free)
- Saving accounts (Variable categórica) 
- - Categorías: (little, moderate, quite rich, rich)
- Checking account (Varieble numérica en DM (Deutsch Mark/Marco Alemán)
- Credit amount (Variable numérica en DM )
- Duration (Variable numérica en meses)
- Purpose (Variable categórica)
- - Categorías: (car, furniture/equipment, radio/TV, domestic appliances, repairs, education, business, vacation/others)

Variable Objetivo 

- Risk (Variable categórica)
- - Categorías: (good, bad)

### :dart: Objetivos y Tareas
---
​
<Describir cada uno de los objetivos y de las tareas que realizarán/realizaron en el proyecto.>
- Con ayuda de __Python__ sobre su herramienta __Jupyter Notebooks__ se ealizarán las siguients tareas:

- - Carga de datos usando `pandas`
- - Análisis exploratorio de datos
- - Labores de predicción
- - Clasificación
- - etc.

-  Con la varile objetivo `Risk`se van a evaluar diferentes tipos de modelos de regresión y clasificación con el fin de poder predecir el perfil de riesgo de nuevos clientes.
 
---
​
## :ballot_box_with_check: Carga y preprocesamiento de datos
  
** Carga de datos **

Con  __Jupyter Notebooks__  y el uso de `pandas` se carga el Dataset `scored_data`.

** Preprocesamiento 1 **
- [scored_data_all_bin.csv](Datasets/scored_data_all_bin.csv)

1. Los datos `saving_accounts` y `checking_account` presentan valores Nan los cuanles se cambian a no una string de `no_info `, para poder trabajar con los datos.
2. Se utiliza `LabelBinarizer` y `LabelEncoder` de  `sklearn.preprocessing` para procesar los datos categoricos a numerícos.
3. Se guarda el archivo.
....

** Preprocesamiento 2 **
- [scored_data_all_bin.csv](Datasets/scored_data_all_bin.csv)

1. La variables numericas (`age`, `duration`, `credit_amount`) se trasforman a numericas.
2. Con `get_dummies` se transforman los datos a binarios.
3. Se guarda el archivo.
.....



---
  
## :ballot_box_with_check: Trabajo a futuro
  
<Describir tareas pendientes que pueden ayudar a mejorar los resultados.>
  
