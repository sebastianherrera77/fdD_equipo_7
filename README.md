***EQUIPO 07 - FUNDAMENTOS DE DISEÑO***

Carrera de Ingenieria Ambiental / Ingeniería informatica /Ingeniería Industrial

Universidad Peruana Cayetano Heredia
---
🌐**Descripción del Equipo**

Somos el Equipo 07 del curso fundamentos de Diseño 2026-2, conformado por estudiantes de la carrera de Ingeniería Ambiental / Informática / Industrial.
Nuestro objetivo es aplicar la metodología de diseño para generar soluciones innovadoras con impacto social, tecnológico y ambiental.

Nos interesa trabajar en los siguientes Objetivos de Desarrollo Sostenible (ODS):

ODS 6: AGUA LIMPIA Y SANEAMIENTO

ODS 13: ACCIÓN POR EL CLIMA

ODS 15: VIDA DE ECOSISTEMAS TERRESTRES

---

# Clasificación textural de suelos y evaluación de aptitud de cultivo basada en humedad, temperatura y conductividad eléctrica

## 1. Problemática: Limitaciones en la Clasificación Textural y la Evaluación de Aptitud de Suelos Agrícolas en el Perú

En el Perú, el suelo de aptitud agropecuaria es el recurso más escaso del país, pues abarca alrededor del 7% del territorio y, según la clasificación de uso mayor de ONERN (1985), el 3.8% del territorio es apto para cultivos en limpio y el 2.1% para cultivos permanentes (9). A esta escasez se suma su deterioro: se estima que al menos el 40% de los suelos agrícolas de la Costa presenta salinización y mal drenaje, más del 60% de los suelos agropecuarios de la Sierra sufre erosión de mediana a extrema gravedad, unos 8 millones de hectáreas están severamente erosionadas a nivel nacional y, en la Amazonía, unas 5 millones de hectáreas han sido abandonadas por pérdida de fertilidad y erosión (9). Si bien el MIDAGRI advierte que esta clasificación es antigua (9), las cifras permiten dimensionar la magnitud del problema. A escala local, además, la pérdida de tierras de cultivo por salinización se ha estudiado en la cuenca baja del río Jequetepeque (6).

Dado este panorama, elegir bien qué cultivar en cada parcela es una decisión crítica, ya que depende de conocer la textura, el pH y la conductividad eléctrica (CE) del suelo (4,5). Sin embargo, en un país con más de 2.2 millones de unidades agropecuarias (8), la caracterización convencional requiere muestreo de campo y análisis de laboratorio, procesos lentos y laboriosos (2,3), cuyos resultados confiables, además, exigen procedimientos de calidad y personal capacitado (1). En consecuencia, su uso rutinario en parcelas pequeñas es limitado, y el productor termina decidiendo qué sembrar sin información inmediata sobre la clase textural de su suelo ni sobre su aptitud para el cultivo que desea establecer.

Por ello, el problema se delimita a las parcelas agrícolas de pequeños y medianos productores del Perú, y se centra en la estimación de la textura del suelo a partir de la humedad, la temperatura, el pH y la CE, con el fin de emitir un diagnóstico preliminar de aptitud para un cultivo objetivo. En cambio, quedan fuera de su alcance la medición de nutrientes (nitrógeno, carbono, sulfatos) y el reemplazo del análisis químico de laboratorio, pues se busca ofrecer una primera orientación y no un análisis completo. En este sentido, la escasez y el deterioro del recurso (9), la demora y la especialización que exigen los análisis convencionales (1,2,3) y la influencia documentada de la textura, el pH y la CE sobre el desarrollo de los cultivos (4,5) justifican contar con una herramienta de campo rápida y accesible. Así, el problema puede resumirse en la falta de herramientas accesibles y rápidas que permitan clasificar la textura del suelo en campo y relacionarla con el pH y la CE para determinar su aptitud para un cultivo específico.

---
## 2. Fundamentos de la Problemática dentro de los Objetivos de Desarrollo Sostenible (ODS)

El prototipo se enfoca en abordar la problemática de degradación de tierras como eje principal, alineándose con la Agenda 2030 mediante metas e indicadores específicos ajustados al alcance de validación técnica del proyecto:

