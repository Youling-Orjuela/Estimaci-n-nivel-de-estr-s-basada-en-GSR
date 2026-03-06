# Estimación del nivel de estres basada en GSR (Respuesta Galvanica de la Piel)
## Introducción
La actividad electrodérmica en un principio se definió como un término común para los fenómenos eléctricos de la piel, este término fue introducido por Johnson y Lubin en 1996.  Hoy en día esta respuesta electrodérmica esta relacionado con la respuesta de las glándulas sudoriparas y existen dos medidas principales la resistencia o conductancia que sería la parte exosomática y la detección de voltajes que es lo endosomática [1].

El estrés es una respuesta fisiológica del cuerpo ante situaciones que pueden pertubar el equilibrio físico y emocional, afectando la homeostasis fisiológica o psicológica que el organismo llega a percibir como nociva. Cuando una persona se estresa se activan síntomas como el aumento de la frecuencia cardíaca, los niveles de insulina, el sudor de la piel, en donde hay una dismiinución de resistencia eléctrica de la piel y la presión arterial [2]. 

La respuesta galvánica de la piel (GSR), también conocida como actividad electrodérmica (EDA), se mide generalmente mediante dos electrodos colocados sobre la superficie de la piel para registrar los cambios en la conductancia relacionados a la actividad de las glándulas sudoríparas. Usualmente, los sitios más utilizados para estas mediciones son las palmas de las manos o las superficies volares de los dedos, debido a que presentan una alta densidad de glándulas sudoríparas y, por lo tanto, muestran una actividad electrodérmica más pronunciada [1].

Sin embargo, en diversas aplicaciones de monitoreo fisiológico, especialmente en sistemas portátiles o de monitoreo continuo, se han explorado ubicaciones alternativas como la muñeca o el antebrazo distal. Estos sitios permiten integrar los electrodos en dispositivos tipo pulsera o reloj, facilitando el registro de la señal durante actividades cotidianas sin interferir significativamente con las tareas del usuario [1]. Además, la superficie volar de la muñeca es adecuada para el contacto con electrodos debido a que presenta menor presencia de vello y permite una fijación estable de los sensores [1].

Aunque la amplitud de la señal electrodérmica obtenida en la muñeca puede ser menor que la registrada en las palmas o dedos, diversos estudios han demostrado que las mediciones en esta zona mantienen correlaciones aceptables con las obtenidas en los sitios estándar, lo que las convierte en una alternativa viable para sistemas de monitoreo ambulatorio y dispositivos portátiles de registro fisiológico [1]. Por esta razón, la captura de GSR en la muñeca resulta adecuada cuando se busca un compromiso entre calidad de la señal, comodidad del usuario y facilidad de implementación en dispositivos portátiles.

## Preparación de la práctica
### Efectos de la corriente
La cantidad de corriente que fluye por el cuerpo genera efectos que podrían ocasionar la muerte, varios de estos efectos resultan del calentamiento de los tejidos y estimulación de músculos y nervios. Se necesitan pequeñas cantidades para causar efectos fisiológicos [3].

### Tabla 1. Efectos estimados de corrientes alternas (CA) de 60 Hz sobre el cuerpo humano

| Corriente (CA, 60 Hz) | Efecto fisiológico estimado                                                       |
| --------------------: | --------------------------------------------------------------------------------- |
|                  1 mA | Apenas perceptible                                                                |
|                 16 mA | Corriente máxima que un adulto promedio puede percibir y “soltar” voluntariamente |
|                 20 mA | Parálisis de los músculos respiratorios                                           |
|                100 mA | Umbral de fibrilación ventricular                                                 |
|                   2 A | Paro cardíaco y daño a órganos internos                                           |
|               15–20 A | Activación del disyuntor eléctrico común (apertura del circuito)                  |

* Valores aproximados para corriente alterna de 60 Hz, dependientes del tiempo de exposición y de las condiciones de contacto.
El valor corresponde al rango típico de disparo de disyuntores domésticos.

La norma IEC 60479 establece los efectos fisiológicos producidos por el paso de corriente eléctrica a través del cuerpo humano, considerando variables como la magnitud de la corriente, el tipo de corriente (directa o alterna), la frecuencia y el tiempo de exposición. Esta norma es ampliamente utilizada como referencia para el diseño seguro de sistemas eléctricos y biomédicos.

**Corriente alterna (CA)**

