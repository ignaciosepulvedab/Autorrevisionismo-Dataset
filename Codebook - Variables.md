**ECONOMÍA Y COMERCIO**

**Eventos arancelarios _(tariff_events)_**
- **Descripción:** El número de veces que Estados Unidos implementó acciones arancelarias conforme a las secciones 122, 201, 232, 301 del código estadounidense, así como el IEPPA y otras modificaciones de los derechos arancelaros del HTS sin contar resoluciones sobre derechos antidumping y compensatorios. Conteo simple.
- **Proceso de recolección:** Se usó un script de Python para conectarse a la API de la Federal Register, obteniendo un conteo anual de eventos arancelarios conforme a los recursos legales anteriormente señalados.
- **Conducta esperada:** Ante un hegemón autorrevisionista, se esperaria que exista un mayor número de casos correspondientes a eventos arancelarios.
- **Período comprendido:** 1995-2025
- **Fuente:** Federal Register API

**Resoluciones sobre derechos antidumping (AD) y compensatorios (CVD) _(ad_cvd)_**
- **Descripción:** El número de veces que Estados Unidos emitió resoluciones sobre derechos antidumping y compensatorios, entendidas como medidas arancelarias enfocadas en contrarrestar presuntas prácticas anticompetitivas por parte de actores en el extranjero. Conteo simple.
- **Proceso de recolección:** Se usó un script de Python para conectarse a la API de la Federal Register, obteniendo un conteo anual de resoluciones sobre derechos antidumping y compensatorios.
- **Conducta esperada:** Un hegemón autorrevisionista haría uso de los derechos antidumping y compensatorios como herramienta comercial, complementando la imposición tradicional de aranceles. Dicho esto, se reconoce que la emisión de resoluciones sobre derechos antidumping y compensatorios está permitida bajo los lineamientos de la OMC, por lo que no constituye una conducta autorrevisionista en sí misma.
- **Período comprendido**: 1995-2025
- **Fuente**: Federal Register API 

**Tasa arancelaria promedio NMF _(mfn_rate)_**
- **Descripción:** Promedio de tasas arancelarias aplicadas a mercancías conforme al criterio de Nación Más Favorecida de la Organización Mundial del Comercio (OMC). Cifra calculada conforme a una agregación de la totalidad de líneas arancelarias vigentes.
- **Proceso de recolección:** Filtrado de datos provenientes de la OMC.
- **Conducta esperada:** Un hegemón autorrevisionista tendería a aplicar tasas arancelarias más altas a los miembros de la OMC con los que no tiene acuerdos comerciales vigentes. Dicho esto, existen dudas respecto a si la información proveída a la OMC ante tal eventualidad sería fidedigna.
- **Período comprendido:** 1996-2025
- **Fuente:** OMC — Tariff & Trade Data

**Tasa arancelaria preferencial promedio *(wto_preferential_rate)***
- **Descripción:** Cifra calculada a partir del promedio de las tasas preferenciales vigentes, entendidas como arreglos comerciales preferenciales otorgados por Estados Unidos a ciertos socios comerciales bajo excepciones legales autorizadas por la OMC al principio de Nación Más Favorecida.
- **Proceso de recolección:** Filtrado de datos provenientes de la OMC.
- **Conducta esperada:** Un hegemón autorrevisionista buscaría aumentar las tasas arancelarias, independiente de la vigencia de acuerdos comerciales preferenciales.
- **Período comprendido:** 1997-2025
- **Fuente:** OMC — Tariff & Trade Data

**Tasa arancelaria efectiva sobre importaciones totales *(effective_tariffs)***
- **Descripción**: Proporción de ingresos de aduana como fracción del valor total de bienes importados, independientemente de si estos están sujetos a aranceles o no.
- **Proceso de recolección**: Cálculo manual a partir de las tablas presentes en el sitio DataWeb de la USITC.
- **Conducta esperada**: Se teoriza que un hegemón autorrevisionista sería propenso a aumentar las tasas arancelarias efectivas sobre importaciones totales en comparación a otros períodos.
- **Período comprendido**: 1993-2025
- **Fuente:** USITC DataWeb

**Tasa arancelaria efectiva sobre importaciones gravadas *(dutiable_rate)***
- **Descripción**: Proporción de ingresos de aduana como fracción del valor total de bienes importados sujetos a aranceles.
- **Proceso de recolección**: Cálculo manual a partir de las tablas presentes en el sitio DataWeb de la USITC.
- **Conducta esperada**: Un hegemón autorrevisionista sería propenso a aumentar las tasas arancelarias efectivas sobre importaciones gravadas en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente**: USITC DataWeb

**Porcentaje de importaciones exentas de aranceles *(duty_free_share)***
- **Descripción**: Proporción de importaciones no gravadas, medida a partir del valor de los bienes no sujetos a aranceles como porcentaje del valor total de mercancías importadas al país durante el año de observación.
- **Proceso de recolección**: Cálculo manual a partir de las tablas presentes en el sitio DataWeb de la USITC.
- **Conducta esperada**: Bajo un hegemón autorrevisionista, se espera que la proporción de importaciones no gravadas tienda a disminuir en comparación a otros períodos.
- **Período comprendido**: 1993-2025
- **Fuente**: USITC DataWeb

**Política arancelaria *(tariff_policy)***
- **Descripción:** Medida en que el discurso oficial del hegemón aboga por la imposición y aumento de aranceles, restricciones comerciales o medidas de represalia comercial unilaterales. Mayor puntaje representa un mayor grado de autorrevisionismo.
- **Proceso de recolección**: Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a la política comercial y asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada**: Un hegemón autorrevisionista debería abogar activa y deliberadamente por medidas que restrinjan el libre comercio, particularmente un aumento de las tasas arancelarias vigentes.
- **Período comprendido:** 1993-2025
- **Fuente**: American Presidency Project

**Sanciones económicas unilaterales activas *(active_unilateral_economic_sanctions)***
- **Descripción:** Número de programas de sanciones financieras o comerciales impuestos unilateralmente activos durante el año de observación. Conteo simple.
- **Proceso de recolección:** Recuento anual de casos señalados por el Global Sanctions Database.
- **Conducta esperada:** Un hegemón autorrevisionista se vería incentivado a aumentar sustancialmente el número de sanciones económicas activas, imponiendolas mayormente de manera unilateral.
- **Período comprendido:** 1993-2025
- **Fuente:** Global Sanctions Database

**Sanciones económicas unilaterales impuestas *(new_unilateral_economic_sanctions)***
- **Descripción:** Número de programas de sanciones financieras o comerciales impuestos unilateralmente durante el año de observación. Conteo simple.
- **Proceso de recolección:** Recuento anual de casos señalados por el Global Sanctions Database.
- **Conducta esperada:** Un hegemón autorrevisionista se vería incentivado a aumentar sustancialmente el número de sanciones económicas, imponiendolas mayormente de manera unilateral.
- **Período comprendido:** 1993-2025
- **Fuente:** Global Sanctions Database

