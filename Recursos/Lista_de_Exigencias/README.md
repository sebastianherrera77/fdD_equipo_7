# Lista de Exigencias

### Datos Generales del Proyecto
* **Proyecto:** Sistema portátil para caracterización y diagnóstico fisicoquímico de suelos agrícolas
* **Asignatura:** Fundamentos de Diseño (C1324) — Semestre 2026-II
* **Docentes:** Mg. Marco Mugaburu / Dr. Harry Rivera
* **Elaborado por:** José Junior Bances Panaqué
* **Revisado por:** Equipo 07
* **Fecha:** 02/09/2026

---

## 1. Criterios de Definición y Estado del Arte

Los requerimientos y tolerancias de esta lista se formularon siguiendo las etapas iniciales de la metodología VDI 2206. Los parámetros operativos se alinean con la revisión bibliográfica y técnica desarrollada por el equipo:

* **Guía MINAM (D.S. N°002-2013-MINAM):** protocolo de muestreo y determinación de puntos de campo — usada para el diseño del procedimiento de medición, no como fuente de los umbrales de pH/CE (ver nota en sección 2.1).
* **Clasificación agronómica de pH y salinidad (CE):** basada en tablas estándar de referencia internacional (metodología Richards/USDA, adoptada regionalmente).
* **Productos comerciales y tesis de ingeniería:** referencias orientativas de autonomía, masa y ergonomía en sondas portátiles de campo — tratadas como *supuestos de diseño*, pendientes de validar con datasheets reales antes de fabricar.

> **Nota de trazabilidad:** las filas marcadas con 🔵 tienen respaldo bibliográfico verificable. Las marcadas con 🟡 son supuestos de diseño razonables (basados en productos similares) que el equipo debe confirmar o ajustar con datos propios antes de la etapa de prototipado.

---

## 2. Matriz de Exigencias Técnicas (VDI 2206)

### 2.1 Rangos de referencia (verificados)

| Parámetro | Rango | Clasificación |
|---|---|---|
| pH | < 5.0 | Fuertemente ácido |
| pH | 5.0 – 6.5 | Moderadamente ácido |
| pH | 6.6 – 7.3 | Neutro |
| pH | 7.4 – 8.5 | Medianamente alcalino |
| pH | > 8.5 | Fuertemente alcalino |
| CE (dS/m, extracto saturación) | < 2 | No salino |
| CE (dS/m, extracto saturación) | 2 – 4 | Ligeramente salino |
| CE (dS/m, extracto saturación) | 4 – 8 | Medianamente salino |
| CE (dS/m, extracto saturación) | 8 – 16 | Fuertemente salino |
| CE (dS/m, extracto saturación) | > 16 | Muy fuertemente salino |

*Fuente: clasificación agronómica estándar de pH y salinidad por conductividad eléctrica, ampliamente adoptada en guías de diagnóstico de suelos.*

### 2.2 Exigencias y Deseos del sistema

