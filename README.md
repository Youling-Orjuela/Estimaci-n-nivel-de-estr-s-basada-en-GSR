# Estimación del nivel de estrés basada en GSR (Respuesta Galvánica de la Piel)
## Introducción
La actividad electrodérmica (EDA) se definió inicialmente como un término general para describir los fenómenos eléctricos que ocurren en la piel; este concepto fue introducido por Johnson y Lubin en 1966. Actualmente, se sabe que esta respuesta está estrechamente relacionada con la actividad de las glándulas sudoríparas y puede medirse principalmente de dos formas: mediante la resistencia o conductancia de la piel, conocida como medición exosomática, y mediante la detección de potenciales eléctricos generados naturalmente por la piel, denominada medición endosomática [1].

Uno de los fenómenos fisiológicos en los que la actividad electrodérmica tiene gran relevancia es el estrés. El estrés corresponde a una respuesta fisiológica del organismo ante situaciones que pueden perturbar el equilibrio físico o emocional, afectando la homeostasis del cuerpo. Cuando una persona experimenta estrés se activa el sistema nervioso autónomo, particularmente su rama simpática, lo que genera diferentes respuestas fisiológicas como el aumento de la frecuencia cardíaca, variaciones en los niveles hormonales, incremento de la sudoración y cambios en la presión arterial. En el caso de la piel, el aumento de la sudoración provoca una disminución en la resistencia eléctrica cutánea, lo que se refleja como un incremento en la conductancia de la piel [2].

Debido a esta relación con la actividad del sistema nervioso autónomo, la respuesta galvánica de la piel (GSR), también conocida como actividad electrodérmica, se utiliza como un indicador fisiológico para evaluar cambios en el estado emocional o en el nivel de activación de una persona. Esta señal se mide generalmente mediante dos electrodos colocados sobre la superficie de la piel, los cuales permiten registrar variaciones en la conductancia asociadas con la actividad de las glándulas sudoríparas. Tradicionalmente, los sitios más utilizados para realizar estas mediciones son las palmas de las manos o las superficies volares de los dedos, ya que estas regiones presentan una alta densidad de glándulas sudoríparas y, por lo tanto, muestran una actividad electrodérmica más pronunciada [1].

No obstante, en aplicaciones modernas de monitoreo fisiológico, especialmente en sistemas portátiles o de monitoreo continuo, se han explorado ubicaciones alternativas para la medición de la GSR, como la muñeca o el antebrazo distal. Estas zonas permiten integrar los electrodos en dispositivos tipo pulsera o reloj, facilitando la captura de la señal durante actividades cotidianas sin interferir significativamente con las tareas del usuario [1]. Además, la superficie volar de la muñeca presenta condiciones favorables para la colocación de sensores, como menor presencia de vello y mayor facilidad para lograr un contacto estable entre los electrodos y la piel.

Aunque la amplitud de la señal electrodérmica obtenida en la muñeca suele ser menor que la registrada en las palmas o los dedos, diversos estudios han demostrado que las mediciones en esta región mantienen correlaciones aceptables con las obtenidas en los sitios tradicionales. Por esta razón, la medición de la GSR en la muñeca se considera una alternativa viable para sistemas de monitoreo ambulatorio y dispositivos vestibles, ya que permite lograr un equilibrio entre la calidad de la señal, la comodidad del usuario y la facilidad de implementación en aplicaciones de monitoreo continuo [1].

## Preparación de la práctica
## Efectos de la corriente eléctrica en el cuerpo humano

La norma **IEC 60479** describe los efectos fisiológicos producidos por el paso de corriente eléctrica a través del cuerpo humano. Estos efectos dependen principalmente de la magnitud de la corriente, el tipo de corriente (directa o alterna), la frecuencia, el tiempo de exposición y la trayectoria que sigue la corriente a través del organismo. Debido a estos factores, incluso corrientes relativamente pequeñas pueden producir efectos fisiológicos perceptibles o potencialmente peligrosos. Por esta razón, dicha norma es ampliamente utilizada como referencia para el diseño seguro de sistemas eléctricos y biomédicos [4].