**Grado de coordinación multilateral en la imposición de sanciones económicas *(mult_economic_sanctions_rate)***
- **Descripción:** Proporción de sanciones económicas impuestas de manera unilateral durante el año de observación, entendiendose como aquellos programas de carácter financiero y/o comercial impuestos por Estados Unidos junto a otros países, incluyendo los foros multilaterales en los que participa (por ejemplo: G7).
- **Proceso de recolección:** Calculo con script de elaboración propia a partir de casos señalados por el Global Sanctions Database.
- **Conducta esperada:** Un hegemón autorrevisionista debería evidenciar un menor grado de coordinación multilateral en la imposición de sanciones económicas.
- **Período comprendido:** 1993-2025
- **Fuente:** Global Sanctions Database

**Acuerdos comerciales vigentes *(active_trade_agreements)***
- **Descripción**: Número de acuerdos comerciales activos durante un respectivo año de observación, considerando tratados de libre comercio (TLC/FTA), tratados de inversión bilateral (TIB/BIT) y Acuerdos Marco de Comercio e Inversión (AMCI/TIFA). Conteo simple.
- **Proceso de recolección**: Recuento anual con script de R a partir de datos recopilados manualmente usando información disponible en las fuentes.
- **Conducta esperada**: Bajo un liderazgo autorrevisionista, el hegemón reduciría el número de acuerdos comerciales vigentes. Nótese, sin embargo, que este también podría eludir sus cláusulas sin abolirlos formalmente.
- **Período comprendido:** 1993-2025
- **Fuente**: USTR — Trade Agreements · UNCTAD — IIA Navigator

**Acuerdos comerciales firmados *(signed_trade_agreements)***
- **Descripción**: Número de acuerdos comerciales firmados durante un respectivo año de observación, considerando tratados de libre comercio (TLC/FTA), tratados de inversión bilateral (TIB/BIT) y Acuerdos Marco de Comercio e Inversión (AMCI/TIFA). Conteo simple.
- **Proceso de recolección**: Recuento anual con script de R a partir de datos recopilados manualmente usando información disponible en las fuentes.
- **Conducta esperada**: Bajo un liderazgo autorrevisionista, el hegemón no se vería incentivado a firmar acuerdos de libre comercio.
- **Período comprendido:** 1993-2025
- **Fuente**: USTR — Trade Agreements · UNCTAD — IIA Navigator

**Acuerdos comerciales finalizados *(finished_trade_agreements)***
- **Descripción**: Número de acuerdos comerciales expirados, retirados o rescindidos durante el respectivo año de observación, considerando tratados de libre comercio (TLC/FTA), tratados de inversión bilateral (TIB/BIT) y Acuerdos Marco de Comercio e Inversión (AMCI/TIFA). Conteo simple.
- **Proceso de recolección**: Recuento anual con script de R a partir de datos recopilados manualmente usando información disponible en las fuentes.
- **Conducta esperada**: Un hegemón autorrevisionista tendería a retirarse de acuerdos comerciales. Es importante, sin embargo, considerar la posibilidad de que los eventos contabilizados puedan ser producto de la voluntad de la otra parte más que del hegemón.
- **Período comprendido:** 1993-2025
- **Fuente**: USTR — Trade Agreements · UNCTAD — IIA Navigator

**Disputas vigentes que involucran a EE. UU. en el Órgano de Solución de Diferencias de la OMC *(active_wto_disputes)***
- **Descripción:** recuento de casos activos dentro del Órgano de Solución de Diferencias de la OMC en los que Estados Unidos es parte.
- **Proceso de recolección:** Recuento anual con script de R a partir de datos recopilados manualmente desde el sitio web de la OMC.
- **Comportamiento esperado:** Si bien se estima que el hegemón dejaría de participar activamente en los procedimientos de arbitraje de la OMC al adoptar una conducta autorrevisionista, la acumulación de casos estancados traídos en su contra podría significar que el número total de disputas activas aumente.
- **Período comprendido:** 1995-2025
- **Fuente:** OMC — Solución de Diferencias

**Disputas abiertas por EE.UU. dentro del Órgano de Solución de Diferencias de la OMC *(new_wto_complainant)***
- **Descripción:** número de casos abiertos por Estados Unidos en el Órgano de Solución de Diferencias de la OMC durante el año de observación. Conteo simple.
- **Proceso de recolección:** Recuento anual con script de R a partir de datos recopilados manualmente desde el sitio web de la OMC
- **Comportamiento esperado:** considerando que la participación en procesos de arbitraje puede ser considerado como un procedimiento integral dentro del funcionamiento del orden internacional liberal, se espera que un hegemón hóstil hacia sus reglas deje de participar activamente en este tipo de instancias.
- **Período comprendido:** 1995-2025
- **Fuente:** OMC — Solución de Diferencias

**Disputas abiertas contra EE.UU. dentro del Órgano de Solución de Diferencias de la OMC *(new_wto_respondent)***
- **Descripción:** Número de casos abiertos dentro del Órgano de Solución de Diferencias de la OMC en los que EE.UU. actúa como la parte demandada. Conteo simple.
- **Proceso de recolección:** Recuento anual con script de R a partir de datos recopilados manualmente desde el sitio web de la OMC
- **Conducta esperada:** Asumiendo que bajo un liderazgo autorrevisionista EE.UU. comete prácticas comerciales indebidas, se esperaría que el número de casos traidos en contra del hegemón aumentaría. Este, sin embargo, se vería incentivado a estancar los procesos en su contra, por lo que resulta necesario triangular con otros indicadores sobre el desarrollo de los casos dentro de la OMC
- **Período comprendido:** 1995-2025
- **Fuente:** OMC — Solución de Diferencias

**Resolución efectiva de disputas que involucran a EE. UU. en el Órgano de Solución de Diferencias de la OMC *(wto_success)***
- **Descripción:** Tasa de éxito de procesos que involucran a Estados Unidos dentro del Órgano de Solución de Diferencias de la OMC. Se considera que el hallazgo de soluciones consensuadas o la emisión efectiva de fallos constituyen un cierre adecuado de estos procesos.
- **Proceso de recolección:** Cálculo con ayuda de script de R a partir de datos recopilados manualmente desde el sitio web de la OMC. Para cada año de observación se agrega el número de casos resueltos, estancados y retirados unilateralmente, calculando el éxito como proporción relativa al número de casos totales.
- **Comportamiento esperado:** En caso de que el hegemón exiba una conducta autorrevisionista, se espera que la tasa de resolución efectiva de disputas dentro de la OMC se reduzca.
- **Período comprendido:** 1995-2025
- **Fuente:** OMC — Solución de Diferencias

