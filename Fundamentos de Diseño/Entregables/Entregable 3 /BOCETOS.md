##SOLUCIÓN 1 (ELEGIDA)

## Descripción de funcionamiento























El sistema de monitoreo basado en **ESP32** se alimenta mediante una **batería de litio de 3.7 V**, cuya energía pasa por el **regulador de voltaje** para suministrar una tensión estable al microcontrolador y a los periféricos, controlando el encendido general mediante el **interruptor**. El cableado interno de energía y señales se organiza a través de las **borneras**.

En operación, el sistema obtiene las medidas de los parámetros mediante la **sonda de pH**, acondicionada por el **sensor de pH**, y el **sensor de humedad**. A partir de estas mediciones, el **ESP32** clasifica el tipo de suelo, identifica un tipo de cultivo apto y presenta los resultados en la **pantalla**, apoyándose en **1 LED** para indicar el estado del sistema.

## Tabla de piezas y ubicación por globo

| Globo | Pieza / Componente | Observación / Ubicación |
| :--- | :--- | :--- |
| **1** | Pantalla | Indicada con el globo **1** en las vistas del plano |
| **2** | 1 LED | Indicador superior derecho en la vista frontal (globo **2**) |
| **3** | Interruptor | Indicado con el globo **3** en la vista frontal |
| **4** | Sonda de pH | Cuerpo inferior / sonda de medición (globo **4**) |
| **5** | Sección trasera / lateral | Indicada con el globo **5** en la vista lateral |
| **6** | Carcasa / Compartimento | Indicado con el globo **6** en la vista lateral |
| **7–10** | Sensor de humedad | Elementos de sonda/medición numerados **7**, **8**, **9** y **10** |
| **8** | Interruptor | Indicado con el globo **8** en el plano |
| **Interno** | Sensor de pH | Módulo electrónico interno de lectura de pH |
| **Interno** | Batería de litio de 3.7 V | Fuente de alimentación interna de 3.7 V |
| **Interno** | Regulador de voltaje | Regulador interno para alimentación del ESP32 |
| **Interno** | Borneras | Bloques de conexión interna para cables |
