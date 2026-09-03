# Lista de Exigencias – Sistema de Diagnóstico Edáfico en Campo

## 1. Contexto del problema

Los suelos agrícolas de la costa peruana presentan procesos crecientes de
salinización y degradación, evaluados hoy mediante análisis de laboratorio
destructivos (lentos y costosos) o inspección visual empírica (poco
confiable). Esta brecha diagnóstica dificulta el monitoreo oportuno de la
aptitud del suelo, en contraste con los lineamientos de la FAO (WRB) y la
normativa MINAM (D.S. N°002-2013-MINAM).

**Vinculación ODS:** Meta principal 15.3 (lucha contra la desertificación,
restauración de tierras degradadas). Metas secundarias: 12.2, 12.4 y 13.1.

## 2. Metodología

Siguiendo la norma VDI 2206, los requerimientos se clasifican en:

- **E (Exigencia):** condición obligatoria, no negociable.
- **D (Deseo):** condición deseable, mejora el sistema pero no es crítica.

Y se agrupan por dominio: mecánico, energético, señales, control y seguridad.

## 3. Matriz de Exigencias y Deseos

### 3.1 Dominio Mecánico

| Tipo | Descripción |
|------|-------------|
| E | El sensor de penetración/compactación debe soportar suelos con dureza típica de campo agrícola costero sin deformarse. |
| E | La carcasa debe ser resistente a polvo y humedad (mín. IP54) para uso en campo abierto. |
| E | El dispositivo debe ser portátil, con peso menor a 2 kg para operación manual de una persona. |
| D | La estructura debe permitir intercambio rápido de sondas/electrodos sin herramientas. |
| D | El diseño debe minimizar componentes para facilitar mantenimiento en campo. |

### 3.2 Dominio Energético

| Tipo | Descripción |
|------|-------------|
| E | El sistema debe operar con batería recargable con autonomía mínima de 4 horas de uso continuo. |
| E | El consumo energético debe permitir al menos 30 mediciones completas por carga. |
| D | Debe contar con indicador visual de nivel de batería. |
| D | Carga mediante USB-C para compatibilidad con equipos estándar. |

### 3.3 Dominio de Señales

| Tipo | Descripción |
|------|-------------|
| E | El sistema debe medir conductividad eléctrica aparente (CE) con precisión suficiente para distinguir rangos de salinidad según MINAM/FAO. |
| E | El sistema debe medir pH del suelo en un rango de 3 a 10. |
| E | El sistema debe medir humedad volumétrica del suelo. |
| E | El sistema debe registrar el grado de compactación del suelo. |
| D | Las mediciones deben poder exportarse digitalmente (Bluetooth/USB) para análisis posterior. |

### 3.4 Dominio de Control

| Tipo | Descripción |
|------|-------------|
| E | El sistema debe mostrar resultados de forma inmediata (menor a 30 segundos por medición) en pantalla legible en campo. |
| E | El sistema debe permitir calibración previa a cada sesión de medición. |
| D | Debe incluir alertas automáticas cuando un parámetro esté fuera del rango admisible normado. |
| D | Debe permitir almacenar histórico de mediciones por punto geográfico. |

### 3.5 Dominio de Seguridad

| Tipo | Descripción |
|------|-------------|
| E | El dispositivo no debe representar riesgo eléctrico para el operador (bajo voltaje, aislamiento adecuado). |
| E | Las sondas de penetración deben tener protección para evitar lesiones al usuario durante el traslado. |
| D | Debe incluir manual de uso y advertencias de seguridad en campo. |

## 4. Trazabilidad

Este documento consolida los hallazgos de los Issues #32 a #36 (revisión
normativa, selección de variables, vinculación ODS y brecha diagnóstica), y
sirve de base para las etapas de conceptualización del sistema, en
coordinación con el resto del equipo.

*Documento elaborado por José Junior Bances Panaque — Issue #37.*