La corriente alterna, especialmente a frecuencias industriales (50–60 Hz), es considerada más peligrosa que la corriente directa para una misma magnitud de corriente, debido a su mayor capacidad de provocar contracciones musculares sostenidas y alteraciones en el ritmo cardíaco. Según la IEC 60479, los efectos fisiológicos de la CA se clasifican en cinco zonas:

**Zona 1:** Corrientes de muy baja magnitud, generalmente imperceptibles o apenas perceptibles, sin efectos fisiológicos dañinos.

**Zona 2:** Corrientes perceptibles que pueden causar sensaciones desagradables y contracciones musculares leves, pero sin efectos fisiológicos permanentes.

**Zona 3:** Corrientes capaces de producir contracciones musculares intensas, dificultad respiratoria y pérdida del control voluntario, sin llegar necesariamente a fibrilación ventricular.

**Zona 4:** Corrientes potencialmente letales, asociadas con alta probabilidad de fibrilación ventricular, paro respiratorio y daño severo a órganos internos.

**Zona 5:** Corrientes extremadamente elevadas que causan paro cardíaco inmediato, quemaduras profundas y daños irreversibles en tejidos y órganos.

**Corriente directa (CD)**

La corriente directa presenta efectos fisiológicos diferentes a los de la corriente alterna. En general, para valores equivalentes de corriente, la CD es menos peligrosa que la CA a 50–60 Hz, aunque no está exenta de riesgos. Los principales efectos descritos por la norma incluyen:

Sensación inicial de choque al inicio y al final de la aplicación de la corriente.

Menor tendencia a producir contracciones musculares sostenidas, lo que reduce la probabilidad de incapacidad para soltar la fuente.

A corrientes elevadas, puede generar quemaduras térmicas, daño tisular y alteraciones en la función cardíaca.

Exposiciones prolongadas a CD pueden causar efectos electroquímicos en tejidos y electrodos, relevantes en aplicaciones biomédicas con contacto piel-electrodo.

Implicaciones para el diseño del sistema GSR

De acuerdo con la IEC 60479, para aplicaciones biomédicas no invasivas como la medición de la respuesta galvánica cutánea, es fundamental limitar tanto el voltaje como la corriente aplicada al sujeto. En el sistema desarrollado durante esta práctica, se garantiza que la corriente que atraviesa la piel del usuario se mantenga muy por debajo de los umbrales de percepción y riesgo fisiológico, asegurando condiciones de operación seguras y compatibles con los estándares internacionales.

### Cálculos 
Con el fin de garantizar la seguridad del sujeto durante la medición de la respuesta galvánica cutánea (GSR), se realizó un análisis eléctrico basado en la norma IEC 60479, la cual describe los efectos fisiológicos de la corriente eléctrica sobre el cuerpo humano. De acuerdo con esta norma, es fundamental asegurar que la corriente que atraviesa el cuerpo se mantenga muy por debajo de los umbrales de percepción y riesgo fisiológico.

En este caso, se evaluarán dos casos de resistencia cutánea: El valor mas bajo dentro del rango de resistencia cutánea (300k Ohmios) y el caso en el que la resistencia cutánea sea nula (0 Ohmios), evaluando esta condición como un corto circuito.

Para esta evaluacion se hizo uso de la siguiente ecuación con las siguientes condiciones:

$$
I = \frac{V_{cc}-V_{ee}}{220k\Omega + R_{skin}}
$$

Donde se tienen en cuenta las siguientes condiciones:

$$
\begin{aligned}
V_{cc} &= 6V \\
V_{ee} &= 0V \\
R_{skin} &= 0\Omega \text{ y } 300k\Omega
\end{aligned}
$$

Sabiendo esto, y previo a la verificación del criterio de seguridad, se evaluan ambos casos para determinar el valor de las corrientes y comparar lo valores para la estimación de la seguridad al paciente.

### Caso 1: $R_{skin} = 0\Omega$

$$
I=\frac{6V}{220k\Omega}
$$

$$
I=2.73\times10^{-5}A
$$

$$
I=27.3\mu A
$$

### Caso 2: $R_{skin} = 300k\Omega$

$$
I=\frac{6V}{220k\Omega + 300k\Omega}
$$

$$
I=\frac{6V}{520k\Omega}
$$

$$
I=1.15\times10^{-5}A
$$

$$
I=11.5\mu A
$$


Los valores de corriente obtenidos se encuentran muy por debajo del límite máximo permitido de 1 mA, e incluso por debajo del umbral de percepción humana para corrientes eléctricas de baja frecuencia:

$I_{max} ≪ 1 mA$

