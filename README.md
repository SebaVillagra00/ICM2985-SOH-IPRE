# ICM2985-SOH-IPRE
Investigación de pregrado: Estado del arte de SOH de baterías de ion litio.

* Docente guía: David Acuña
* Alumno: Sebastian Villagra
* Fecha investigación: 2024-1

## Data University of Cambridge (EIS Cambridge)
Data publicada en "Identifying degradation patterns of lithium ion batteries from impedance spectroscopy using machine learning" (Zhang, Tang, Zhang, Wang, Stimming & Lee, 2020) https://www.nature.com/articles/s41467-020-15235-7.

Carpeta contiene:
* Paper de Nature Comunications (IF: 16.6).
* Data frames para IOS.
* Data frames para Windows.

Cada Data frame está contenido en un archivo .txt con las siguientes columnas:
* time/s: tiempo en que se mide la muestra.
* cycle number: ciclo de carga de la batería.
* freq/Hz: frecuencia de la señal de input.
* Re(Z)/Ohm: Parte resistiva de la impedancia.
* Im(Z)/Ohm: Parte reactiva de la impedancia.
* |Z|/Ohm: Magnitud de la impedancia.
* Phase(Z)/deg: Ángulo de la impedancia (grados sexagesimales).

### Modelo de batería y método de prueba
Las baterías con las que se genera la base de datos son 12 baterías de ion litio tipo moneda Eunicell LR2032 de 45 mAh. Estas baterías son puestas a prueba bajo tres condiciones de temperatura constante (8 a 25 °C, 2 a 35 °C y 2 a 45 °C). Las pruebas de cada batería se hacen en 9 estados distintos de carga (SOC) para cada batería. 

Esta información está contenida en el nombre de cada archivo .txt de la siguiente forma:
**EIS_state_i_tCn**. Donde:

* i: número del estado de carga (I - IX).
* t: temperatura a la que se testea la batería (25, 35, 45).
* n: número de la celda a probar.

Además, la carga está hecha a razón constante de 1C (45 mA) hasta los 4.2 V y la descarga a razón constante de 2C (90 mA) hasta los 3 V.

**Modelo de batería**: 45 mAh Eunicell LR2032 Li-ion coin cells.
Referencia en Amazon: https://www.amazon.com/LIR2032-Rechargeable-Certified-Bluetooth-Controllers/dp/B07MHYQHY3?th=1.


##