**Grado de estancamiento de disputas que involucran a EE. UU. en el Órgano de Solución de Diferencias de la OMC *(wto_stagnation)***
- **Descripción:** Proporción de disputas comerciales involucrando a Estados Unidos que se ven estancados dentro del mecanismo de solución de diferencias de la OMC. Para que un caso se entienda como estancado este debe quedar inconcluso debido a falta de cooperacion de las partes sin que sea formalmente rescindido.
- **Proceso de recolección:** Cálculo con ayuda de script de R a partir de datos recopilados manualmente desde el sitio web de la OMC.
- Comportamiento esperado: Se espera que la presencia de hegemón autorrevisionista produzca un aumento en el número de casos estancados dentro de la OMC.
- Período comprendido: 1995-2025
- Fuente: OMC — Solución de Diferencias

**Cumplimiento de sentencias del Órgano de Solución de Diferencias de la OMC *(wto_compliance)***
- **Descripción:** La medida en que el hegemón respeta y cumple con las resoluciones emitidas por los tribunales de la OMC. Entendido como la tasa de cumplimiento entre los fallos emitidos por la OMC en los que EE.UU. actúa como demandado. Mayor puntaje indica una mayor tasa de cumplimiento.
- **Proceso de recolección:** Evaluación manual del complimiento efectivo por parte de Estados Unidos respecto a las resoluciones emitidas por el Órganismo de Solución de Diferencias de la OMC en casos donde actúa como la parte demandada. El cumplimiento, en este caso, se define como la adopción de recomendaciones y acatamiento de los informes publicados por la OMC.
- **Comportamiento esperado:** Se asume que una potencia autorrevisionista tendería a no respetar las resoluciones de la OMC, traduciendose en una tasa de cumplimiento sustancialmente menor que en otros períodos.
- **Período comprendido:** 1996-2025
- **Fuente:** OMC — Solución de Diferencias

**COORDINACIÓN INTERNACIONAL**

**Incorporación a organizaciones internacionales *(igo_accession)***
- **Descripción:** Recuento de organizaciones intergubernamentales a las que Estados Unidos se adherió durante el año de observación.
- **Proceso de recolección:** Accediendo al yearbook de la UIA, fue posible filtrar y obtener archivos .csv conteniendo listados anuales de organizaciones intergubernamentales activas a las que el gobierno de Estados Unidos se encuentra afiliados. Estos archivos fueron posteriormente comparados y procesados usando un script de python, el cual proporcionó detalles sobre la incorporación de Estados Unidos a nuevas organizaciones internacionales. Conteo simple.
- **Comportamiento esperado:** Se espera que un hegemón autorrevisionista disminuya o paralice la incorporación de Estados Unidos a nuevas organizaciones internacionales.
- **Período comprendido:** 2002-2025
- **Fuente:** UIA Yearbook Online

**Retiro de organizaciones internacionales *(igo_withdrawals)***
- **Descripción:** Recuento de casos en los que Estados Unidos dejó de participar activamente en organizaciones internacionales de carácter intergubernamental durante el año de observación.
- **Proceso de recolección:**  Accediendo al yearbook de la UIA, fue posible filtrar y obtener archivos .csv conteniendo listados anuales de organizaciones intergubernamentales activas a las que el gobierno de Estados Unidos se encuentra afiliados. Estos archivos fueron posteriormente comparados y procesados usando un script de python, el cual proporcionó detalles sobre la disagregación estadounidense en organizaciones internacionales. Conteo simple.
- **Comportamiento esperado:** Se espera que bajo una gestión autorrevisionista, se produzca un mayor número de retiros consumados de organizaciones internacionales por parte de Estados Unidos que en otros períodos.
- **Período comprendido:** 2002-2025
- **Fuente:** UIA Yearbook Online

**Participación en organizaciones internacionales *(igo_participation)***
- **Descripción:** Recuento de organizaciones intergubernamentales con participación activa de Estados Unidos
- **Proceso de recolección:** Accediendo al yearbook de la UIA, fue posible filtrar y obtener archivos .csv conteniendo listados anuales de organizaciones intergubernamentales activas a las que el gobierno de Estados Unidos se encuentra afiliados. Estos archivos fueron posteriormente comparados y procesados usando un script de python. Conteo simple.
- **Comportamiento esperado**: Se espera que ante un hegemón autorrevisionista reduzca el involucramiento internacional de Estados Unidos, incluyendo la participación en organizaciones intergubernamentales. Este recuento, por tanto, debería tender a bajar a medida que el autorrevisionismo surge como fuerza política en Estados Unidos.
- **Período comprendido:** 2002-2025
- **Fuente:** UIA Yearbook Online

**Utilización del veto en el Consejo de Seguridad de la ONU *(unsc_veto_usage)***
- **Descripción:** Número de ocasiones en las que Estados Unidos hizo uso de su derecho a veto dentro del Consejo de Seguridad de las Naciones Unidas. Conteo simple.
- **Proceso de recolección:** Filtración y recuento anual de casos correspondientes a vetos estadounidenses dentro del consejo usando un script de R.
- **Comportamiento esperado**: Se espera que el autorrevisionismo hegemónico se manifieste sectorialmente como una mayor utilización del derecho a veto en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:** ONU DPPA — Vetos del CSNU · Sciences Po — Security Council Vetoes

**Tasa de utilización del veto en el Consejo de Seguridad de la ONU *(unsc_veto_rate)***
- **Descripción:** Utilización del veto por parte de Estados Unidos en relación a la totaliad de votos llevados a cabo en el Consejo de Seguridad durante el año de observación.
- **Proceso de recolección:** Recuento anual de vetos dividido por el número total  de votaciones efectuadas en el mismo período, uso de R.
- **Comportamiento esperado**: Se espera que el autorrevisionismo hegemónico se manifieste sectorialmente como una mayor utilización del derecho a veto en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:** ONU DPPA — Vetos del CSNU · Sciences Po — Security Council Vetoes

**Contribuciones a organizaciones internacionales *(igo_contributions)***
- **Descripción:** Presupuesto anual dedicado a cubrir las obligaciones financieras y otro tipo de cuotas asignadas a Estados Unidos producto de su participación en organizaciones internacionales. Cifras en dólares
- **Proceso de recolección:** Recuento manual de contribuciones financieras a organizaciones internacionales a partir de las fuentes.
- **Comportamiento esperado:** Se asume que las contribuciones a organizaciones internacionales se vean reducidas sustancialmente bajo gestión autorrevisionista.
- **Período comprendido:** 2001-2025
- **Fuente:** Depto. de Estado — Intl. Affairs Budget · CRS RL30515