Por lo tanto, el sistema diseñado garantiza condiciones de operación seguras para el usuario, cumpliendo con los criterios de seguridad eléctrica establecidos por la norma IEC 60479, incluso bajo condiciones extremas de contacto eléctrico.

### Diseño del dispositivo vestible
[![prototipo-1.jpg](https://i.postimg.cc/wMvsKB9z/prototipo-1.jpg)](https://postimg.cc/FdMK3NfC)
[![prototipo-2.jpg](https://i.postimg.cc/h45XzcKH/prototipo-2.jpg)](https://postimg.cc/c6fxPqgm)
[![prototipo-3.jpg](https://i.postimg.cc/2yb8FLCH/prototipo-3.jpg)](https://postimg.cc/4HGgXd7t)
[![prototipo-4.jpg](https://i.postimg.cc/0NkkXB8w/prototipo-4.jpg)](https://postimg.cc/jD1YLvnx)

## Pruebas y señal adquirida
[![estres.jpg](https://i.postimg.cc/ZR8X5cZR/estres.jpg)](https://postimg.cc/9RfLxyD5)
[![nivel-de-estres.jpg](https://i.postimg.cc/C1g6XqDz/nivel-de-estres.jpg)](https://postimg.cc/67M0GTMX)
## Código ESP
## Código MATLAB

## Resultados de la práctica
Durante la práctica de laboratorio se desarrolló un sistema vestible capaz de capturar en tiempo real las variaciones de la respuesta galvánica cutánea (GSR) utilizando electrodos colocados en la muñeca del sujeto de prueba, de manera inalámbrica por medio de una ESP32. La señal adquirida fue transmitida a un computador para su visualización y análisis, permitiendo observar la evolución temporal del voltaje asociado a la conductancia de la piel.

La gráfica muestra la señal de voltaje registrada durante un periodo de tiempo determinado por el usuario manualmente. En esta señal se observan variaciones graduales del nivel basal junto con incrementos súbitos de amplitud, característicos de la respuesta galvánica cutánea. En dicha gráfica se distinguen dos componentes principales de la señal GSR:

**Componente tónica o estacionaria (SCL – Skin Conductance Level):** corresponde al nivel basal de la señal, el cual cambia lentamente con el tiempo.

**Componente fásica o transitoria (SCR – Skin Conductance Response):** se manifiesta como incrementos rápidos de la señal seguidos de una recuperación gradual.

Este comportamiento coincide con lo reportado en la literatura sobre actividad electrodérmica, donde las respuestas SCR aparecen como aumentos rápidos en la conductancia cutánea seguidos de un retorno más lento hacia el nivel basal.

Previo a la estimación del nivel de estrés se realizó un proceso de calibración dividido en dos etapas: El periodo de reposo (REST), en el que el sujeto permaneció en reposo durante aproximadamente 35 s para registrar el nivel basal de la señal y tomar un valor promedio de voltaje para umbralizar, y la segunda etapa que fue, el periodo de respiración profunda (BREATH), en el cual, el sujeto de prueba realizó una inspiración profunda seguida de una exhalación lenta, lo cual generó un incremento en la señal GSR.

A partir de los valores registrados como voltaje promedio, se estimaban dos umbrales, los cuales delimitarían el nivel de estrés al cual esta expuesto el sujeto de prueba. Para esto, se clasificó en tres categorías de estrés: Bajo, cuando hay valores de voltaje inferiores a Th1, moderado, cuando hay valores entre Th1 y Th2, y alto, cuando hay valores superiores a Th2.

Durante la ejecución de la prueba se registraron diferentes niveles de estrés, evidenciados por el sistema mediante mensajes en consola tales como BAJO, MODERADO y ALTO. Estas variaciones coinciden con los cambios observados en la señal GSR, donde los picos de voltaje corresponden a incrementos temporales de la conductancia cutánea asociados a activación del sistema nervioso autónomo.

## Análisis de resultados
## Conclusiones
## Bibliografía
[1] W. Boucsein, Electrodermal Activity. Nueva York, NY, Estados Unidos:
Springer Science & Business Media, 2012.

[2] M. A. G. Rivera and J. R. J. Cruz, “MEDICIÓN DE ESTRÉS a PARTIR DE LA FRECUENCIA CARDÍACA y LA RESPUESTA GALVÁNICA DE LA PIEL,” González Rivera | Pistas Educativas, Apr. 09, 2018.

[3] R. M. Fish and L. A. Geddes, “Conduction of electrical current to and through the human body: a review,” Oct. 12, 2009. https://pmc.ncbi.nlm.nih.gov/articles/PMC2763825/