En general, la cantidad de corriente que fluye por el cuerpo humano puede generar diversos efectos fisiológicos que van desde sensaciones apenas perceptibles hasta consecuencias graves como paro respiratorio, fibrilación ventricular o incluso la muerte. Muchos de estos efectos se deben al calentamiento de los tejidos biológicos y a la estimulación eléctrica de músculos y nervios, los cuales pueden alterarse con corrientes relativamente pequeñas [5].

### Corriente alterna (CA)

La corriente alterna, particularmente a frecuencias industriales de 50–60 Hz, se considera más peligrosa que la corriente directa para valores equivalentes de corriente. Esto se debe a su mayor capacidad para provocar contracciones musculares sostenidas, interferir con el control neuromuscular y alterar el ritmo cardíaco [4].

De acuerdo con la norma IEC 60479, los efectos fisiológicos de la corriente alterna pueden clasificarse en diferentes zonas de riesgo, dependiendo de la magnitud de la corriente y del tiempo de exposición.

En una primera zona se encuentran corrientes muy pequeñas, generalmente imperceptibles o apenas perceptibles, que no generan efectos fisiológicos dañinos. A medida que la corriente aumenta, se entra en una segunda zona en la que la corriente es perceptible y puede generar sensaciones desagradables y contracciones musculares leves, aunque sin producir efectos fisiológicos permanentes.

En una tercera zona, la corriente puede provocar contracciones musculares intensas, dificultad respiratoria y pérdida del control voluntario de los músculos, lo que puede impedir que una persona suelte la fuente de corriente. Cuando la corriente alcanza valores mayores, se entra en una zona de riesgo significativo en la cual existe una alta probabilidad de fibrilación ventricular, paro respiratorio y otros efectos fisiológicos graves[4].

Finalmente, corrientes extremadamente elevadas pueden producir paro cardíaco inmediato, quemaduras profundas y daños irreversibles en los tejidos y órganos internos.

De manera aproximada, algunos valores típicos reportados para corriente alterna de 60 Hz en el cuerpo humano son:

| Corriente | Efecto fisiológico aproximado |
|-----------|-------------------------------|
| 1 mA | Apenas perceptible |
| 10–16 mA | Corriente máxima que una persona puede soltar voluntariamente |
| 20 mA | Posible parálisis de músculos respiratorios |
| 100 mA | Umbral aproximado de fibrilación ventricular |
| > 1 A | Paro cardíaco y daño severo en órganos |

Estos valores dependen del tiempo de exposición, condiciones de contacto y trayectoria de la corriente en el cuerpo [3].

### Corriente directa (CD)

La corriente directa presenta efectos fisiológicos diferentes a los de la corriente alterna. En términos generales, para valores equivalentes de corriente, la corriente directa suele ser menos peligrosa que la corriente alterna a frecuencias de red, aunque igualmente puede producir efectos fisiológicos importantes [4].

La aplicación de corriente directa suele generar una sensación de choque al inicio y al final del contacto, debido a los cambios bruscos en la intensidad de corriente. A diferencia de la corriente alterna, la corriente directa tiene menor tendencia a producir contracciones musculares sostenidas, lo que reduce la probabilidad de que una persona quede atrapada sin poder soltar la fuente de corriente[4].

No obstante, cuando la corriente alcanza valores elevados, también puede producir quemaduras térmicas, daño tisular y alteraciones en la función cardíaca. Además, exposiciones prolongadas a corriente directa pueden generar efectos electroquímicos en la interfaz piel–electrodo, fenómeno particularmente relevante en aplicaciones biomédicas donde existe contacto directo con la piel [5].

### Implicaciones para el diseño del sistema de medición GSR

Considerando los lineamientos establecidos por la norma **IEC 60479**, en el diseño de sistemas biomédicos no invasivos como el utilizado para medir la respuesta galvánica cutánea (GSR) es fundamental limitar tanto el voltaje aplicado como la corriente que circula a través del cuerpo del usuario.

En el sistema desarrollado durante esta práctica, se implementaron resistencias limitadoras de corriente que garantizan que la corriente que atraviesa la piel del sujeto se mantenga en el orden de los microamperios, muy por debajo de los umbrales de percepción y riesgo fisiológico descritos en la literatura. De esta manera, se asegura que el dispositivo opere bajo condiciones seguras y compatibles con los estándares internacionales de seguridad eléctrica, permitiendo la medición de la conductancia de la piel sin representar un riesgo para el usuario.