**Contribuciones asignadas al presupuesto ordinario de la ONU *(un_payable_contributions)***
- **Descripción:** Cifra anual de las contribuciones que Estados Unidos debe abonar al presupuesto ordinario de la ONU, compuesta por la suma de sus cuotas asignadas y la deuda pendiente respecto a años anteriores. Cifras en dólares.
- **Proceso de recolección:** Entrada manual de datos disponibles en la página web del Comité de Cuotas de las Naciones Unidas, completando la información faltante mediante la triangulación de cifras.
- **Comportamiento esperado:** Se espera que las contribuciones asignadas al presupuesto ordinario de la ONU tiendan a aumentar en caso de que la morosidad por parte del hegemón se intensifique.
- **Período comprendido:** 1993-2025
- **Fuente:** ONU – Comité de Contribuciones

**Contribuciones efectuadas al presupuesto ordinario de la ONU *(un_contributions)***
- **Descripción:** Pagos efectuados por Estados Unidos al presupuesto ordinario de la ONU durante el año de observación. Cifras en dólares.
- **Proceso de recolección:** Entrada manual de datos disponibles en la página web del Comité de Cuotas de las Naciones Unidas, completando la información faltante mediante la triangulación de cifras.
- Conducta esperada: En caso de existir una gestión autorrevisionista, se teoriza que las contribuciones estadounidenses al presupuesto ordinario de la ONU tendrán a disminuir sustancialmente respecto a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:** ONU – Comité de Contribuciones

**Deuda pendiente respecto al presupuesto ordinario de la ONU *(un_pending_contributions)***
- **Descripción:** Pagos pendientes respecto a las contribuciones estadounidenses al presupuesto ordinario de la ONU durante el año de observación.
- **Proceso de recolección:** Entrada manual de datos disponibles en la página web del Comité de Cuotas de las Naciones Unidas, completando la información faltante mediante la triangulación de cifras.
- **Conducta esperada**: Se estima que una posible gestión autorrevisionista de las contribuciones al presupuesto ordinario de la ONU daría lugar a un aumento de la deuda estadounidense al sistema de Naciones Unidas.
- **Período comprendido:** 1993-2025
- **Fuente:** ONU – Comité de Contribuciones

**Presupuesto total de ayuda exterior *(foreign_assistance_budget)***
- **Descripción:** Fondos gubernamentales estadounidenses destinados a ayuda internacional según las subfunciones 151 y 152 del presupuesto anual. Cifras en millones de dólares. Se comprende tanto la ayuda en materia de asistencia humanitaria y desarrollo (subfunción 151) como la asistencia militar (subfunción 152)
- **Proceso de recolección:** Entrada manual de datos a partir de la fuente.
- **Conducta esperada:** Se estima que una reducción presupuestaria en materia de ayuda exterior podría considerarse como una manifestación sectorial del autorrevisionismo hegemónico.
- **Período comprendido: 1993-2025**
- **Fuente:** OMB — Historical Tables

**Presupuesto destinado a desarrollo internacional y ayuda humanitaria *(international_development_budget)***
- **Descripción:** Fondos gubernamentales estadounidenses destinados a ayuda internacional según la subfunción 151 del presupuesto anual, correspondiente a la asistencia humanitaria y el desarrollo internacional. Se excluye, por tanto, la asistencia militar de esta cifra. Cifras en millones de dólares.
- **Proceso de recolección:** Recuento de datos obtenidos a partir de un recuento manual de cifras desglosadas en la fuente, particularmente el presupuesto anual del gobierno federal estadounidense y sus pagos según la subfunción 151.
- **Conducta esperada:** Se estima que una reducción presupuestaria en materia de desarrollo internacional y ayuda humanitaria podría considerarse como una manifestación sectorial del autorrevisionismo hegemónico.
- **Período comprendido:** 1993-2025
- **Fuente:** OMB — Historical Tables

**Presupuesto de la Agencia de EE.UU. para el Desarrollo Internacional *(usaid_budget)***
- **Descripción:** Presupuesto anual de la Agencia de EE.UU. para el Desarrollo Internacional (USAID) en su conjunto, calculada a partir de los pagos recibidos por la agencia durante el período. Cifras en millones de dólares.
- **Proceso de recolección:** Entrada manual de datos a partir de cifras desglosadas en la fuente.
- **Conducta esperada:** Dado el propósito y misión de USAID, se espera que su presupuesto se vea reducido sustancialmente bajo la influencia del autorrevisionismo.
- **Período comprendido:** 2001-2024
- **Fuente:** ForeignAssistance.gov

**Ayuda exterior como porcentaje del presupuesto federal *(foreign_assistance_share)***
- **Descripción:** Porcentaje del gasto federal estadounidense dedicado a la ayuda exterior según las subfunciones 151 y 152 del presupuesto.
- **Proceso de recolección:** Cálculo de cifra en R usando información recopilada manualmente a partir de la información disponible en las fuentes respecto al gasto federal en ayuda exterior y el presupuesto anual del gobierno federal de los Estados Unidos en su conjunto.
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista despriorizaría el gasto en materia de ayuda exterior, resultando en una reducción relativa en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:** OMB – Historical Tables

**Postura discursiva respecto a la ayuda exterior *(foreign_aid_stance)***
- **Descripción:** Medida en que el discurso del hegemón refleja una postura crítica y/o contraria a la ayuda exterior, presentándola como un desperdicio presupuestario o como algo contrario a los intereses estadounidenses. Mayor puntaje indica mayor grado de conducta autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a la ayuda externa y asignandole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- Conducta esperada: Se espera que un hegemón autorrevisionista se posicione como crítico al gasto en materia de ayuda internacional y desarrollo, proponiendo una reducción presupuestaria para focalizar el gasto a nivel doméstico.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**SEGURIDAD Y DEFENSA**

**Cuestionamiento u condicionamiento de compromisos de seguridad colectiva *(collective_defense_conditioning)***
- **Descripción:** Medida en que el discurso del hegemón condiciona o pone en duda sus compromisos de seguridad colectiva vigentes. Mayor puntaje indica mayor grado de discurso autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a los compromisos de seguridad colectiva y asignandole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista tendrá a referirse a los acuerdos de seguridad colectiva como condicionales, negociables o contingentes a la conducta de sus aliados, sugiriendo que Estados Unidos podría cumplir con sus obligaciones de defensa.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**Tratados de defensa firmados *(signed_defense_treaties)***
- **Descripción:** Número de tratados bilaterales y multilaterales en materia de defensa firmados durante el año de observación. Conteo simple.
- **Proceso de recolección:** Usando una serie de scripts de Python y R, se analizó la serie de documentos Treaties in Force para hacer un recuento de los tratados bilaterales y multilaterales en materia de defensa firmados durante el año de observación. Debido a la presencia de ciertas discrepancias en los archivos originales de la fuente, se hizo uso del modelo GLM-OCR para automatizar el proceso de reconocimiento óptico de caracteres (OCR).
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista reduciría la cooperación militar con otros Estados, traduciendose a una baja en el número de tratados de defensa firmados. 
- **Período comprendido:** 1993-2013; 2016-2020; 2025
- **Fuente:** HeinOnline, Treaties in Force

