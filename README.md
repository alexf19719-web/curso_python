1. Contexto
Las fugas físicas en las redes de distribución de agua potable representan uno de los principales desafíos operativos y financieros para las empresas de acueducto a nivel mundial. 
Por esto, predecir y detectar estas anomalías a tiempo es fundamental para minimizar el Índice de Agua No Contabilizada (ANC), reducir costos operativos de reparación, proteger la 
infraestructura y garantizar la continuidad del servicio a los usuarios. Su definición operativa corresponde a la pérdida de agua tratada que escapa del sistema de tuberías 
antes de llegar al consumidor final, usualmente provocada por el desgaste natural de los materiales, variaciones bruscas de presión o condiciones del entorno.

Las pérdidas de agua han estado presentes desde los inicios de los sistemas de acueducto modernos, y la forma de abordarlas ha evolucionado significativamente a lo largo del 
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