### Cálculos 
Con el fin de garantizar la seguridad del sujeto durante la medición de la respuesta galvánica cutánea (GSR), se realizó un análisis eléctrico basado en la norma IEC 60479, la cual describe los efectos fisiológicos de la corriente eléctrica sobre el cuerpo humano. De acuerdo con esta norma, es fundamental asegurar que la corriente que atraviesa el cuerpo se mantenga muy por debajo de los umbrales de percepción y riesgo fisiológico.

En este caso, se evaluarán dos casos de resistencia cutánea: El valor mas bajo dentro del rango de resistencia cutánea (300k Ohmios) y el caso en el que la resistencia cutánea sea nula (0 Ohmios), evaluando esta condición como un corto circuito.

Para esta evaluacion se hizo uso de la siguiente ecuación:

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
Como la región anatómica que se eligio fue la muñeca, se realizó una pulsera con electrodos para medir la respuesta galvánica de la piel y se agregó un chaleco con un compartimiento donde va todo el circuito para la adquisión de la señal por bluetooth.

[![prototipo-1.jpg](https://i.postimg.cc/wMvsKB9z/prototipo-1.jpg)](https://postimg.cc/FdMK3NfC)
[![prototipo-2.jpg](https://i.postimg.cc/h45XzcKH/prototipo-2.jpg)](https://postimg.cc/c6fxPqgm)
[![prototipo-3.jpg](https://i.postimg.cc/2yb8FLCH/prototipo-3.jpg)](https://postimg.cc/4HGgXd7t)
[![prototipo-4.jpg](https://i.postimg.cc/0NkkXB8w/prototipo-4.jpg)](https://postimg.cc/jD1YLvnx)

## Pruebas y señal adquirida
[![estres.jpg](https://i.postimg.cc/ZR8X5cZR/estres.jpg)](https://postimg.cc/9RfLxyD5)
[![nivel-de-estres.jpg](https://i.postimg.cc/C1g6XqDz/nivel-de-estres.jpg)](https://postimg.cc/67M0GTMX)
## Código ESP
```
C++
#include "BluetoothSerial.h"
BluetoothSerial SerialBT;

const char* BT_NAME = "ESP32_GSR";
```
Se importa la librería BluetoothSerial para usar Bluetooth clásico (SPP) en ESP32.
SerialBT actúa como un “Serial” pero inalámbrico.
BT_NAME es el nombre con el que aparece el ESP32 al emparejar.
```
const int adcPin = 34;
const int fs = 25;
const int dt_ms = 1000 / fs;
const int Navg = 20;
```
adcPin: pin analógico donde se lee el voltaje del circuito GSR (GPIO34 recomendado).
fs: frecuencia de muestreo (25 Hz).
dt_ms: tiempo entre muestras para mantener esa frecuencia.
Navg: número de lecturas ADC promediadas por muestra para reducir ruido.
```
float Vbase = NAN;
float Vmin  = NAN;
float Vmax  = NAN;

float Th1 = NAN;
float Th2 = NAN;

double sumBase = 0;
uint32_t nBase = 0;

float H = 0.01;
int level = 0;
```
Vbase: voltaje promedio en reposo.
Vmin, Vmax: valores mínimo y máximo durante respiración profunda.
Th1, Th2: umbrales para definir el nivel de estrés.
sumBase y nBase: se usan para calcular el promedio Vbase.
H: histéresis (10 mV) para evitar que el nivel cambie por ruido.
level: nivel actual (0=LOW, 1=MED, 2=HIGH).
```
int readAdcAvg() {
  long acc = 0;
  for (int i = 0; i < Navg; i++) {
    acc += analogRead(adcPin);
    delayMicroseconds(200);
  }
  return (int)(acc / Navg);
}
```
Se toman Navg lecturas del ADC y se promedian. Esto mejora estabilidad de la señal sin necesidad de suavizar en MATLAB.
```
float rawToVolt(int raw) {
  return (raw / 4095.0f) * 3.3f;
}
```
Convierte el ADC de 12 bits (0–4095) a voltaje aproximado (0–3.3V). Así MATLAB recibe valores en voltios.
```
const char* levelStr(int L) {
  if (L == 0) return "LOW";
  if (L == 1) return "MED";
  return "HIGH";
}
```
Convierte el nivel numérico a texto para enviar por Bluetooth una etiqueta legible.
```
void computeThresholds() {
  float d = Vmax - Vbase;
  if (d < 0.02f) d = 0.02f;
  Th1 = Vbase + 0.25f * d;
  Th2 = Vbase + 0.60f * d;
}
```
Calcula el rango d = Vmax - Vbase.
Si d es muy pequeño, se fuerza un mínimo (0.02 V) para evitar umbrales inútiles.
Umbrales:
Th1: inicio de nivel moderado
Th2: inicio de nivel alto
```
int classifyWithHysteresis(float v, int prev) {
  if (prev == 0 && v > Th1 + H) return 1;
  if (prev == 1 && v > Th2 + H) return 2;

  if (prev == 2 && v < Th2 - H) return 1;
  if (prev == 1 && v < Th1 - H) return 0;

  return prev;
}
```
El nivel sube o baja solo si el voltaje supera el umbral con un margen ±H. Esto evita que el estado cambie rápidamente por ruido cuando el voltaje está cerca del umbral.
```
void startCalibration() {
  st = CAL_REST;
  t_state0 = millis();
  sumBase = 0;
  nBase = 0;
  Vmin =  10;
  Vmax = -10;
  Vbase = NAN;
  Th1 = NAN;
  Th2 = NAN;
  level = 0;

  SerialBT.println("CAL,REST,START");
}
```
Reinicia variables y cambia a CAL_REST. Además envía un mensaje para que MATLAB sepa que inició la calibración.
```
void setup() {
  Serial.begin(115200);
  analogReadResolution(12);

  if (!SerialBT.begin(BT_NAME)) {
    while (true) delay(1000);
  }

  st = IDLE;
  SerialBT.println("READY,SEND_C_TO_CALIBRATE");
}
```
Inicializa el ADC en 12 bits.
Inicia Bluetooth con el nombre BT_NAME.
Queda en IDLE y avisa que está listo para recibir C.
```
void loop() {
  while (SerialBT.available()) {
    char c = (char)SerialBT.read();
    if (c == 'C' || c == 'c') startCalibration();
  }

  int raw = readAdcAvg();
  float v = rawToVolt(raw);
  uint32_t t = millis();
```
Si llega C desde el PC, comienza calibración.
Luego mide raw, lo convierte a v y toma timestamp t.
```
if (st == IDLE) {
    SerialBT.printf("%lu,%d,%.4f,IDLE\n", (unsigned long)t, raw, v);
    delay(dt_ms);
    return;
  }
```
Envía datos en formato CSV sin clasificar estrés. Útil para verificar que el sensor funciona antes de calibrar.
```
if (st == CAL_REST) {
    sumBase += v;
    nBase++;

    if (t - t_state0 > 35000) {
      Vbase = (float)(sumBase / (double)nBase);
      st = CAL_BREATH;
      t_state0 = t;
      SerialBT.printf("CAL,REST,DONE,%.4f\n", Vbase);
      SerialBT.println("CAL,BREATH,START");
    }

    SerialBT.printf("%lu,%d,%.4f,CAL_REST\n", (unsigned long)t, raw, v);
    delay(dt_ms);
    return;
  }
```
Durante 35 s suma voltajes para obtener Vbase.
Al terminar, cambia a CAL_BREATH y avisa a MATLAB.
```
if (st == CAL_BREATH) {
    if (v < Vmin) Vmin = v;
    if (v > Vmax) Vmax = v;

    if (t - t_state0 > 50000) {
      computeThresholds();
      st = RUN;
      SerialBT.printf("CAL,BREATH,DONE,Vmin=%.4f,Vmax=%.4f\n", Vmin, Vmax);
      SerialBT.printf("TH,Th1=%.4f,Th2=%.4f\n", Th1, Th2);
    }

    SerialBT.printf("%lu,%d,%.4f,CAL_BREATH\n", (unsigned long)t, raw, v);
    delay(dt_ms);
    return;
  }
```
Durante respiración profunda se actualizan Vmin y Vmax.
Después de 50 s se calculan umbrales y pasa a RUN.
Se envían mensajes CAL...DONE y TH... para registrar umbrales.
```
if (st == RUN) {
    level = classifyWithHysteresis(v, level);
    const char* tag = levelStr(level);
    SerialBT.printf("%lu,%d,%.4f,%s\n", (unsigned long)t, raw, v, tag);

    delay(dt_ms);
    return;
  }
}
```
Clasifica el voltaje actual en LOW/MED/HIGH usando umbrales e histéresis.
Envía el voltaje junto con la etiqueta (nivel de estrés).

## Código MATLAB
```
MatLab
clear; clc; close all
port = "COM6";
baud = 115200;

s = serialport(port, baud);
flush(s);
s.Timeout = 0.1;
```
clear: borra variables del workspace.
clc: limpia la consola.
close all: cierra todas las figuras abiertas.
Esto asegura que la ejecución empiece “desde cero”.
port y baud definen el puerto COM y la velocidad (debe coincidir con el emisor).
serialport(port, baud) crea el objeto de comunicación s.
flush(s) limpia el buffer del puerto (descarta datos viejos acumulados).
s.Timeout = 0.1 define cuánto espera una lectura antes de “rendirse” (aquí es corto porque no se usa readline, se lee el buffer por bytes).
```
writeline(s, "C");
disp("Calibración iniciada: 35s reposo + 50s respiración...");
```
writeline(s, "C") envía el carácter C por serial hacia el ESP32.
En el código Arduino, ese C dispara startCalibration() y comienza la secuencia de calibración.
disp(...) solo imprime un mensaje informativo en la consola de MATLAB.
```
figure; grid on;
al = animatedline('LineWidth',1.2);
xlabel('Tiempo (s)'); ylabel('Voltaje (V)');
title('GSR - Voltaje en tiempo real');
ylim([0 3.3]);
```
figure; grid on;
al = animatedline('LineWidth',1.2);
xlabel('Tiempo (s)'); ylabel('Voltaje (V)');
title('GSR - Voltaje en tiempo real');
ylim([0 3.3]);
```
t0 = [];
lastLevel = "";
lastDraw = tic;

disp("Leyendo...");
```
t0: guarda el primer timestamp recibido para convertir el tiempo a “tiempo transcurrido” (comienza en 0).
lastLevel: guarda el último nivel (LOW/MED/HIGH) para imprimir en consola solo cuando cambie.
lastDraw = tic: inicia un cronómetro interno para controlar cada cuánto se actualiza la figura.
disp("Leyendo..."): mensaje informativo.
```
while ishandle(al)
```
Este bucle se ejecuta continuamente mientras la gráfica esté abierta.
Si cierras la figura, ishandle(al) deja de ser verdadero y el programa termina.
```
nAvail = s.NumBytesAvailable;
    if nAvail == 0
        pause(0.01);
        continue
    end
```
s.NumBytesAvailable devuelve cuántos bytes hay esperando en el buffer del puerto.
Si es 0, no hay nada que leer → se hace pause(0.01) para no saturar CPU, y continue vuelve al inicio del bucle.
Esto evita warnings típicos de “timeout” y mantiene el programa estable.
```
raw = read(s, nAvail, "char");
    lines = splitlines(string(raw));
```
read(s, nAvail, "char") lee todo lo que esté disponible en ese instante.
Luego se convierte a string y se parte por saltos de línea con splitlines.
Esto es más robusto y rápido que readline(), porque no depende de esperar una línea completa.
```
for i = 1:numel(lines)
        line = strtrim(lines(i));
        if line == "", continue; end
```
Recorre cada línea recibida.
strtrim elimina espacios/saltos al inicio y final.
Si la línea queda vacía, se ignora.
```
if startsWith(line, "CAL") || startsWith(line, "TH") || startsWith(line, "READY")
            disp(line);
            continue
        end
```
El ESP32 además de datos numéricos envía mensajes tipo:
READY,...
CAL,REST,...
CAL,BREATH,...
TH,Th1=...,Th2=...
Si detecta que la línea es un mensaje de estado (CAL, TH, READY), lo imprime en consola y no intenta parsearlo como dato numérico.
```
parts = split(line, ",");
        if numel(parts) ~= 4
            continue
        end
```
El formato esperado de datos es:
timestamp_ms, raw_adc, voltaje, nivel
Por eso:
Se separa por coma.
Si no hay exactamente 4 elementos, se descarta (evita errores por líneas incompletas o ruido).
```
t_ms = str2double(parts(1));
        v    = str2double(parts(3));
        lvl  = strtrim(parts(4));

        if isnan(t_ms) || isnan(v)
            continue
        end
```
t_ms toma el timestamp en milisegundos (campo 1).
v toma el voltaje en voltios (campo 3).
lvl toma el nivel (LOW/MED/HIGH o IDLE/CAL_REST/CAL_BREATH, según el estado que mande el ESP32).
Si t_ms o v no se pueden convertir a número (NaN), la línea se ignora.
```
if isempty(t0)
            t0 = t_ms;
        end
        t_s = (t_ms - t0)/1000;
```
La primera vez que llega un dato, se guarda t0 (origen del tiempo).
Cada nuevo tiempo se convierte a “tiempo transcurrido”:
```
addpoints(al, t_s, v);
```
Añade un punto (tiempo, voltaje) a la línea animada sin tener que redibujar todo desde cero.
```
if lvl ~= lastLevel
            lastLevel = lvl;
            if lvl == "LOW"
                disp("Nivel: BAJO");
            elseif lvl == "MED"
                disp("Nivel: MODERADO");
            elseif lvl == "HIGH"
                disp("Nivel: ALTO");
            else
                disp("Nivel: " + lvl);
            end
        end
```
Se compara el lvl actual con lastLevel.
Solo si cambió, imprime en consola.
Traduce LOW/MED/HIGH a español (BAJO/MODERADO/ALTO).
Si llega cualquier otra etiqueta, la imprime tal cual (por ejemplo IDLE, CAL_REST, CAL_BREATH).
```
if toc(lastDraw) > 0.03
        drawnow nocallbacks
        lastDraw = tic;
    end
```
toc(lastDraw) mide cuánto tiempo pasó desde el último refresco.
Si pasó más de 0.03 s (~33 ms), actualiza la figura.
drawnow nocallbacks refresca la gráfica de forma eficiente y reduce “delay”.
Luego reinicia el cronómetro con lastDraw = tic;.
## Resultados de la práctica
Durante la práctica de laboratorio se desarrolló un sistema vestible capaz de capturar en tiempo real las variaciones de la respuesta galvánica cutánea (GSR) utilizando electrodos colocados en la muñeca del sujeto de prueba, de manera inalámbrica por medio de una ESP32. La señal adquirida fue transmitida a un computador para su visualización y análisis, permitiendo observar la evolución temporal del voltaje asociado a la conductancia de la piel.

La gráfica muestra la señal de voltaje registrada durante un periodo de tiempo determinado por el usuario manualmente. En esta señal se observan variaciones graduales del nivel basal junto con incrementos súbitos de amplitud, característicos de la respuesta galvánica cutánea. En dicha gráfica se distinguen dos componentes principales de la señal GSR:

**Componente tónica o estacionaria (SCL – Skin Conductance Level):** corresponde al nivel basal de la señal, que cambia lentamente con el tiempo.

**Componente fásica o transitoria (SCR – Skin Conductance Response):** se manifiesta como incrementos rápidos de la señal seguidos de una recuperación gradual.

Este comportamiento coincide con lo reportado en la literatura sobre actividad electrodérmica, donde las respuestas SCR aparecen como aumentos rápidos en la conductancia cutánea seguidos de un retorno más lento hacia el nivel basal.

Previo a la estimación del nivel de estrés se realizó un proceso de calibración dividido en dos etapas: El periodo de reposo (REST), en el que el sujeto permaneció en reposo durante aproximadamente 35 s para registrar el nivel basal de la señal y tomar un valor promedio de voltaje para umbralizar, y la segunda etapa que fue, el periodo de respiración profunda (BREATH), en el cual, el sujeto de prueba realizó una inspiración profunda seguida de una exhalación lenta, lo cual generó un incremento en la señal GSR.

A partir de los valores registrados como voltaje promedio, se estimaban dos umbrales, los cuales delimitarían el nivel de estrés al cual esta expuesto el sujeto de prueba. Para esto, se clasificó en tres categorías de estrés: Bajo, cuando hay valores de voltaje inferiores a Th1, moderado, cuando hay valores entre Th1 y Th2, y alto, cuando hay valores superiores a Th2.

Durante la ejecución de la prueba se registraron diferentes niveles de estrés, evidenciados por el sistema mediante mensajes en consola tales como BAJO, MODERADO y ALTO. Estas variaciones coinciden con los cambios observados en la señal GSR, donde los picos de voltaje corresponden a incrementos temporales de la conductancia cutánea asociados a activación del sistema nervioso autónomo.

## Análisis de resultados
El sistema desarrollado demostró ser eficaz a la hora de capturar en tiempo real las variaciones de la respuesta galvánica cutánea (GSR) mediante un dispositivo vestible colocado en la muñeca del sujeto. A partir de la señal adquirida fue posible identificar tanto el nivel basal de conductancia cutánea (SCL) como las respuestas transitorias (SCR) asociadas a estímulos fisiológicos, como la respiración profunda realizada durante la etapa de calibración. Durante la medición se observaron incrementos rápidos en el voltaje de la señal, seguidos de una disminución gradual hacia el nivel basal, comportamiento característico de la actividad electrodérmica. A partir de los valores mínimo y máximo obtenidos durante la calibración, se establecieron umbrales que permitieron clasificar el estado del sujeto en niveles de estrés bajo, moderado y alto. 

Desde el punto de vista práctico, el sistema presenta características favorables para su uso en entornos rutinarios como oficinas, aulas de clase o el hogar, ya que el dispositivo vestible permite monitoreo continuo sin restringir significativamente el movimiento del usuario. Además, la visualización en tiempo real facilita la interpretación inmediata del estado fisiológico del sujeto. Sin embargo, la señal GSR puede verse afectada por factores externos como el movimiento, cambios en la temperatura de la piel o variaciones en el contacto de los electrodos, lo que puede introducir ruido o fluctuaciones en la medición.

Por otro lado, su aplicación en el contexto neonatal es mas complicado de introducir, ya que existen diversos factores que dificultan esta tarea. En primer lugar, la piel de los recién nacidos tiene propiedades fisiológicas diferentes (como grosor o actividad de las glándulas sudoríparas), lo que puede modificar la amplitud y dinámica de la señal capturada. Por otro lado, la colocación de los electrodos en la piel de los bebés debe ser realizada de manera cuidadosa para evitar irritación o lesiones cutaneas.

Sin embargo, el principio fisiológico relacionado con la medición de la actividad electrodérmica sigue aplicando de la misma forma, ya que la EDA esta directamente relacionada con la activación del sistema nervioso simpático, el cual responde también a estimulos de estres o incomodidad en los neonatos. 

**¿A qué se debe que una inspiración profunda incremente la magnitud de la respuesta galvánica cutánea (GSR)?:** Una inspiración profunda incrementa la magnitud de la respuesta galvánica cutánea (GSR) debido a la activación del sistema nervioso autónomo, particularmente de su componente simpática. Este sistema regula la actividad de las glándulas sudoríparas ecrinas presentes en la piel. Cuando ocurre una inspiración profunda, se produce una ligera activación fisiológica que aumenta temporalmente la secreción de sudor, incluso si este no es perceptible. La presencia de sudor en la superficie de la piel incrementa su conductividad eléctrica, lo que reduce la resistencia cutánea y genera un aumento en la señal medida de GSR. Este fenómeno se observa como un incremento rápido en la señal seguido de un retorno gradual al nivel basal, comportamiento característico de las respuestas de conductancia cutánea ante estímulos fisiológicos o emocionales.

**¿Cuáles serían las ventajas y desventajas de utilizar la GSR como indicador de estrés?:** La respuesta galvánica cutánea presenta varias ventajas como indicador de estrés, entre ellas que es una técnica no invasiva, fácil de implementar y sensible a cambios en la actividad del sistema nervioso simpático, lo que permite detectar variaciones fisiológicas asociadas a estímulos emocionales o cognitivos. Además, puede integrarse fácilmente en dispositivos vestibles para monitoreo continuo en diferentes entornos. Sin embargo, también presenta algunas limitaciones importantes. La GSR no es un indicador exclusivo del estrés, ya que también puede verse afectada por factores como la temperatura, el movimiento, la respiración o el contacto de los electrodos con la piel. Asimismo, existe una alta variabilidad entre individuos en los niveles basales de conductancia cutánea, lo que hace necesario realizar procesos de calibración para cada sujeto. Por esta razón, en aplicaciones más complejas suele complementarse con otras señales fisiológicas para obtener una estimación más confiable del nivel de estrés.

## Conclusiones

En la presente práctica se desarrolló un sistema vestible capaz de medir y monitorear en tiempo real la respuesta galvánica cutánea (GSR) de un individuo sano, permitiendo observar las variaciones de la conductancia de la piel asociadas a la actividad del sistema nervioso autónomo. A partir de la señal adquirida fue posible identificar tanto el nivel basal de la señal como las respuestas transitorias generadas ante estímulos fisiológicos, como la respiración profunda, lo que evidencia la sensibilidad de la GSR frente a cambios en la activación simpática del organismo.

Durante el proceso de calibración se establecieron valores mínimos y máximos de la señal, a partir de los cuales se definieron umbrales para clasificar el nivel de estrés en categorías de bajo, moderado y alto. Esto permitió que el sistema no solo capturara la señal fisiológica, sino que también interpretara sus variaciones para estimar el estado de activación del sujeto durante la medición.

Los resultados obtenidos demuestran que la respuesta galvánica cutánea es una herramienta útil para detectar cambios en la activación fisiológica asociados a procesos como la concentración, el esfuerzo mental o estímulos emocionales. No obstante, también se evidenció que la señal puede verse influenciada por factores externos como el movimiento del sujeto, la presión de los electrodos o las condiciones de la piel, lo cual puede introducir variaciones adicionales en la medición.

## Bibliografía
[1] W. Boucsein, Electrodermal Activity. Nueva York, NY, Estados Unidos:
Springer Science & Business Media, 2012.

[2] M. A. G. Rivera and J. R. J. Cruz, “MEDICIÓN DE ESTRÉS a PARTIR DE LA FRECUENCIA CARDÍACA y LA RESPUESTA GALVÁNICA DE LA PIEL,” González Rivera | Pistas Educativas, Apr. 09, 2018.

[3] R. M. Fish and L. A. Geddes, “Conduction of electrical current to and through the human body: a review,” Oct. 12, 2009. https://pmc.ncbi.nlm.nih.gov/articles/PMC2763825/

[4] IEC 60479-1. *Effects of current on human beings and livestock – Part 1: General aspects*. International Electrotechnical Commission.

[5] J. G. Webster. *Medical Instrumentation: Application and Design*. 4th ed. Wiley, 2009.

[6] M. L. Loggia, M. Juneau y C. M. Bushnell, “Autonomic responses to heat pain: Heart rate, skin conductance, and their relation to verbal ratings and stimulus intensity,” Pain, vol. 152, no. 3, pp. 592–598, 2011.https://doi.org/10.1016/j.pain.2010.11.032.

[7] M. Breimhorst, S. Sandrock, M. Fechir, N. Hausenblas, C. Geber y F. Birklein, “Do intensity ratings and skin conductance responses reliably discriminate between different stimulus intensities in experimentally induced pain?” The Journal of Pain, vol. 12, no. 1, pp. 61–70, 2011. https://doi.org/10.1016/j.jpain.2010.04.012.

[8] B. Figner y R. O. Murphy, “Using skin conductance in judgment and decision making research,” en A Handbook of Process Tracing Methods for Decision Research, M. Schulte-Mecklenbeck, A. Kuehberger y R. Ranyard, Eds. Nueva York, NY, Estados Unidos: Psychology Press, 2011, pp. 163–184.