**Tratados de defensa activos *(active_defense_treaties)***
- **Descripción: Número de tratados bilaterales y multilaterales en materia de defensa vigentes durante el año de observación. Conteo simple.**
- **Proceso de recolección: En desarrollo.**
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista reduciría la cooperación militar con otros Estados, traduciendose en una baja en el número de tratados de defensa activos a medida que estos dejan de ser renovados o son deliberadamente cancelados.
- **Período comprendido:** Usando una serie de scripts de Python y R, se analizó la serie de documentos Treaties in Force para hacer un recuento de los tratados bilaterales y multilaterales en materia de defensa mencionados como vigentes durante el año de observación. Debido a la presencia de ciertas discrepancias en los archivos originales de la fuente, se hizo uso del modelo GLM-OCR para automatizar el proceso de reconocimiento óptico de caracteres (OCR).
- **Período comprendido:** 1993-2013; 2016-2020; 2025
- **Fuente:** HeinOnline, Treaties in Force

**Tratados de defensa expirados, retirados o rescindidos *(removed_defense_treaties)***
- **Descripción:** Número de tratados bilaterales y multilaterales en materia de defensa que dejaron de estar vigentes durante el año de observación. Conteo simple.
- **Proceso de recolección:** Usando una serie de scripts de Python y R, se analizó la serie de documentos Treaties in Force para hacer un recuento de los tratados bilaterales y multilaterales en materia de defensa mencionados como vigentes durante el año de observación. Debido a la presencia de ciertas discrepancias en los archivos originales de la fuente, se hizo uso del modelo GLM-OCR para automatizar el proceso de reconocimiento óptico de caracteres (OCR).
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista reduciría la cooperación militar con otros Estados, traduciendose en una baja en el número de tratados de defensa activos a medida que estos dejan de ser renovados o son deliberadamente cancelados.
- **Período comprendido:** 1993-2013; 2016-2020; 2025
- **Fuente:** HeinOnline, Treaties in Force

**Presupuesto total de asistencia militar *(military_assistance_budget)***
- **Descripción:** Fondos gubernamentales estadounidenses destinados a asistencia militar según la subfunción 152 del presupuesto anual. Cifras en millones de dólares.
- **Proceso de recolección:** Entrada manual de datos a partir de la fuente.
- **Conducta esperada:** Se estima que una reducción presupuestaria en materia de asistencia militar podría considerarse como una manifestación sectorial del autorrevisionismo hegemónico.
- **Período comprendido:** 1993-2025
- **Fuente:** OMB — Historical Tables

**Participación en conflictos internacionales *(us_conflict_count)***
- **Descripción:** Número de conflictos internacionales activos en los que Estados Unidos actúa como parte durante el año de observación. Conteo simple.
- **Proceso de recolección:** Recuento con script de R.
- **Período comprendido:** Si bien la participación en conflictos no puede considerarse como un acto inherentemente opuesto al orden internacional liberal, se espera que un hegemón autorrevisionista sea más propenso a hacer uso de la fuerza que lo habitual.
- **Período Comprendido:** 1993-2025
- **Fuente:** UCDP

**Implicación en crisis internacionales *(crises_involvement)***
- **Descripción:** Grado de involucramiento estadounidense en crisis internacionales, ponderado a partir del grado de involucramiento estadounidense promedio dentro de todas las crisis internacionales registradas en el año de observación.
- **Proceso de recolección:** Cifra calculada con un script de R a partir de la fuente.
- **Conducta esperada:** Se espera que un hegemón autorrevisionista sería más propenso a involucrarse en crisis internacionales, tanto de manera directa como indirecta.
- **Período comprendido:** 1993-2022
- **Fuente:** International Crisis Behavior

**Invocación de la Resolución sobre los Poderes de Guerra *(wpr_count)***
- **Descripción:** Recuento anual de casos en los que el Presidente de Estados Unidos hizo uso de la Resolución sobre los Poderes de Guerra, entendiendose como una notificación formal al Congreso dentro de las 48 horas posteriores al uso de fuerzas militares en el extranjero. Conteo simple.
- **Proceso de recolección:** Filtración y recuento anual de casos correspondientes a usos de la Resolución sobre los Poderes de Guerra usando un script de R.
- **Conducta esperada:** Se considera que ante una mayor disposición a hacer uso de la fuerza, el uso de la Resolución sobre los Poderes de la Guerra tenderá a aumentar. Dicho esto, es importante considerar la posibilidad de que una presidencia que exhibe un carácter autorrevisionista decida ignorar las obligaciones de aquella resolución.
- **Período comprendido:** 1993-2025
- **Fuente:** War Powers Project

**Despliegue de fuerzas armadas en el extranjero *(deployments_abroad)***
- **Descripción:** Número de instancias en las que fuerzas militares de los Estados Unidos fueron desplegadas en el extranjero según listados del Servicio de Investigación del Congreso (CRS). Conteo simple.
- **Proceso de recolección:** Recuento anual de información compilada manualmente a partir de información del Servicio de Investigación del Congreso (CRS).
- **Conducta esperada:** Si bien el despliegue internacional de tropas no puede considerarse como un acto inherentemente opuesto al orden internacional liberal, se espera que un hegemón autorrevisionista sea más propenso a hacer uso de la fuerza que lo habitual.
- **Período comprendido:** 1993-2022
- **Fuente:** CRS R43738

**Coordinación internacional en el despliegue de fuerzas armadas en el extranjero *(deployments_abroad_coordination)***
- **Descripción:** Grado de coordinación internacional dentro de las instancias de despliegue de fuerzas militares estadounidenses en el extranjero según listados del Servicio de Investigación del Congreso (CRS). Junto a acciones coordinadas con otros Estados, se consideran operaciones militares autorizadas por el Consejo de Seguridad de Naciones Unidas, así como operaciones propias de la OTAN.
- **Proceso de recolección:** Recuento anual de información compilada manualmente a partir de información del Servicio de Investigación del Congreso (CRS).
- **Conducta esperada:** Se espera que un hegemón autorrevisionista actúe de manera mayormente unilateral a la hora de desplegar fuerzas armadas en el extranjero.
- **Período comprendido:** 1993-2022
- **Fuente:** CRS R43738

**Personal desplegado en actividades de mantenimiento de la paz *(peacekeeping_personnel)***
- **Descripción:** Recuento de personal estadounidense desplegado en operaciones de mantenimiento de la paz autorizadas por el Consejo de Seguridad de Naciones Unidas. Se consideran tanto oficiales como tropas. Conteo simple.
- **Proceso de recolección:** Recuento anual de información compilada manualmente. Cifra calculada a partir del último reporte mensual de fuerzas disponible para cada año de observación.
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista disminuiría sustancialmente la presencia estadounidense en operaciones internacionales de mantenimiento de la paz, evidenciandose en el número de misiones con participación estadounidense.
- **Período comprendido:** 1993-2025
- **Fuente:** UN Peacekeeping – Troop and police contributions data

