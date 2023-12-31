# Proyecto Final DL: Métodos de DL para  Análisis de Tractografía Mediante Datos de dMRI.
En este proyecto se muestra cómo se puede utilizar el modelo TractSeg para la segementación de bundles, así como las etapas de pre entrenamiento y entrenamiento para bundles no vistos.

La tractografía por resonancia magnética ponderada en difusión, combinada con la selección de trayectorias basada en regiones (bundles), es una combinación única de herramientas que permite la delineación y análisis in vivo de tractos anatómicamente conocidos. Sin embargo, estos procesos son complejos y computacionalmente intensivos. En este proyecto se utiliza como modelo base a ``TractSeg'', estado del arte para segmentar directamente los tractos mediante las direcciones predominantes de la difusión del agua. La base de datos que con la que se trabajó corresponde a la de Renauld 2023, la cual contiene 21 bundles ( ground truth ) de un sujeto que fueron segmentadas por expertos. En este trabajo, exploramos el problema de segmentación cuando se requieren bundles que no formaron parte del modelo preentrenado TractSeg y cuando se tiene únicamente un paciente para entrenamiento. Los resultados aquí expuestos nos llevan a concluir que el problema de segmentación con un solo paciente es un reto muy desafiante y bastante común que puede tratarse con la metodología aquí mostrada pues se obtuvieron dice scores aceptables para la complejidad del problema.

Link de TractSeg: https://github.com/MIC-DKFZ/TractSeg.git

Link de los datos utilizados: 

https://tractometer.org/ismrm2015/home/
https://db.humanconnectome.org/app/template/Login.vm;jsessionid=666DB5400CD1CBB91F74052FAAB77445
