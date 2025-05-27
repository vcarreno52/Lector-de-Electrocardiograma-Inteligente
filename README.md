# Lector-de-Electrocardiograma-Inteligente
## Resumen del proyecto 
Este proyecto consiste en una lector de Electrocardiogrmama (ECG), que detecta la frecuencia cardiaca y genera una simuación del ritmo cardiaco esperado en ondiciones normales. El sistema compara la suimulación con la frecuencia medida por medio del sensor enfocándose en la distgancia entre picos R-R para lograr la detección de posibles irregularidades presentes en el pulso de un paciente. 

### Objetivo actual: 
- Detectar arritmias simples mediante el análisis estadístico de los segmentos presentes entre picos R-R.
- Presentar visualmente tanto la señal detectada por medio del sensor como la simulación del pulso esperado.
- Parametrizar el umbral del diferencia para emitir una alerta. 

Figura 1. En la Figura 1 se presenta la comparación entre una señal ECG real y una señal ECG perfecta simulada. La señal real fue extraída del MIT-BIH Arrhythmia Database, específicamente del Record 100, utilizando una duración de 5 segundos. La señal modelada fue generada a partir de una función idealizada ajustada a la frecuencia cardíaca estimada de la señal real, lo cual permite una comparación visual y temporal más precisa. Ambas señales muestran una coincidencia temporal aceptable en la ocurrencia de los picos R, lo cual valida el ajuste de la frecuencia cardíaca entre ambas. Este alineamiento permitió emplear un algoritmo de detección de picos R, con el cual se calcularon los intervalos RR y se estimó la frecuencia cardíaca.

Con este breve análisis, es posible aventurarse a afirmar que no se evidencian anomalías importantes en la señal, y que el ritmo parece ser regular. Al consultar la base de datos, se verificó que el paciente correspondiente al Record 100 es un hombre de 75 años con ritmo sinusal normal. La frecuencia cardíaca detectada por el sistema fue de 75,9 latidos por minuto, lo que concuerda con la información registrada. Este resultado preliminar indica que el modelo simulado representa adecuadamente la periodicidad de la señal real, aunque aún no captura la variabilidad morfológica presente en señales patológicas. A futuro, será necesario avanzar en la detección de cambios morfológicos en las ondas P, QRS y T, con el fin de identificar alteraciones sutiles que podrían indicar la presencia de arritmias u otras condiciones cardíacas.