**Participación en actividades de mantenimiento de la paz *(peacekeeping_active)***
- **Descripción:** Recuento de operaciones de mantenimiento de la paz autorizadas por el Consejo de Seguridad de Naciones Unidas con presencia de personal estadounidense. Conteo simple.
- **Proceso de recolección:** Recuento anual de información compilada manualmente. Cifra calculada a partir del último reporte mensual de fuerzas disponible para cada año de observación.
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista disminuiría sustancialmente la participación estadounidense en operaciones internacionales de mantenimiento de la paz, evidenciandose en el número de misiones con participación estadounidense.
- **Período comprendido:** 1993-2025
- **Fuente:** UN Peacekeeping – Troop and police contributions data

**Grado de participación en actividades de mantenimiento de la paz *(peacekeeping_rate)***
- **Descripción:** Porcentaje de operaciones de mantenimiento de la paz autorizadas por el Consejo de Seguridad de Naciones Unidas con presencia de personal estadounidense durante el año de observación.
- **Proceso de recolección:** Recuento anual de información compilada manualmente. Cifra calculada a partir del último reporte mensual de fuerzas disponible para cada año de observación.
- **Conducta esperada:** Se espera que bajo la influencia del autorrevisionismo hegemónico, el grado de participación estadounidense en actividades de mantenimiento de la paz disminuya sustancialmente en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:** UN Peacekeeping – Troop and police contributions data

**Contribuciones financieras al mantenimiento internacional de la paz *(peacekeeping_contributions)***
- **Descripción:** Fondos presupuestarios destinados a cubrir operaciones internacionales de mantenimiento de la paz, según cifras señaladas por el Departamento de Estado. Cifras en dólares.
- **Proceso de recolección:** Entrada manual de datos a partir de las fuentes.
- **Conducta esperada:** Se estima que un hegemón autorrevisionista sería propenso a disminuir la asignación de fondos destinados al mantenimiento internacional de la paz.
- **Período comprendido:** 1993-2025
- **Fuente:** Depto. de Estado — Intl. Affairs Budget · CRS RL30515

**Justificación y dispcición a hacer uso de la fuerza *(force_willingness)***
- **Descripción:** Medida en que el discurso del hegemón se dispone a y justifica el uso de la fuerza de manera unilateral. Mayor puntaje indica mayor grado de conducta autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados al uso de fuerza y asignandole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- Conducta esperada: Se teoriza que un hegemón autorrevisionista tendrá a justificar el uso de la fuerza de manera unilateral, citando el interés nacional por sobre materias como un mandato legal, el consentimiento de aliados o la autorización internacional.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**Tratados de no proliferación y control de armas firmados *(signed_npac_treaties)***
- **Descripción:** Número de tratados bilaterales y multilaterales en materia de no proliferación y control de armas firmados durante el año de observación. Conteo simple.
- **Proceso de recolección:** [...]
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista reduciría la cooperación militar con otros Estados, traduciendose a una baja en el número de tratados de defensa firmados.
- **Período comprendido:** 1993-2025
- **Fuente:** HeinOnline, Treaties in Force

**Tratados de no proliferación y control de armas activos *(active_npac_treaties)***
- **Descripción:** Número de tratados bilaterales y multilaterales en materia de no proliferación y control de armas vigentes durante el año de observación. Conteo simple.
- **Proceso de recolección:** [...]
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista reduciría la cooperación militar con otros Estados, traduciendose en una baja en el número de tratados de defensa activos a medida que estos dejan de ser renovados o son deliberadamente cancelados.
- **Período comprendido:** 1993-2013; 2016-2020; 2025
- **Fuente:** HeinOnline, Treaties in Force

**Tratados de no proliferación y control de armas expirados, retirados o rescindidos *(removed_npac_treaties)***
- **Descripción:** Número de tratados bilaterales y multilaterales en materia de no proliferación y control de armas que dejaron de estar vigentes durante el año de observación. Conteo simple.
- **Proceso de recolección:** [...]
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista reduciría la cooperación militar con otros Estados, traduciendose en un aumento en el número de tratados de no proliferación y control de armas no renovados o son deliberadamente cancelados.
- **Período comprendido:** 1993-2013; 2016-2020; 2025
- **Fuente:** HeinOnline, Treaties in Force

**Respeto por el derecho internacional *(int_law_respect)***
- **Descripción:** Medida en que el discurso del hegemón desestima, desprecia o subordina el derecho internacional. Mayor puntaje indica mayor grado de conducta autorrevisionista. Mayor puntaje indica mayor grado de discurso autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados al derecho internacional y asignandole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** se teoriza que un hegemón autorrevisionista tenderá a poner en duda el derecho internacional, afirmando que Estados Unidos no está obligado a cumplirlo y justificando las desviaciones respecto a este.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**Actitud hacia tribunales internacionales *(int_trib_attitude)***
- **Descripción:** Medida en que el discurso del hegemón desestima, desprecia o subordina la autoridad de tribunales y cortes internacionales, particularmente la Corte Penal Internacional y la Corte Internacional de Justicia, entre otros. Mayor puntaje indica mayor grado de discurso autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a tribunales internacionales y asignandole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- Conducta esperada: se teoriza que un hegemón autorrevisionista tenderá a poner en duda la autoridad de los tribunales internacionales, rechazando su jurisdicción y presentándolos como órganos ilegítimos o sesgados.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**ADHESIÓN DOMÉSTICA**
- **Índice de democracia liberal *(v2x_libdem)***
- **Descripción:** Medición sobre el grado en qué se alcanza el ideal de democracia liberal en Estados Unidos, considerando elementos como la protección de libertades individuales y de minorías frente al Estado en conjunto a otros elementos propios de la democracia electoral.
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Conducta esperada:** Se estima que un comportamiento autorrevisionista de parte de Estados Unidos estaría asociado a una disminución relativa del puntaje obtenido en el índice de democracia liberal.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Índice de democracia electoral *(v2x_polyarchy)***
- **Descripción:** Medición sobre el grado en qué se alcanza el ideal de democracia electoral en Estados Unidos, comprendiendo aspectos como elecciones limpias, sufragio amplio o cargos ejecutivos y legislativos electos.
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Conducta esperada:** Se estima que un comportamiento autorrevisionista de parte de Estados Unidos estaría asociado a una disminución relativa del puntaje obtenido en el índice de democracia electoral.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Índice de libertad en el mundo *(fiw_score)***
- **Descripción:** [...]
- **Proceso de recolección:** Filtrado de datos provenientes de Freedom House.
- **Conducta esperada:** [...]
- **Período comprendido:** [...]
- **Fuente:** Freedom House