| D/E | Categoría | Descripción Técnica | Respaldo | Responsable |
|:---:|---|---|:---:|---|
| E | FUNCIÓN PRINCIPAL | Cuantificar in situ pH, conductividad eléctrica y humedad del estrato arable para determinar aptitud edáfica según los rangos de la sección 2.1. | 🔵 | General |
| E | GEOMETRÍA | Dimensiones máximas de la unidad de control: 200 × 120 × 60 mm. Sonda de inserción con longitud útil ≥ 150 mm. | 🟡 | Mecánica |
| D | GEOMETRÍA | Sonda desmontable con acople rápido roscado para facilitar transporte y recambio. | 🟡 | Mecánica |
| E | CINEMÁTICA | Dispositivo estacionario durante la lectura. Tiempo de inserción y retiro manual ≤ 5 s por punto evaluado. | 🟡 | Mecánica |
| E | FUERZAS | Resistencia mecánica a carga axial de compresión adecuada para penetrar suelo agrícola compactado sin deformación del chasis (valor a confirmar con ensayo de penetrometría). | 🟡 | Mecánica |
| E | MATERIA | Electrodos de contacto en acero inoxidable 316L (resistente a corrosión por sales y acidez). Carcasa exterior en filamento PETG. | 🟡 | Mecánica |
| E | ENERGÍA | Alimentación mediante celda Li-Ion recargable (3.7 V nominal), con puerto de carga USB-C. Capacidad a definir según consumo real del circuito. | 🟡 | Electrónica |
| E | ENERGÍA | Autonomía mínima de una jornada de campo (objetivo referencial: 4–6 h de muestreo activo) sin recarga externa. | 🟡 | Electrónica |
| E | SEÑALES (Entradas) | Adquisición de pH (rango 3.0–10.0), conductividad eléctrica (0–20 dS/m) y humedad volumétrica, con precisión suficiente para distinguir las clases de la sección 2.1. | 🔵 | Electrónica |
| E | SEÑALES (Salidas) | Visualización de resultados en pantalla legible en campo (mín. 128 × 64 px) e indicador visual de estado. | 🟡 | Software |
| E | CONTROL | Microcontrolador con ADC de resolución suficiente para resolver las variaciones de señal esperadas en los rangos de pH/CE definidos. | 🟡 | Control |
| E | ELECTRÓNICA | Acondicionamiento analógico (filtro) para atenuar ruido inducido por la impedancia variable del terreno. | 🟡 | Electrónica |
| E | SOFTWARE | Rutina embebida de calibración (mínimo dos puntos de referencia) y categorización automática según los umbrales de la sección 2.1. | 🔵 | Software |
| D | COMUNICACIONES | Almacenamiento local de lecturas (memoria flash/microSD) con enlace inalámbrico (BLE) para volcado de datos. | 🟡 | Software |
| E | SEGURIDAD | Grado de protección adecuado (objetivo IP54–IP65) del gabinete electrónico frente a polvo y humedad, propio de uso en campo abierto. | 🟡 | Mecánica |
| E | ERGONOMÍA | Sistema portátil, operable por una persona; masa total y empuñadura aptas para trabajo prolongado en campo (a definir con prueba de usuario). | 🟡 | Mecánica |
| E | FABRICACIÓN | Carcasa fabricable mediante manufactura aditiva FDM en el laboratorio de la UPCH; PCB apto para ensamblaje manual. | 🟡 | Manufactura |
| E | CONTROL DE CALIDAD | Verificación del error de medición contrastando contra soluciones patrón de calibración certificadas (ej. pH 4.01/7.00, CE 1413 µS/cm), con tolerancia a definir tras pruebas. | 🟡 | Validación |
| E | MONTAJE | Ensamble modular con tornillería estándar, evitando pegamentos o cierres irreversibles, para permitir mantenimiento. | 🟡 | Mecánica |
| E | TRANSPORTE | Estructura resistente a manipulación y traslado en campo (morral estándar), sin daño a componentes de medición. | 🟡 | Mecánica |
| E | USO | Operación confiable bajo condiciones ambientales representativas de la costa peruana (temperatura y humedad relativa elevadas). | 🟡 | General |
| E | MANTENIMIENTO | Limpieza rápida de electrodos/sondas con agua destilada y paño no abrasivo; retención de calibración durante uso repetido. | 🟡 | Operativo |
| E | COSTOS | Costo directo de componentes y manufactura del prototipo dentro del presupuesto asignado por el curso (monto a definir con el equipo). | 🟡 | Gestión |
| E | PLAZOS | Banco de pruebas funcional para la Semana 8; prototipo integrado y operativo para la Semana 16 del ciclo académico. | 🟡 | Gestión |

---

## 3. Trazabilidad

Este documento consolida los hallazgos de los Issues #32 a #36 (revisión normativa, selección de variables, vinculación ODS y brecha diagnóstica) y sirve de base para las etapas de conceptualización del sistema, en coordinación con el resto del equipo.

**Pendiente antes de prototipado:** validar con el equipo los valores marcados 🟡 (fuerza de penetración, capacidad de batería, IP, tolerancias de calibración, presupuesto) contra datasheets de componentes reales o pruebas propias, para que la lista quede completamente defendible ante el docente.

*Documento elaborado por José Junior Bances Panaqué — Issue #37.*