### ODSPrincipal

* **ODS 15: Vida de Ecosistemas Terrestres**
  * **Meta 15.3:** Proporcionar una herramienta de monitoreo temprano in situ para la detección de indicadores de salinización, erosión y degradación física del suelo.
  * **Indicador 15.3.1:** Registro y seguimiento continuo de parámetros de salinidad (Conductividad Eléctrica) y acidez (pH) en parcelas de prueba.
  * **Fundamentación:** Dado que más de 8 millones de hectáreas sufren erosión severa y el 40% de los valles costeros peruanos se ven afectados por salinización (9), el aporte central del prototipo es servir como un instrumento accesible para el monitoreo frecuente de la salud del suelo, proporcionando bases técnicas para prevenir la pérdida de fertilidad y la degradación de los agroecosistemas (4,6,7).

---

### ODS Secundarios

* **ODS 12: Producción y Consumo Responsables**
  * **Meta 12.4:** Promover el uso racional de insumos agrícolas y agua mediante el conocimiento de la retención hídrica y química del suelo.
  * **Indicador 12.4.2:** Reducción en la sobreaplicación de fertilizantes sintéticos a través del diagnóstico previo de la muestra.
  * **Fundamentación:** Como soporte a la conservación del suelo, el prototipo permite prescribir la fertilización y el riego según las necesidades reales del cultivo y la textura estimada (1,7). Esto previene la contaminación de acuíferos subterráneos por lixiviación de nitratos y optimiza el uso del agua (1,5).

* **ODS 2: Hambre Cero**
  * **Meta 2.3:** Contribuir al fortalecimiento de la productividad de pequeños productores agrícolas mediante herramientas de diagnóstico de bajo costo.
  * **Indicador 2.3.1:** Optimización del rendimiento agrícola por unidad de superficie cultivada.
  * **Fundamentación:** Al conocer el estado del suelo y su clasificación textural (4), el agricultor puede tomar decisiones informadas para seleccionar el cultivo más apto en parcelas reducidas, mejorando la productividad de tierras agrícolas escasas (1,4,9).

---

## 3. Enfoque del Proyecto y Propuesta de Valor

El proyecto consiste en un Sistema embebido para la clasificación textural de suelos y evaluación de aptitud de cultivo basada en humedad, temperatura y conductividad eléctrica del suelo sin recurrir a análisis de laboratorio tradicionales o costosos (2,3). El dispositivo mide en tiempo real **humedad, temperatura, pH y conductividad eléctrica (CE)**.

A partir de las lecturas de humedad, temperatura, pH y conductividad eléctrica (CE) de la muestra, el sistema infiere su comportamiento físico (retención hídrica) y la clasifica dentro de las 12 categorías del Triángulo Textural de Suelos del USDA (ej. franco, arcillo-arenoso o arcillo-limoso) (2,3,8). Finalmente, cruza la textura estimada con los niveles de pH y CE y con los parámetros del cultivo objetivo elegido por el usuario, para emitir un diagnóstico preliminar de aptitud agrícola (4).
---

## 4. Beneficios 

* **Ahorro y Eficiencia:** Reduce costos de análisis tradicionales de laboratorio y evita gastos innecesarios en fertilizantes al ajustar las dosis según el diagnóstico real del suelo (1,7).
* **Toma de Decisiones In Situ:** Proporciona recomendaciones inmediatas sobre qué cultivos sembrar según el tipo de suelo, previniendo pérdidas de cosecha por incompatibilidad (4,5).
* **Protección del Recurso Suelo y Agua:** Optimiza la programación del riego de acuerdo con la capacidad de retención del suelo y ayuda a monitorear la salinización, frenando la degradación de las tierras (6,7,9).
* **Democratización Tecnológica:** Acerca el uso de herramientas de agricultura de precisión a comunidades rurales con limitados recursos (1,4).

---

## REFERENCIAS BIBLIOGRAFICAS

