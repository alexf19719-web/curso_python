# 1. Contexto

Las fugas físicas en las redes de distribución de agua potable representan uno de los principales desafíos operativos y financieros para las empresas de acueducto a nivel mundial. 
Por esto, predecir y detectar estas anomalías a tiempo es fundamental para minimizar el Índice de Agua No Contabilizada (ANC), reducir costos operativos de reparación, proteger la 
infraestructura y garantizar la continuidad del servicio a los usuarios. Su definición operativa corresponde a la pérdida de agua tratada que escapa del sistema de tuberías 
antes de llegar al consumidor final, usualmente provocada por el desgaste natural de los materiales, variaciones bruscas de presión o condiciones del entorno.

Las pérdidas de agua han estado presentes desde los inicios de los sistemas de acueducto modernos, y la forma de abordarlas ha evolucionado significativamente a# lo largo del 
tiempo. Históricamente, la identificación de fugas tenía un enfoque puramente reactivo, dependiente de la afloración visible del agua en la superficie o de los reportes ciudadanos. 
Debido a la necesidad de optimizar el recurso, las empresas empezaron a desarrollar sistemas de monitoreo preventivo, como la sectorización hidráulica y los barridos manuales con 
equipos acústicos (geófonos). Posteriormente, se inició el uso de métodos estadísticos tradicionales e indicadores de balance hídrico, que demostraron ser efectivos para aislar 
zonas problemáticas. Con el paso del tiempo, el avance en la recolección de datos permitió incorporar métodos de aprendizaje automático (Machine Learning) que analizan en conjunto
múltiples variables complejas para identificar los patrones ocultos que predisponen a una tubería a fallar.

Una de las principales características que dificultan la predicción de fugas es que, al igual que en otros sistemas de detección de anomalías, las fallas son eventos poco 
frecuentes en comparación con la inmensa extensión de la red que opera con normalidad. Esto genera un problema de desbalance de clases, en el sentido de que la clase minoritaria 
("Hay fuga") se encuentra subrepresentada frente a los registros normales, lo cual puede afectar el análisis exploratorio y el rendimiento de los modelos de predicción. 
El presente trabajo utiliza una base de datos operativa de la red de acueducto de la ciudad de Barranquilla, Colombia, la cual integra registros históricos e hidráulicos del 
sistema, abarcando variables estructurales y dinámicas como la presión, el material de la tubería, los caudales, la geolocalización, la fecha de instalación y el diámetro de las 
redes.

# 2. Objetivos

  ## 2.1 Objetivo general
  Diseñar y desarrollar un dashboard interactivo que permita visualizar y analizar la interacción entre las variables operativas y de infraestructura de la red 
  de acueducto en Barranquilla, integrando un modelo de Machine Learning que facilite la identificación de patrones de fallo y contribuya a la predicción temprana de fugas de agua.
  
  ##2.2 Objetivos específicos
    •	Describir la estructura general de la base de datos, abarcando variables espaciales, temporales, hidráulicas y físicas (presión, material, caudales, geolocalización, fecha de 
    instalación y diámetro).
    •	Evaluar el desbalance de la variable respuesta "Hay o no fuga", dada la baja frecuencia de fallos frente al total de la red operativa.
    •	Analizar la distribución de las variables numéricas (como presiones, caudales y antigüedad de la tubería) utilizando estadísticas descriptivas y visualizaciones.
    •	Comparar las características operativas y físicas de los segmentos de red que presentan fugas frente a aquellos que operan con normalidad.
    •	Identificar posibles patrones espaciales o estructurales asociados a la vulnerabilidad y rotura de las tuberías.
    •	Detectar posibles relaciones y multicolinealidad entre variables (por ejemplo, el impacto combinado de la presión y el material) mediante análisis de correlación.


    •	Generar conclusiones que orienten la selección de características (Feature Engineering) y determinen los algoritmos de clasificación más adecuados para el modelo predictivo.


    
