# Lista de Exigencias

### Datos Generales del Proyecto
* **Proyecto:** Sistema portátil para caracterización y diagnóstico fisicoquímico de suelos agrícolas
* **Asignatura:** Fundamentos de Diseño — Semestre 2026-II
* **Docentes:** Mg. Marco Mugaburu / Dr. Harry Rivera
* **Elaborado por:** José Junior Bances Panaque
* **Revisado por:** Equipo FdD07
* **Fecha:** 02/09/2026

---

## 1. Criterios de Definición

Los requerimientos de esta lista se formularon siguiendo las etapas iniciales de la metodología VDI 2206, considerando la revisión de la Guía para Muestreo de Suelos del MINAM (D.S. N°002-2013-MINAM) y la clasificación agronómica estándar de pH y salinidad. Esta es una primera versión: se irá refinando conforme avance la revisión bibliográfica del equipo (artículos científicos, patentes, productos comerciales y tesis relacionadas, actualmente en curso).

## 2. Rangos de referencia

| Parámetro | Rango | Clasificación |
|---|---|---|
| pH | < 5.0 | Fuertemente ácido |
| pH | 5.0 – 6.5 | Moderadamente ácido |
| pH | 6.6 – 7.3 | Neutro |
| pH | 7.4 – 8.5 | Medianamente alcalino |
| pH | > 8.5 | Fuertemente alcalino |
| CE (dS/m) | < 2 | No salino |
| CE (dS/m) | 2 – 4 | Ligeramente salino |
| CE (dS/m) | 4 – 8 | Medianamente salino |
| CE (dS/m) | 8 – 16 | Fuertemente salino |
| CE (dS/m) | > 16 | Muy fuertemente salino |

## 3. Matriz de Exigencias Técnicas (VDI 2206)

| D/E | Categoría | Descripción Técnica | Responsable |
|:---:|---|---|---|
| E | FUNCIÓN PRINCIPAL | Cuantificar conductividad eléctrica y humedad del estrato arable para determinar aptitud edáfica según los rangos de la sección 2. | General |
| E | GEOMETRÍA | Dimensiones máximas de la unidad de control: 200 × 120 × 60 mm. Sonda de inserción con longitud útil ≥ 150 mm. | Mecánica |
| D | GEOMETRÍA | Sonda desmontable con acople rápido roscado para facilitar transporte y recambio. | Mecánica |
| E | CINEMÁTICA | Dispositivo estacionario durante la lectura. Tiempo de inserción y retiro manual ≤ 5 s por punto evaluado. | Mecánica |
| E | FUERZAS | Resistencia mecánica adecuada para penetrar suelo agrícola compactado sin deformación del chasis. | Mecánica |
| E | MATERIA | Electrodos de contacto en acero inoxidable 316L. Carcasa exterior en filamento PETG. | Mecánica |
| E | ENERGÍA | Alimentación mediante celda Li-Ion recargable (3.7 V nominal), con puerto de carga USB-C. | Electrónica |
| E | ENERGÍA | Autonomía mínima de una jornada de campo (4–6 h de muestreo activo) sin recarga externa. | Electrónica |
| E | SEÑALES (Entradas) | Adquisición de pH (3.0–10.0), conductividad eléctrica (0–20 dS/m) y humedad volumétrica del suelo. | Electrónica |
| E | SEÑALES (Salidas) | Visualización de resultados en pantalla legible en campo e indicador visual de estado. | Software |
| E | CONTROL | Microcontrolador con ADC de resolución suficiente para resolver las variaciones de señal esperadas. | Control |
| E | ELECTRÓNICA | Acondicionamiento analógico (filtro) para atenuar ruido inducido por la impedancia del terreno. | Electrónica |
| E | SOFTWARE | Rutina embebida de calibración (mínimo dos puntos de referencia) y categorización automática según los rangos de la sección 2. | Software |
| D | COMUNICACIONES | Almacenamiento local de lecturas con enlace inalámbrico (BLE) para volcado de datos. | Software |
| E | SEGURIDAD | Grado de protección adecuado (IP54–IP65) del gabinete electrónico frente a polvo y humedad. | Mecánica |
| E | ERGONOMÍA | Sistema portátil, operable por una persona, con empuñadura apta para trabajo prolongado en campo. | Mecánica |
| E | FABRICACIÓN | Carcasa fabricable mediante manufactura aditiva FDM en el laboratorio de la UPCH; PCB apto para ensamblaje manual. | Manufactura |
| E | CONTROL DE CALIDAD | Verificación del error de medición contrastando contra soluciones patrón de calibración certificadas. | Validación |
| E | MONTAJE | Ensamble modular con tornillería estándar, evitando pegamentos o cierres irreversibles. | Mecánica |
| E | TRANSPORTE | Estructura resistente a manipulación y traslado en campo (morral estándar). | Mecánica |
| E | USO | Operación confiable bajo condiciones ambientales representativas de la costa peruana. | General |
| E | MANTENIMIENTO | Limpieza rápida de electrodos/sondas con agua destilada y paño no abrasivo. | Operativo |
| E | COSTOS | Costo directo de componentes y manufactura del prototipo dentro del presupuesto asignado por el curso. | Gestión |
| E | PLAZOS | Banco de pruebas funcional para la Semana 8; prototipo integrado y operativo para la Semana 16. | Gestión |

## 4. Trazabilidad

Este documento consolida los hallazgos de los Issues #32 a #36 (revisión normativa, selección de variables, vinculación ODS y brecha diagnóstica), y sirve de base para las etapas de conceptualización del sistema, en coordinación con el resto del equipo.

*Documento elaborado por José Junior Bances Panaque — Issue #37.*
