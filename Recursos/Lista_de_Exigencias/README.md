# Lista de Exigencias - Proyecto de Diagnóstico Fisicoquímico de Suelos Agrícolas
**Metodología de Diseño: VDI 2206**  
**Responsable:** José Bances Panaqué  
**Entregable:** E1 / Recursos  

---

## 1. Ficha Técnica del Documento
* **Proyecto:** Sistema Portátil de Diagnóstico y Clasificación Fisicoquímica de Suelos Agrícolas según Criterios FAO
* **Cliente / Cátedra:** Fundamentos de Diseño (UPCH) - Mg. Ing. Marco Mugaburu / Harry Rivera
* **Edición:** 1.0 (Preliminar Adaptable)
* **Fecha:** Septiembre 2026

---

## 2. Marco de Adaptabilidad
Esta Lista de Exigencias traduce la problemática de degradación de suelos (ODS 15.3, 12.2, 12.4, 13.1) en especificaciones medibles. Se encuentra abierta a calibración según los hallazgos del estado del arte recopilados por el equipo:
* **Artículos científicos (Johan):** Rangos de precisión electroquímica y métodos ISFET / reflectometría.
* **Patentes (José Luis):** Mecanismos de penetración y arquitecturas de sondas protegidas.
* **Productos comerciales (Alessandra):** Parámetros estándar de mercado en portabilidad y autonomía.
* **Tesis (Sebastián):** Procedimientos de validación experimental en campo.

---

## 3. Matriz de Exigencias Técnicas (VDI 2206)

| Categoría | E / D | Descripción Técnica y Magnitud Cuantificada | Dominio / Responsable |
| :--- | :---: | :--- | :--- |
| **Función Principal** | **E** | Medir y clasificar in situ parámetros fisicoquímicos del suelo (pH, conductividad eléctrica y humedad) para determinar aptitud edáfica bajo umbrales FAO/WRB. | General (Todos) |
| **Geometría** | **E** | Dimensiones de la carcasa principal $\le 200 \times 120 \times 60\text{ mm}$. Sonda de inserción $\ge 150\text{ mm}$ de profundidad efectiva. | Mecánico |
| **Geometría** | **D** | Sonda modular intercambiable mediante conexión estanca de acople rápido. | Mecánico |
| **Cinemática** | **E** | Dispositivo estacionario durante la lectura. Tiempo de inserción y extracción $\le 5\text{ s}$. | Mecánico |
| **Fuerzas** | **E** | Resistencia estructural a compresión axial en punta $\ge 250\text{ N}$ para penetración en suelo compactado sin deformación. | Mecánico |
| **Materia** | **E** | Electrodos de contacto en acero inoxidable 316L (resistente a corrosión ácida/salina). Carcasa en polímero técnico (PETG/ABS). | Mecánico |
| **Energía** | **E** | Batería recargable Li-Ion (3.7V nominal, $\ge 2500\text{ mAh}$) con circuito integrado de carga USB-C. | Electrónico |
| **Energía** | **E** | Autonomía de operación continua en campo $\ge 6\text{ horas}$ de muestreo activo. | Electrónico |
| **Señales (Entrada)** | **E** | Rango de lectura de pH: $3.0 - 10.0$ ($\pm 0.2$). Conductividad Eléctrica: $0 - 20\text{ dS/m}$ ($\pm 3\%$). Humedad volumétrica: $0 - 100\%$ ($\pm 3\%$). | Electrónico |
| **Señales (Salida)**| **E** | Despliegue visual directo en pantalla OLED/LCD ($\ge 128 \times 64\text{ px}$) y codificación de alerta mediante LED RGB de estado. | Software |
| **Control** | **E** | Unidad de procesamiento de 32 bits, frecuencia de reloj $\ge 80\text{ MHz}$, con ADC nativo $\ge 12\text{ bits}$. | Control / Embebidos |
| **Electrónica** | **E** | Etapa de acondicionamiento analógico con filtro paso bajo para supresión de ruido por acoplamiento capacitivo del suelo. | Electrónico |
| **Software** | **E** | Algoritmo de calibración de dos puntos y procesamiento local para correlación de datos con índices de salinidad/acidez FAO. | Software |
| **Comunicaciones** | **D** | Registro local en memoria no volátil (Flash/MicroSD) y transmisión inalámbrica opcional (BLE/WiFi). | Software |
| **Seguridad** | **E** | Protección IP65 en el compartimento electrónico contra polvo y proyecciones de lodo o agua. | Mecánico |
| **Ergonomía** | **E** | Peso total en mano $\le 750\text{ g}$. Mango con grip antideslizante operable con guantes agrícolas estándar. | Mecánico |
| **Fabricación** | **E** | Chasis manufacturable mediante impresión 3D FDM en el laboratorio UPCH y PCB diseñada para ensamble manual. | Manufactura |
| **Control Calidad** | **E** | Margen de error $< 5\%$ frente a patrones de calibración certificados ($pH\ 4.01 / 7.00$ y CE $1413\ \mu\text{S/cm}$). | Validación |
| **Montaje** | **E** | Ensamble modular mediante tornillería métrica M3, permitiendo mantenimiento y cambio de piezas sin daño estructural. | Mecánico |
| **Transporte** | **E** | Resistencia a impactos por caídas accidentales desde $1.0\text{ m}$ sobre suelo agrícola. Factor de forma apto para morral. | Mecánico |
| **Uso** | **E** | Rango térmico de operación ambiental de $10^\circ\text{C}$ a $38^\circ\text{C}$ con humedad relativa ambiente de hasta $90\%$. | General |
| **Mantenimiento** | **E** | Procedimiento de limpieza rápida de electrodos con agua destilada y secado sin pérdida de calibración en $\ge 50$ lecturas. | Operativo |
| **Costos** | **E** | Costo directo total de componentes electrónicos y materiales de manufactura $\le 280\text{ PEN}$ por unidad prototipo. | Gestión |
| **Plazos** | **E** | Integración del circuito y validación de banco para Semana 8; prototipo funcional TRL 3-4 para Semana 16. | Gestión |
