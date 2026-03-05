# Estimación del nivel de estres basada en GSR (Respuesta Galvanica de la Piel)
## Introducción
La actividad electrodérmica en un principio se definió como un término común para los fenómenos eléctricos de la piel, este término fue introducido por Johnson y Lubin en 1996.  Hoy en día esta respuesta electrodérmica esta relacionado con la respuesta de las glándulas sudoriparas y existen dos medidas principales la resistencia o conductancia que sería la parte exosomática y la detección de voltajes que es lo endosomática [1].
El estrés es una respuesta fisiológica del cuerpo ante situaciones que pueden pertubar el equilibrio físico y emocional, afectando la homeostasis fisiológica o psicológica que el organismo llega a percibir como nociva. Cuando una persona se estresa se activan síntomas como el aumento de la frecuencia cardíaca, los niveles de insulina, el sudor de la piel, en donde hay una dismiinución de resistencia eléctrica de la piel y la presión arterial [2], 

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
† El valor corresponde al rango típico de disparo de disyuntores domésticos.



(Revisar)
(Norma IEC 60479, ítems 1–5)

La norma IEC 60479 establece los efectos fisiológicos producidos por el paso de corriente eléctrica a través del cuerpo humano, considerando variables como la magnitud de la corriente, el tipo de corriente (directa o alterna), la frecuencia y el tiempo de exposición. Esta norma es ampliamente utilizada como referencia para el diseño seguro de sistemas eléctricos y biomédicos.

Corriente alterna (CA)

La corriente alterna, especialmente a frecuencias industriales (50–60 Hz), es considerada más peligrosa que la corriente directa para una misma magnitud de corriente, debido a su mayor capacidad de provocar contracciones musculares sostenidas y alteraciones en el ritmo cardíaco. Según la IEC 60479, los efectos fisiológicos de la CA se clasifican en cinco zonas:

Zona 1: Corrientes de muy baja magnitud, generalmente imperceptibles o apenas perceptibles, sin efectos fisiológicos dañinos.

Zona 2: Corrientes perceptibles que pueden causar sensaciones desagradables y contracciones musculares leves, pero sin efectos fisiológicos permanentes.

Zona 3: Corrientes capaces de producir contracciones musculares intensas, dificultad respiratoria y pérdida del control voluntario, sin llegar necesariamente a fibrilación ventricular.

Zona 4: Corrientes potencialmente letales, asociadas con alta probabilidad de fibrilación ventricular, paro respiratorio y daño severo a órganos internos.

Zona 5: Corrientes extremadamente elevadas que causan paro cardíaco inmediato, quemaduras profundas y daños irreversibles en tejidos y órganos.

Corriente directa (CD)

La corriente directa presenta efectos fisiológicos diferentes a los de la corriente alterna. En general, para valores equivalentes de corriente, la CD es menos peligrosa que la CA a 50–60 Hz, aunque no está exenta de riesgos. Los principales efectos descritos por la norma incluyen:

Sensación inicial de choque al inicio y al final de la aplicación de la corriente.

Menor tendencia a producir contracciones musculares sostenidas, lo que reduce la probabilidad de incapacidad para soltar la fuente.

A corrientes elevadas, puede generar quemaduras térmicas, daño tisular y alteraciones en la función cardíaca.

Exposiciones prolongadas a CD pueden causar efectos electroquímicos en tejidos y electrodos, relevantes en aplicaciones biomédicas con contacto piel-electrodo.

Implicaciones para el diseño del sistema GSR

De acuerdo con la IEC 60479, para aplicaciones biomédicas no invasivas como la medición de la respuesta galvánica cutánea, es fundamental limitar tanto el voltaje como la corriente aplicada al sujeto. En el sistema desarrollado durante esta práctica, se garantiza que la corriente que atraviesa la piel del usuario se mantenga muy por debajo de los umbrales de percepción y riesgo fisiológico, asegurando condiciones de operación seguras y compatibles con los estándares internacionales.

### Cálculos 
(Revisar)
Con el fin de garantizar la seguridad del sujeto durante la medición de la respuesta galvánica cutánea (GSR), se realizó un análisis eléctrico basado en la norma IEC 60479, la cual describe los efectos fisiológicos de la corriente eléctrica sobre el cuerpo humano. De acuerdo con esta norma, es fundamental asegurar que la corriente que atraviesa el cuerpo se mantenga muy por debajo de los umbrales de percepción y riesgo fisiológico.

\[
I=\frac{V_{cc}-V_{ee}}{220\,k\Omega + R_{skin}}
\]

\[
V_{cc}=6\,V
\]

\[
V_{ee}=0\,V
\]

\[
R_{skin}=0\,\Omega \; \text{a} \; 300\,k\Omega
\]

Para un diseño conservador, se consideró el escenario más crítico posible, en el cual la resistencia de la piel del sujeto equivale a un cortocircuito eléctrico:

R_skin = 0 Ω

En esta condición, la limitación de corriente depende exclusivamente de la resistencia fija del circuito.

Análisis del circuito

El sistema de medición opera con una fuente de alimentación continua comprendida entre:

Vcc = 3.3 V a 5 V

y emplea una resistencia limitadora de:

R = 68 kΩ

La corriente máxima que puede circular a través del sujeto se calcula utilizando la Ley de Ohm:

I_max = Vcc / R

Cálculo de la corriente máxima

Para el peor caso (Vcc = 5 V):

I_max = 5 V / 68 000 Ω

I_max ≈ 73.5 µA

Para Vcc = 3.3 V:

I_max = 3.3 V / 68 000 Ω

I_max ≈ 48.5 µA

Verificación de seguridad

Los valores de corriente obtenidos se encuentran muy por debajo del límite máximo permitido de 1 mA, e incluso por debajo del umbral de percepción humana para corrientes eléctricas de baja frecuencia:

I_max ≪ 1 mA

Por lo tanto, el sistema diseñado garantiza condiciones de operación seguras para el usuario, cumpliendo con los criterios de seguridad eléctrica establecidos por la norma IEC 60479, incluso bajo condiciones extremas de contacto eléctrico.

### Diseño del dispositivo vestible
## Pruebas y señal adquirida
## Código ESP
## Código MATLAB
## Resultados de la práctica
## Análisis de resultados
## Conclusiones
## Bibliografía
[1] W. Boucsein, Electrodermal Activity. Nueva York, NY, Estados Unidos:
Springer Science & Business Media, 2012.

[2] M. A. G. Rivera and J. R. J. Cruz, “MEDICIÓN DE ESTRÉS a PARTIR DE LA FRECUENCIA CARDÍACA y LA RESPUESTA GALVÁNICA DE LA PIEL,” González Rivera | Pistas Educativas, Apr. 09, 2018.

[3] R. M. Fish and L. A. Geddes, “Conduction of electrical current to and through the human body: a review,” Oct. 12, 2009. https://pmc.ncbi.nlm.nih.gov/articles/PMC2763825/

