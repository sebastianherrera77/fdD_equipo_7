# Lista de Exigencias

### Datos Generales del Proyecto
* **Proyecto:** Sistema portátil para caracterización y diagnóstico fisicoquímico de suelos agrícolas
* **Asignatura:** Fundamentos de Diseño (C1324) — Semestre 2026-II[cite: 1]
* **Docentes:** Mg. Marco Mugaburu / Dr. Harry Rivera[cite: 1]
* **Elaborado por:** José Junior Bances Panaqué
* **Revisado por:** Equipo 07
* **Versión:** 1.0
* **Fecha:** 02/09/2026

---

## 1. Criterios de Definición y Estado del Arte

Los requerimientos y tolerancias de esta lista se formularon siguiendo las etapas iniciales de la metodología VDI 2206[cite: 2]. Los parámetros operativos se alinean con la revisión bibliográfica y técnica desarrollada por el equipo:

* **Artículos científicos:** Rangos de sensibilidad electroquímica y métodos de medición in situ en sustratos agrícolas.
* **Patentes:** Disposiciones geométricas para penetración en suelo y sellado de sensores frente a humedad.
* **Productos comerciales:** Referencias de autonomía, masa total y ergonomía en sondas portátiles de campo.
* **Tesis de ingeniería:** Procedimientos de calibración analítica y errores máximos admisibles frente a patrones certificados.

---

## 2. Matriz de Exigencias Técnicas (VDI 2206)

| Fecha | D / E | Categoría / Requerimiento | Descripción Técnica y Magnitud Cuantificada | Responsable |
| :---: | :---: | :--- | :--- | :--- |
| 02/09/2026 | **E** | **FUNCIÓN PRINCIPAL** | Cuantificar in situ pH, conductividad eléctrica y humedad del estrato arable para determinar aptitud edáfica bajo umbrales FAO/WRB. | General |
| 02/09/2026 | **E** | **GEOMETRÍA** | Dimensiones máximas de la unidad de control: $200 \times 120 \times 60\text{ mm}$. Sonda de inserción con longitud útil $\ge 150\text{ mm}$. | Mecánica |
| 02/09/2026 | **D** | **GEOMETRÍA** | Sonda desmontable con acople rápido roscado para facilitar transporte y recambio. | Mecánica |
| 02/09/2026 | **E** | **CINEMÁTICA** | Dispositivo estacionario durante la lectura. Tiempo de inserción y retiro manual $\le 5\text{ s}$ por punto evaluado. | Mecánica |
| 02/09/2026 | **E** | **FUERZAS** | Resistencia mecánica a carga axial de compresión $\ge 250\text{ N}$ en la punta de penetración sin deformación del chasis. | Mecánica |
| 02/09/2026 | **E** | **MATERIA** | Electrodos de contacto en acero inoxidable 316L (resistente a corrosión por sales y acidez). Carcasa exterior en filamento PETG. | Mecánica |
| 02/09/2026 | **E** | **ENERGÍA** | Alimentación mediante celda Li-Ion recargable (3.7 V nominal, $\ge 2500\text{ mAh}$) con puerto de carga integrado USB-C. | Electrónica |
| 02/09/2026 | **E** | **ENERGÍA** | Autonomía mínima de $6\text{ horas}$ continuas de muestreo activo en campo sin recarga externa. | Electrónica |
| 02/09/2026 | **E** | **SEÑALES (Entradas)** | Adquisición analógica/digital de pH ($3.0 - 10.0 \pm 0.2$), conductividad eléctrica ($0 - 20\text{ dS/m} \pm 3\%$) y humedad ($0 - 100\% \pm 3\%$). | Electrónica |
| 02/09/2026 | **E** | **SEÑALES (Salidas)** | Visualización en pantalla OLED de al menos $128 \times 64\text{ px}$ e indicador visual de estado mediante LED RGB. | Software |
| 02/09/2026 | **E** | **CONTROL** | Microcontrolador de 32 bits con ADC nativo de resolución $\ge 12\text{ bits}$ y frecuencia de reloj base $\ge 80\text{ MHz}$. | Control |
| 02/09/2026 | **E** | **ELECTRÓNICA** | Acondicionamiento analógico con filtro paso bajo pasivo/activo para atenuar ruido inducido por la impedancia del terreno. | Electrónica |
| 02/09/2026 | **E** | **SOFTWARE** | Rutina embebida de calibración por software (dos puntos de referencia) y categorización automática según límites de salinidad FAO. | Software |
| 02/09/2026 | **D** | **COMUNICACIONES** | Almacenamiento local de lecturas en memoria flash interna o microSD, con enlace Bluetooth Low Energy (BLE) para volcado de datos. | Software |
| 02/09/2026 | **E** | **SEGURIDAD** | Grado de protección IP65 en el gabinete electrónico principal frente al ingreso de polvo y salpicaduras de agua o lodo. | Mecánica |
| 02/09/2026 | **E** | **ERGONOMÍA** | Masa total del conjunto (consola + batería + sonda) $\le 750\text{ g}$. Empuñadura antideslizante operable con guantes de trabajo. | Mecánica |
| 02/09/2026 | **E** | **FABRICACIÓN** | Carcasa fabricable mediante manufactura aditiva FDM en el laboratorio de la UPCH; placa de circuito impreso (PCB) para ensamblaje manual[cite: 1, 5]. | Manufactura |
| 02/09/2026 | **E** | **CONTROL DE CALIDAD** | Error relativo experimental $< 5\%$ al contrastar contra soluciones patrón de calibración ($pH\ 4.01 / 7.00$ y CE $1413\ \mu\text{S/cm}$). | Validación |
| 02/09/2026 | **E** | **MONTAJE** | Ensamble modular fijado por tornillería métrica M3 con insertos metálicos, evitando pegamentos o cierres irreversibles. | Mecánica |
| 02/09/2026 | **E** | **TRANSPORTE** | Estructura resistente a caídas accidentales desde $1.0\text{ m}$ sobre superficie de tierra compactada; dimensiones aptas para morral estándar. | Mecánica |
| 02/09/2026 | **E** | **USO** | Operación confiable bajo condiciones ambientales de costa: temperatura de $10^\circ\text{C}$ a $38^\circ\text{C}$ y humedad relativa de hasta $90\%$. | General |
| 02/09/2026 | **E** | **MANTENIMIENTO** | Limpieza rápida de varillas con agua destilada y paño no abrasivo; retención de calibración operativa durante al menos 50 ciclos. | Operativo |
| 02/09/2026 | **E** | **COSTOS** | Costo directo acumulado en componentes electrónicos y materiales de manufactura $\le 280\text{ PEN}$ por unidad prototipo. | Gestión |
| 02/09/2026 | **E** | **PLAZOS** | Banco de pruebas funcional validado para la Semana 8; prototipo integrado y operativo para la Semana 16 del ciclo académico[cite: 1, 5]. | Gestión |