**Índice de restricciones legislativas al ejecutivo *(v2xlg_legcon)***
- **Descripción:** Medición sobre las capacidades del poder legislativo y de otros organismos de control para interpelar, investigar y fiscalizar al ejecutivo en Estados Unidos, incluyendo el rol de la oposición parlamentaria.
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Conducta esperada:** Se estima que un comportamiento autorrevisionista de parte de Estados Unidos estaría asociado a una disminución relativa del puntaje obtenido en el índice de restricciones legislativas al ejecutivo.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Índice de restricciones judiciales al ejecutivo *(v2x_jucon)***
- **Descripción:** Medición sobre el grado en que el poder ejecutivo respeta la constitución y acata los fallos judiciales en Estados Unidos. Se considera, además, el grado de independencia del poder judicial.
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Conducta esperada:** Se estima que un comportamiento autorrevisionista de parte de Estados Unidos estaría asociado a una disminución relativa del puntaje obtenido en el índice de restricciones judiciales al ejecutivo.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Índice del estado de derecho *(v2x_rule)***
- **Descripción:** Medición sobre el grado en que las leyes se aplican de manera transparente, predecible, imparcial e igualitaria en Estados Unidos
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Conducta esperada:** Se estima que un comportamiento autorrevisionista de parte de Estados Unidos estaría asociado a una disminución relativa del puntaje obtenido en el índice del estado de derecho.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Índice de libertades civiles *(v2x_civlib)***
- **Descripción:** Medición sobre el respeto a las libertades civiles en Estados Unidos, entendidas como la ausencia de restricciones gubernamentales a las libertades privadas y políticas junto a la ausencia de violencia física ejercida por agentes del Estado.
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Conducta esperada:** Se estima que un comportamiento autorrevisionista de parte de Estados Unidos estaría asociado a una disminución relativa del puntaje obtenido en el índice de libertades civiles.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Subíndice de libertades civiles *(fh_civlib)***
- **Descripción:** Medición sobre el grado de respeto por las libertades civiles en Estados Unidos.
- **Proceso de recolección:** Filtrado de datos provenientes de Freedom House.
- **Conducta esperada:** Se espera que bajo la influencia del autorrevisionismo hegemónico, las mediciones sobre el respeto por las libertades civiles en Estados Unidos tiendan a la baja en comparación a otros períodos.
- **Período comprendido:** 2002-2025
- **Fuente:** Freedom House

**Subíndice de derechos políticos *(fh_polrights)***
- **Descripción:** Medición sobre el grado de respeto por los derechos políticos en Estados Unidos.
- **Proceso de recolección:** Filtrado de datos provenientes de Freedom House.
- **Conducta esperada:** Se espera que bajo la influencia del autorrevisionismo hegemónico, las mediciones sobre el respeto por los derechos políticos en Estados Unidos tiendan a la baja en comparación a otros períodos.
- **Período comprendido:** 2002-2025
- **Fuente:** Freedom House

**Autonomía de los partidos de oposición *(v2psoppaut)***
- **Descripción:** Medición sobre el grado en que los partidos de oposición en Estados Unidos pueden ser considerados como autónomos e independientes del partido gobernante, abarcando un espectro que va desde la prohibición total hasta la autonomía plena de todos los partidos.
- **Proceso de recolección:** Filtrado de datos provenientes de V-Dem.
- **Período comprendido:** 1993-2025
- **Fuente:** V-Dem

**Índice de protección de derechos humanos *(human_rights_score)***
- **Descripción:** Puntuación latente respecto a la protección de los derechos humanos en Estados Unidos. Cifras calculadas por Cristopher Fariss a partir de un modelo dinámico de teoría ordinal de la respuesta del elemento.
- **Conducta esperada:** Se estima que el autorrevisionismo hegemónico estaría asociado a una menor puntuación acorde al índice de protección de derechos humanos en comparación a otros períodos.
- **Proceso de recolección:** Filtrado de datos […]
- **Período comprendido:** 1993-2021
- **Fuente:** [...]

**Ratificación de tratados internacionales sobre derechos humanos *(hr_ratification_rate)***
- **Descripción:** Proporción de tratados en materia de derechos humanos ratificados por Estados Unidos. Se comprenden aquellos instrumentos legales señalados como fundamentales por la Oficina del Alto Comisionado de las Naciones Unidas para los Derechos Humanos.
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista tendría a no ratificar y posiblemente revocar la participación estadounidense en tratados internacionales en materia de derechos humanos en comparación a otros períodos.
- **Proceso de recolección:** Entrada manual a partir de datos señalados, ponderando [...]
- **Período comprendido:** 1993-2025
- **Fuente:** OHCHR – Human Rights Instruments. OHCHR – UN Treaty Body Database.

**Índice de derechos humanos *(human_rights_index)***
- **Descripción:** [...]
- **Conducta esperada:** [...]
- **Proceso de recolección:** [...]
- **Período comprendido:** 1993-2025
- **Fuente:** Our World in Data

**COMPROMISO IDEOLÓGICO**

**Ayuda externa destinada a materias relacionadas con la democracia *(democracy_aid)***
- **Descripción:** Fondos de ayuda externa catalogados como pertenecientes al sector de democracia, derechos humanos y governanza conforme al programa de estructuras estandarizadas y definiciones (SPSD) del Departamento de Estado.
- **Proceso de recolección:** Entrada manual de información disponible en el portal oficial de ayuda externa del gobierno estadounidense.
- **Conducta esperada:** Se teoriza que bajo gestión autorrevisionista, los fondos de ayuda externa dedicadas a materias relacionadas con la democracia se verán reducidos sustancialmente en comparación con otros períodos.
- **Período comprendido:** 2001-2024
- **Fuente: ForeignAssistance.gov**

**Asignaciones destinadas a la Fundación Nacional para la Democracia *(ned_allocations)***
- **Descripción:** Fondos asignados por el congreso estadounidense a la Fundación Nacional para la Democracia (NED). Cifras en dólares.
- **Proceso de recolección:** Entrada manual a partir de información disponible en las fuentes.
- **Conducta esperada:** Se estima que una reducción presupuestaria en materia de fondos destinados a la Fundación Nacional para la Democracia sean indicativos de una despriorización de la promoción de la democracia como objetivo de política exterior.
- **Período comprendido:** 1993-2025
- **Fuente:** [...]