1.	López-González, F. J., Ponce-García, O. C., Trejo-Téllez, L. I., Mendoza-Araujo, S., & Navarrete-Saldaña, E. S. (2026). Del campo al laboratorio: La calidad en los análisis de suelos. Voces del Suelo, Agricultura y Medioambiente, 4(2), 16-26. https://doi.org/10.28940/vocesdelsuelo.v4i2.2836
2.	Martínez-Ríos, J. J., & Monger, H. C. (2002). SOIL CLASSIFICATION IN ARID LANDS WITH THEMATIC MAPPER DATA. https://jornada.nmsu.edu/files/bibliography/JRN00368.pdf
3.	B, E. J. O. (1995). Características físico-químicas del suelo y su incidencia en la absorción de nutrimentos, con énfasis en el cultivo de la palma de aceite. Palmas, 16(1), 31-39. https://publicaciones.fedepalma.org/index.php/palmas/article/view/461
4.	Jahnsen Cisneros, M. (2014). Impacto de la represa Gallito Ciego en la pérdida de tierras de cultivo por salinización en la Cuenca Baja del río Jequetepeque 1980-2003. http://hdl.handle.net/20.500.12404/5125
5.	Navarro Bravo, A., Figueroa Sandoval, B., Martínez Menes, M., González Cossio, F., & Osuna Ceja, E. S. (2008). Indicadores físicos del suelo bajo labranza de conservación y su relación con el rendimiento de tres cultivos. Agricultura técnica en México, 34(2), 151-158. http://www.scielo.org.mx/scielo.php?script=sci_abstract&pid=S0568-25172008000200002&lng=es&nrm=iso&tlng=es
6.	Villarroel, J. S., Espinoza, H. A., Hinojoza, J. L. T., Diaz, L. F. B., Magallanes, J. L. M., & Pasache, J. L. D. (2026). Determinantes fisicoquímicos del suelo y su influencia en la productividad de Ipomoea batatas L. en valles costeros áridos de Perú. Alfa Revista de Investigación en Ciencias Agronómicas y Veterinarias, 10(29), 1-11. https://doi.org/10.33996/revistaalfa.v10i29.478
7.	Puma Chuquichampi, J., & Teran Corredor, I. E. (2022). La importancia de la clasificación de suelos tropicales por la metodología MCT en contraste con las recomendaciones AASHTO para el proyecto vial Carretera Pe—5N DV Cabo Leveau departamento de San Martin. https://repositorio.usil.edu.pe/entities/publication/fc9f3a18-2cc8-49a4-96d7-2c3bca74eb0c
8.	Suelo. (s. f.). Recuperado 22 de septiembre de 2026, de https://www.midagri.gob.pe/portal/43-sector-agrario/suelo
  

----------

📸 **Fotografia del equipo**

----<img width="4032" height="3024" alt="image" src="https://github.com/user-attachments/assets/888a5b24-4f43-4b1c-86f6-fe9a15e42b77" />

## Integrantes

| Foto | Integrante | Rol | intereses | 
|:----|:-----------|:---|:-------|
| <img width="240" height="288" alt="image" src="https://github.com/user-attachments/assets/229baebf-81cb-4079-9bcb-3f9cc8ef5a81" />| Johan Daymar Chara Franco | Lider de equipo | Innovacion social, analisis de datos y estructuracion de imformacion.|
|![sebastian.png](./Recursos/sebastian.png) | Wilmer Sebastian Herrera Neira | Diseñador frontend | diseño, programación |
|<img width="240" height="288" alt="ale" src="https://github.com/user-attachments/assets/3b7af26c-7b55-4fe3-8d5a-4c02d38d1507" />| Alessandra Nicol Palomino Lima| Documentación | redacción técnica |
|<img width="240" height="288" alt="image" src="https://github.com/user-attachments/assets/6f32328b-37b6-4e85-aef1-4313297dd407" />| José Luis Cepida Castellares | Responsable de investigación| Química, Física, Biología y Cálculo |
| <img width="240" height="288" alt="image" src="https://github.com/user-attachments/assets/14c15ef0-18b5-4a34-94b0-80de2f6d0147" />| José Junior Bances Panaque| Programador | Programación, análisis de datos, simulación |

**Resumen Final**
Este README presenta información resumida de cada uno de los integrantes de este equipo, así como lo qué nos motiva y en qué ODS queremos enfocar y orientar nuestro trabajo durante el curso
