# Estimación Textural y Diagnóstico Fisicoquímico de Suelos Agrícolas

## 1. Problemática: Limitaciones en la Clasificación y Diagnóstico Fisicoquímico de Suelos Agrícolas en el Perú

En el sector agrícola, los análisis de suelo en laboratorio son indispensables para tomar decisiones sobre la nutrición de los cultivos y evitar la degradación ambiental (1). Sin embargo, las metodologías convencionales basadas en muestreos de campo y ensayos de laboratorio suelen ser lentas, costosas y de carácter destructivo (2,3), lo que dificulta su adopción por parte de pequeños y medianos productores en el Perú.

La falta de una caracterización oportuna genera diagnósticos inadecuados de las propiedades físicas y químicas (textura, retención de humedad, pH y conductividad eléctrica), limitando la disponibilidad de nutrientes y el desarrollo radicular (4,5). Esta deficiencia provoca el uso ineficiente del agua de riego e insumos químicos, favoreciendo la pérdida de tierras de cultivo por salinización (un problema recurrente en valles costeros como la cuenca del río Jequetepeque (6) y la degradación por lixiviación de contaminantes (1,7). Frente a estas limitaciones, surge la necesidad de implementar herramientas basadas en sensores no destructivos y modelos indirectos que permitan la caracterización e inferencia física del suelo de forma rápida y accesible en campo (2,3).

Esta problemática se vuelve aún más crítica al considerar que en el Perú el recurso suelo de aptitud agropecuaria es un bien sumamente escaso, representando únicamente el 7% del territorio nacional (9), del cual solo el 3.8% corresponde a tierras aptas para cultivos en limpio y el 2.1% a cultivos permanentes (9). Asimismo, este recurso se encuentra severamente amenazado por procesos de deterioro: al menos un 40% de los suelos agrícolas de la Costa están afectados por salinización y mal drenaje (9), más del 60% de los suelos agropecuarios de la Sierra sufren erosión de mediana a extrema gravedad (9), y en la Amazonía cerca de 5 millones de hectáreas han sido abandonadas por pérdida de fertilidad debido a técnicas inadecuadas (9).

---
## 2. Fundamentos de la Problemática dentro de los Objetivos de Desarrollo Sostenible (ODS)

El prototipo se enfoca en abordar la problemática de degradación de tierras como eje principal, alineándose con la Agenda 2030 mediante metas e indicadores específicos ajustados al alcance de validación técnica del proyecto:

### ODSPrincipal

* **ODS 15: Vida de Ecosistemas Terrestres**
  * **Meta 15.3 (Aporte directo del proyecto):** Proporcionar una herramienta de monitoreo temprano in situ para la detección de indicadores de salinización, erosión y degradación física del suelo.
  * **Indicador 15.3.1:** Registro y seguimiento continuo de parámetros de salinidad (Conductividad Eléctrica) y acidez (pH) en parcelas de prueba.
  * **Fundamentación:** Dado que más de 8 millones de hectáreas sufren erosión severa y el 40% de los valles costeros peruanos se ven afectados por salinización (9), el aporte central del prototipo es servir como un instrumento accesible para el monitoreo frecuente de la salud del suelo, proporcionando bases técnicas para prevenir la pérdida de fertilidad y la degradación de los agroecosistemas (4,6,7).

---

### ODS Secundarios

* **ODS 12: Producción y Consumo Responsables**
  * **Meta 12.4 (Aporte complementario):** Promover el uso racional de insumos agrícolas y agua mediante el conocimiento de la retención hídrica y química del suelo.
  * **Indicador 12.4.2:** Reducción en la sobreaplicación de fertilizantes sintéticos a través del diagnóstico previo de la muestra.
  * **Fundamentación:** Como soporte a la conservación del suelo, el prototipo permite prescribir la fertilización y el riego según las necesidades reales del cultivo y la textura estimada (1,7). Esto previene la contaminación de acuíferos subterráneos por lixiviación de nitratos y optimiza el uso del agua (1,5).

* **ODS 2: Hambre Cero**
  * **Meta 2.3 (Aporte complementario):** Contribuir al fortalecimiento de la productividad de pequeños productores agrícolas mediante herramientas de diagnóstico de bajo costo.
  * **Indicador 2.3.1:** Optimización del rendimiento agrícola por unidad de superficie cultivada.
  * **Fundamentación:** Al conocer el estado del suelo y su clasificación textural (4), el agricultor puede tomar decisiones informadas para seleccionar el cultivo más apto en parcelas reducidas, mejorando la productividad de tierras agrícolas escasas (1,4,9).

---

## 3. Enfoque del Proyecto y Propuesta de Valor

El proyecto consiste en un **prototipo accesible basado en sistemas embebidos** que estima la clase textural y las condiciones fisicoquímicas del suelo sin recurrir a análisis de laboratorio tradicionales o costosos (2,3). El dispositivo mide en tiempo real **humedad, temperatura, pH y conductividad eléctrica (CE)**.

A partir de la respuesta termo-electromagnética de la muestra, el firmware deduce su comportamiento físico (retención hídrica e intercambio iónico) y la clasifica dentro de las 12 categorías del **Triángulo Textural de Suelos del USDA** (ej. franco, arcillo-arenoso o arcillo-limoso) (2,3,8). Finalmente, cruza la textura estimada con los niveles de pH y salinidad para emitir un **diagnóstico automatizado de aptitud agrícola** (4).

---

## 4. Beneficios 

* **Ahorro y Eficiencia:** Reduce costos de análisis tradicionales de laboratorio y evita gastos innecesarios en fertilizantes al ajustar las dosis según el diagnóstico real del suelo (1,7).
* **Toma de Decisiones In Situ:** Proporciona recomendaciones inmediatas sobre qué cultivos sembrar según el tipo de suelo, previniendo pérdidas de cosecha por incompatibilidad (4,5).
* **Protección del Recurso Suelo y Agua:** Optimiza la programación del riego de acuerdo con la capacidad de retención del suelo y ayuda a monitorear la salinización, frenando la degradación de las tierras (6,7,9).
* **Democratización Tecnológica:** Acerca el uso de herramientas de agricultura de precisión a comunidades rurales con limitados recursos (1,4).

---


### Referencias Bibliográficas

1.	López-González, F. J., Ponce-García, O. C., Trejo-Téllez, L. I., Mendoza-Araujo, S., & Navarrete-Saldaña, E. S. (2026). Del campo al laboratorio: La calidad en los análisis de suelos. Voces del Suelo, Agricultura y Medioambiente, 4(2), 16-26. https://doi.org/10.28940/vocesdelsuelo.v4i2.2836
2.	Martínez-Ríos, J. J., & Monger, H. C. (2002). SOIL CLASSIFICATION IN ARID LANDS WITH THEMATIC MAPPER DATA. https://jornada.nmsu.edu/files/bibliography/JRN00368.pdf
3.	B, E. J. O. (1995). Características físico-químicas del suelo y su incidencia en la absorción de nutrimentos, con énfasis en el cultivo de la palma de aceite. Palmas, 16(1), 31-39. https://publicaciones.fedepalma.org/index.php/palmas/article/view/461
4.	Jahnsen Cisneros, M. (2014). Impacto de la represa Gallito Ciego en la pérdida de tierras de cultivo por salinización en la Cuenca Baja del río Jequetepeque 1980-2003. http://hdl.handle.net/20.500.12404/5125
5.	Navarro Bravo, A., Figueroa Sandoval, B., Martínez Menes, M., González Cossio, F., & Osuna Ceja, E. S. (2008). Indicadores físicos del suelo bajo labranza de conservación y su relación con el rendimiento de tres cultivos. Agricultura técnica en México, 34(2), 151-158. http://www.scielo.org.mx/scielo.php?script=sci_abstract&pid=S0568-25172008000200002&lng=es&nrm=iso&tlng=es
6.	Villarroel, J. S., Espinoza, H. A., Hinojoza, J. L. T., Diaz, L. F. B., Magallanes, J. L. M., & Pasache, J. L. D. (2026). Determinantes fisicoquímicos del suelo y su influencia en la productividad de Ipomoea batatas L. en valles costeros áridos de Perú. Alfa Revista de Investigación en Ciencias Agronómicas y Veterinarias, 10(29), 1-11. https://doi.org/10.33996/revistaalfa.v10i29.478
7.	Puma Chuquichampi, J., & Teran Corredor, I. E. (2022). La importancia de la clasificación de suelos tropicales por la metodología MCT en contraste con las recomendaciones AASHTO para el proyecto vial Carretera Pe—5N DV Cabo Leveau departamento de San Martin. https://repositorio.usil.edu.pe/entities/publication/fc9f3a18-2cc8-49a4-96d7-2c3bca74eb0c
8.	Narvaez, H. (s. f.). iNVERSIÓN SOCIAL PARA EL DESARROLLO SOSTENIBLE. https://fechac.org.mx/app_fechac/_files/_img/_documents/012821-160142_rf-1-03compromisodefechacconlosodsrev1.pdf?gad_source=1&gad_campaignid=20014956691&gbraid=0AAAAABsloXpyztw9ymjiuG3H4cZDV4-Aj&gclid=EAIaIQobChMI2qDkrIyDlwMVv01IAB0XlxGjEAAYASAAEgLRP_D_BwE
9.	Suelo. (s. f.). Recuperado 22 de septiembre de 2026, de https://www.midagri.gob.pe/portal/43-sector-agrario/suelo