**Promoción de la democracia como objetivo de política exterior *(democracy_objective)***
- **Descripción:** Medida en la que el discurso del hegemón promueve o rechaza la promoción internacional de la democracia como objetivo de su política exterior. Mayor puntaje indica mayor grado de conducta autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a la promoción internacional de la democracia y los objetivos internacionales de Estados Unidos, asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** Se teoriza que un hegemón autorrevisionista despriorizaría o rechazaría la promoción de la democracia como objetivo de política exterior, posicionando el tipo de sistema político de otros estados como irrelevante para los intereses de Estados Unidos.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**Transaccionalismo de alianzas *(alliance_transactionalism)***
- **Descripción: Medida en que el discurso del hegemón se refiere al tipo de relación entre Estados Unidos y sus aliados internacionales en términos transaccionales.** Mayor puntaje indica mayor grado de conducta autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a alianzas internacionales y asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada: Se espera que un hegemón autorrevisionista se refiera a los aliados de Estados Unidos en términos mayormente transaccionales, [burden sharing y beneficio neto más que valores compartidos o seguridad colectiva]**
- **Período comprendido:** 1993-2025
- **Fuente:** [...]

**Cordialidad discursiva hacia aliados internacionales *(ally_tone)***
- **Descripción:** Medida en que en que el discurso del hegemón se refiere a sus aliados y socios internacionales de manera cordial y respetuosa. Mayor puntaje indica mayor grado de discurso autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a alianzas internacionales y asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** Se espera que un hegemón autorrevisionista se refiera a sus aliados en términos despectivos, hostiles o condescendientes, tratándolos como subordinados, free-riders o incluso adversarios.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**Elogio o legitimación de líderes y regímenes autoritarios *(authoritarian_legitimation)***
- **Descripción:** Medida en la que el discurso del hegemón refleja una visión positiva de líderes. Gobiernos o regímenes autoritarios. Mayor puntaje indica mayor grado de conducta autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados a líderes autoritarios y asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** Se estima que bajo un hegemón autorrevisionista exista un mayor grado de afinidad discursiva hacia regímenes autoritarios que en otros períodos, tratándolos de igual o mejor manera que las democracias liberales.
- **Período comprendido:** 1993-2025
- **Fuente:** American Presidency Project

**Colaboración militar con Estados autoritarios *(auth_military_collaboration)***
- **Descripción:** Medida en la que los tratados de defensa bilaterales firmados por el hegemón se realizan en conjunto a Estados autoritarios. Medido a partir de una escala democrática contínua, una puntuación más baja es indicativa de un mayor grado de colaboración militar con Estados autoritarios efectuada a partir de la firma de tratados
- **Proceso de recolección:** [...]
- **Conducta esperada:** [...]
- **Período comprendido:** 1993-2025
- **Fuente:** HeinOnline, V-Dem

**Encuentros diplomáticos con democracias liberales mediante visitas de Estado. *(libdem_engagement)***
- **Descripción:** Proporción de visitas de Estado realizadas desde o hacia Estados considerados como democracias liberales. Se considera tanto la recepción de mandatarios internacionales en territorio estadounidense como las visitas de Estado efectuadas por el Presidente de los Estados Unidos y el Secretario de Estado.
- **Proceso de recolección:** Recolección manual de información disponible en la fuente, ponderada según [...].
- **Conducta esperada:** Se espera que bajo una administración autorrevisionista aumente el grado de visitas de Estado efectuadas a regímenes autoritarios en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:** [...]

**Encuentros diplomáticos con autocracias mediante visitas de Estado. *(autocratic_engagement)***
- **Descripción:** Proporción de visitas de Estado realizadas desde o hacia Estados considerados como regímenes autocraticos o autoritarios. Se considera tanto la recepción de mandatarios internacionales en territorio estadounidense como las visitas de Estado efectuadas por el Presidente de los Estados Unidos y el Secretario de Estado.
- **Proceso de recolección:** Recolección manual de información disponible en la fuente, ponderada según [...].
- **Conducta esperada:** Se espera que bajo una administración autorrevisionista aumente el grado de visitas de Estado efectuadas a regímenes autocráticos en comparación a otros períodos.
- **Período comprendido:** 1993-2025
- **Fuente:**

**Alineamiento de votos con democracias liberales en la Asamblea General *(un_libdem_alignment)***
- **Descripción:** Tasa de alineación promedio entre Estados Unidos con democracias liberales en las votaciones de la Asamblea General de las Naciones Unidas. Mayor puntaje indica mayor grado de alineamiento.
- **Proceso de recolección:** Cifra obtenida a partir del promedio de veces en las que las votaciones de un país considerado como democracia liberal por V-Dem se alinea al de Estados Unidos dentro de la Asamblea General de las Naciones Unidas. Uso de R.
- **Conducta esperada:** [...]
- **Período comprendido:** 1993-2025
- **Fuente:** [...]

**Alineamiento de votos con Estados autoritarios en la Asamblea General *(un_auth_alignment)***
- **Descripción:** Tasa de alineación promedio entre Estados Unidos con Estados autoritarios en las votaciones de la Asamblea General de las Naciones Unidas. Mayor puntaje indica mayor grado de alineamiento.
- **Proceso de recolección:** Cifra obtenida a partir del promedio de veces en las que las votaciones de un país considerado como autoritario por V-Dem se alinea al de Estados Unidos dentro de la Asamblea General de las Naciones Unidas. Uso de R.
- **Conducta esperada:** [...]
- **Período comprendido:** 1993-2025
- **Fuente:** [...]

**Actitudes hacia el internacionalismo liberal *(liberal_internationalism)***
- **Descripción:** Medida en que el discurso del hegemón refleja una visión alineada con los ideales del internacionalismo liberal en relación al rol que Estados Unidos debería cumplir en el mundo. Mayor puntaje indica mayor grado de discurso autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados al rol internacional de Estados Unidos y asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** Se espera que un hegemón autorrevisionista abogue por la reducción o retirada de Estados Unidos respecto a asuntos internacionales, priorizando cuestiones doméstitcas por sobre compromisos globales, rechazando su rol de liderazgo dentro del orden internacional.
- **Período comprendido:** 1993-2025
- **Fuente:** Corpus American Presidency Project

**Actitud hacia el multilateralismo *(mult_attitude)***
- **Descripción:** Forma en que el discurso del hegemón se refiere a organizaciones internacionales, instituciones multilaterales, la Organización de las Naciones Unidas o la acción colectiva a nivel internacional. Mayor puntaje indica mayor grado de discurso autorrevisionista.
- **Proceso de recolección:** Análisis discursivo computacional al corpus del American Presidency Project, filtrando por documentos relacionados al multilateralismo y/o diplomacia y asignándole un puntaje a los fragmentos relevantes a lo largo de un eje revisionista.
- **Conducta esperada:** Se espera que un hegemón autorrevisionista presente un discurso mayormente crítico en relación con instancias o foros multilaterales, posicionándolas como inefectivas, hostiles o limitantes.
- **Período comprendido:** 1993-2025
- **Fuente:** Corpus American Presidency Project
