# Consolidación del expediente técnico del proyecto en Word y generación automatizada de la presentación ejecutiva final del diseño para el comité.

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 60 minutos |
| Complejidad | Alta |
| Nivel de Bloom | Crear |
| Modalidad | Individual o equipos de proyecto |
| Producto final | Expediente técnico trazable en Word, presentación ejecutiva en PowerPoint y síntesis de acuerdos de Teams |

## Descripción general

En esta práctica final consolidarás los entregables generados en las prácticas anteriores en un expediente técnico único, estructurado y apto para revisión ejecutiva. Utilizarás Word y Copilot para sintetizar documentación, Excel para incorporar evidencia cuantitativa, Teams para registrar acuerdos y PowerPoint con Copilot para generar una narrativa orientada a decisión.

El resultado será un paquete de entrega final para el comité de NOVA Hydrate, con evidencia de mercado, propuesta de diseño, viabilidad comercial, riesgos, responsables y una recomendación explícita: aprobar, ajustar o detener la propuesta.

## Objetivos de aprendizaje

Al finalizar la práctica, podrás:

- [ ] Consolidar documentos, datos y activos visuales de un proyecto en un expediente técnico de Word con trazabilidad de fuentes.
- [ ] Sintetizar acuerdos, responsables, riesgos y próximos pasos desde una reunión o transcripción de Microsoft Teams.
- [ ] Incorporar datos y gráficos de Excel en Word y PowerPoint manteniendo coherencia con la fuente original.
- [ ] Generar y refinar una presentación ejecutiva de 10 a 12 diapositivas mediante Microsoft 365 Copilot.
- [ ] Validar que las conclusiones, cifras, responsables y recomendaciones sean verificables antes de compartir el paquete con el comité.

## Requisitos previos

### Conocimientos necesarios

- Uso intermedio de estilos, encabezados, tablas, imágenes y referencias cruzadas en Microsoft Word.
- Uso básico de gráficos, filtros y tablas en Microsoft Excel.
- Uso intermedio de diapositivas, diseños, notas del orador y modo de presentación en PowerPoint.
- Conocimiento de reuniones, transcripción y publicaciones en canales de Microsoft Teams.
- Capacidad para diferenciar hechos documentados, hipótesis y decisiones pendientes.
- Conocimiento de prompting parametrizado: contexto, fuente, audiencia, formato, restricciones y criterio de validación.

### Accesos y entregables necesarios

Antes de iniciar, verifica que tienes acceso de lectura y edición a la biblioteca corporativa del proyecto:

`/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/`

Deben estar disponibles los siguientes entregables de prácticas anteriores:

| Entregable esperado | Carpeta de referencia | Uso en esta práctica |
|---|---|---|
| `01_Guia_Prompts_NOVA_Hydrate.docx` | `/01_Prompts/` | Anexo de prompts y trazabilidad metodológica |
| `02_Moodboard_NOVA_Hydrate.pptx` | `/02_Moodboard/` | Evidencia visual y concepto de diseño |
| `02_Concepto_Seleccionado_NOVA_Hydrate.docx` | `/02_Moodboard/` | Identidad verbal, concepto y especificaciones preliminares |
| `03_Matriz_Competitiva_NOVA_Hydrate.xlsx` | `/03_Caso_Negocio/` | Datos, gráficos y análisis competitivo |
| `03_Caso_de_Negocio_NOVA_Hydrate.docx` | `/03_Caso_Negocio/` | Viabilidad comercial, supuestos y recomendación |

También debes disponer de acceso al equipo de Teams `LAB-Copilot-Diseno-Desarrollo`, al canal `Proyecto-NOVA-Hydrate` y a Microsoft 365 Copilot.

> **Nota sobre nombres de archivo:** la convención corporativa exige el formato `NN_TipoEntregable_NOVA_Hydrate_vMAJOR.MINOR.ext`. Durante esta práctica se utilizarán los nombres versionados `04_Expediente_Tecnico_NOVA_Hydrate_v1.0.docx` y `04_Presentacion_Comite_NOVA_Hydrate_v1.0.pptx`.

## Entorno de laboratorio

### Configuración de hardware recomendada

| Componente | Requisito |
|---|---|
| Procesador | Intel Core i5 de 11.ª generación, AMD Ryzen 5 5000 Series o superior |
| Memoria | 16 GB de RAM como mínimo; 32 GB recomendados |
| Almacenamiento | 20 GB libres en SSD |
| Pantalla | 1920 × 1080 como mínimo; segundo monitor recomendado |
| Red | 25 Mbps de descarga y 5 Mbps de carga como mínimo |
| Audio y vídeo | Micrófono y cámara funcionales para Teams |

### Software y servicios

| Componente | Referencia de entorno |
|---|---|
| Sistema operativo | Windows 11 Enterprise 24H2 |
| Microsoft 365 Apps for enterprise | Versión 2508, Canal actual |
| Word, Excel y PowerPoint | Versión 2508 o posterior compatible |
| Microsoft Teams | Cliente corporativo con acceso a reuniones y transcripción |
| Microsoft 365 Copilot | Servicio habilitado para el tenant corporativo |
| Microsoft Designer | Servicio web, si se utiliza para recursos visuales complementarios |
| Navegador | Microsoft Edge |

### Configuración obligatoria

Confirma la siguiente configuración antes de crear o editar archivos:

| Configuración | Valor requerido |
|---|---|
| Tenant de referencia | `contoso.onmicrosoft.com` |
| Idioma de aplicaciones | Español (España) |
| Zona horaria | `Europe/Madrid` |
| Formato de fecha | `dd/MM/yyyy` |
| Moneda | EUR |
| Separador decimal | Coma |
| Equipo de Teams | `LAB-Copilot-Diseno-Desarrollo` |
| Canal de trabajo | `Proyecto-NOVA-Hydrate` |

### Preparación de la estructura de carpetas

Comprueba que existe la siguiente estructura dentro de la ruta corporativa. Créala desde OneDrive o SharePoint si falta alguna carpeta.

```text
/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
├── 01_Prompts/
├── 02_Moodboard/
├── 03_Caso_Negocio/
├── 04_Expediente_Final/
├── Fuentes_Verificadas/
└── Exportaciones_PDF/
```

No guardes los entregables finales en Escritorio, Descargas ni unidades locales no administradas.

---

## Procedimiento paso a paso

### Paso 1. Verificar fuentes, permisos y trazabilidad inicial

**Objetivo:** confirmar que los entregables previos están disponibles, actualizados y accesibles antes de consolidar información.

**Instrucciones:**

1. Abre OneDrive para la Empresa o la biblioteca de SharePoint asociada al proyecto.
2. Navega a:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
   ```

3. Comprueba la existencia de los cinco entregables previos indicados en la sección de requisitos.
4. Abre cada archivo en modo de lectura y registra en una nota temporal:
   - Nombre del archivo.
   - Ubicación.
   - Fecha de modificación.
   - Propietario o autor visible.
   - Sección o contenido que se reutilizará.
5. Verifica que la matriz competitiva de Excel contiene datos identificables, encabezados claros y al menos un gráfico o una tabla que pueda utilizarse como evidencia.
6. Confirma que el caso de negocio contiene una recomendación, supuestos o estimaciones que puedan revisarse.
7. Si detectas información contradictoria entre documentos, no la resuelvas inventando una conclusión. Regístrala como una discrepancia que deberá aparecer en riesgos, pendientes o decisiones requeridas.
8. Crea, si no existe, una carpeta de trabajo dentro de `04_Expediente_Final/` para las versiones editables y otra para exportaciones.

**Resultado esperado:**

Dispones de un inventario mínimo de fuentes y de todos los archivos necesarios para consolidar el expediente.

**Verificación:**

- Los cinco entregables se abren desde la biblioteca corporativa.
- No hay archivos finales almacenados únicamente de forma local.
- Puedes identificar la procedencia de cada dato, gráfico, imagen o afirmación que se incluirá en el expediente.

---

### Paso 2. Crear la estructura base del expediente técnico en Word

**Objetivo:** crear un documento de Word con estructura ejecutiva, navegación clara y secciones trazables.

**Instrucciones:**

1. Abre Microsoft Word y crea un documento en blanco.
2. Guarda inmediatamente el archivo en:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/04_Expediente_Final/
   ```

3. Asigna el nombre:

   ```text
   04_Expediente_Tecnico_NOVA_Hydrate_v1.0.docx
   ```

4. Configura el idioma de revisión como **Español (España)**.
5. Inserta una portada con los siguientes elementos:
   - Título: `Expediente técnico del proyecto NOVA Hydrate`.
   - Subtítulo: `Consolidación de investigación, propuesta de diseño, viabilidad y decisiones para comité`.
   - Versión: `v1.0`.
   - Fecha con formato `dd/MM/yyyy`.
   - Equipo: `LAB-Copilot-Diseno-Desarrollo`.
   - Canal: `Proyecto-NOVA-Hydrate`.
   - Estado: `Borrador para validación ejecutiva`.
6. Después de la portada, inserta una tabla de control documental con estas columnas:

   | Campo | Valor |
   |---|---|
   | Documento | 04_Expediente_Tecnico_NOVA_Hydrate_v1.0.docx |
   | Versión | v1.0 |
   | Fecha | Fecha actual |
   | Elaborado por | Nombre del participante o equipo |
   | Revisado por | Comité NOVA Hydrate |
   | Ubicación corporativa | Ruta de OneDrive o SharePoint |
   | Clasificación | Uso interno / según política corporativa |

7. Inserta una tabla de contenido automática.
8. Crea las siguientes secciones utilizando estilos de encabezado de Word:

   1. Resumen ejecutivo  
   2. Reto de negocio  
   3. Investigación y evidencia de mercado  
   4. Identidad verbal y propuesta de valor  
   5. Concepto visual y dirección de diseño  
   6. Especificaciones preliminares  
   7. Matriz competitiva y análisis comparativo  
   8. Caso de negocio y viabilidad comercial  
   9. Riesgos, supuestos y dependencias  
   10. Decisiones, acuerdos y próximos pasos  
   11. Anexos y fuentes verificadas  

9. Inserta un salto de página antes de cada sección principal.
10. Añade en el pie de página:
    - Nombre corto del proyecto: `NOVA Hydrate`.
    - Número de página.
    - Versión del documento.

**Resultado esperado:**

Existe un expediente técnico con portada, control documental, tabla de contenido y once secciones estructuradas.

**Verificación:**

- Al aplicar el panel de navegación de Word, se visualizan las once secciones.
- La tabla de contenido se actualiza correctamente.
- El archivo se guarda en la carpeta corporativa `04_Expediente_Final`.
- La portada y el pie de página muestran una versión coherente.

---

### Paso 3. Consolidar el contenido mediante Word y Copilot

**Objetivo:** convertir los entregables previos en un documento coherente sin perder distinción entre evidencia, hipótesis y decisiones.

**Instrucciones:**

1. Abre en paralelo los documentos:
   - `01_Guia_Prompts_NOVA_Hydrate.docx`
   - `02_Concepto_Seleccionado_NOVA_Hydrate.docx`
   - `03_Caso_de_Negocio_NOVA_Hydrate.docx`
   - `02_Moodboard_NOVA_Hydrate.pptx`
   - `03_Matriz_Competitiva_NOVA_Hydrate.xlsx`

2. Completa primero las secciones del expediente con información verificada:
   - En **Reto de negocio**, resume el problema, oportunidad, público objetivo y objetivo de diseño.
   - En **Investigación y evidencia de mercado**, integra hallazgos documentados y separa datos observables de hipótesis.
   - En **Identidad verbal y propuesta de valor**, incorpora nombre, tono, atributos, promesa y mensajes clave definidos.
   - En **Concepto visual y dirección de diseño**, describe referencias, paleta, estilo, recursos visuales y criterio de selección.
   - En **Especificaciones preliminares**, documenta características del producto, restricciones, supuestos y criterios iniciales.
   - En **Caso de negocio y viabilidad comercial**, incorpora datos de mercado, estimaciones, costes, oportunidades y limitaciones existentes en la fuente.

3. Inserta una tabla de trazabilidad al final de cada sección principal con esta estructura:

   | Afirmación o activo | Tipo | Fuente | Ubicación | Estado de validación |
   |---|---|---|---|---|
   | Ejemplo: atributo de marca | Decisión de diseño | 02_Concepto_Seleccionado... | Sección de identidad | Verificado |
   | Ejemplo: posición competitiva | Dato analítico | 03_Matriz_Competitiva... | Hoja y rango | Verificado |
   | Ejemplo: previsión comercial | Supuesto | 03_Caso_de_Negocio... | Sección financiera | Pendiente de comité |

4. Utiliza Copilot en Word para producir un primer borrador del resumen ejecutivo. Adapta el siguiente prompt a los datos reales del expediente:

   > A partir del contenido de este documento, redacta un resumen ejecutivo de un máximo de 350 palabras para un comité de decisión. Incluye: reto de negocio, evidencia más relevante, propuesta de NOVA Hydrate, viabilidad comercial, principales riesgos y recomendación actual. Distingue explícitamente entre hechos verificados, supuestos y decisiones pendientes. Usa tono profesional, conciso y orientado a decisión. No inventes cifras, fuentes, responsables ni conclusiones que no aparezcan en el documento.

5. Revisa el resultado de Copilot frase por frase. Corrige o elimina:
   - Cifras sin fuente.
   - Generalizaciones no respaldadas.
   - Riesgos no documentados.
   - Recomendaciones que no hayan sido aprobadas o justificadas.
   - Referencias a personas, clientes o datos que no deban incluirse.
6. Inserta en la sección **Riesgos, supuestos y dependencias** una tabla como la siguiente:

   | ID | Riesgo, supuesto o dependencia | Impacto | Probabilidad | Mitigación o validación requerida | Responsable | Estado |
   |---|---|---|---|---|---|---|
   | R-01 | Completar con información real | Alto/Medio/Bajo | Alta/Media/Baja | Acción verificable | Persona o rol | Abierto/Cerrado |

7. Inserta una tabla de decisiones inicial en la sección **Decisiones, acuerdos y próximos pasos**. Déjala preparada para completarla con la síntesis de Teams:

   | ID | Decisión o acción | Responsable | Fecha objetivo | Evidencia o fuente | Estado |
   |---|---|---|---|---|---|

8. Actualiza la tabla de contenido de Word.

**Resultado esperado:**

El expediente contiene un borrador completo, con contenido procedente de fuentes identificadas, trazabilidad visible y una separación clara entre hechos, supuestos y pendientes.

**Verificación:**

- Cada sección sustantiva contiene al menos una referencia a su fuente.
- El resumen ejecutivo no incluye información no verificable.
- La sección de riesgos identifica elementos pendientes de validación.
- Las tablas de trazabilidad permiten localizar la fuente de las afirmaciones relevantes.

---

### Paso 4. Incorporar evidencia de Excel y activos visuales del moodboard

**Objetivo:** integrar gráficos, tablas y recursos visuales de manera legible, trazable y consistente con los datos originales.

**Instrucciones:**

1. Abre `03_Matriz_Competitiva_NOVA_Hydrate.xlsx`.
2. Revisa los encabezados, criterios de evaluación, fórmulas y gráficos antes de copiar contenido.
3. Identifica:
   - Un gráfico comparativo útil para el comité.
   - Una tabla o resumen con criterios de diferenciación.
   - Cualquier dato que deba tratarse como supuesto o estimación.
4. Si el gráfico necesita ajustes, realiza los cambios en Excel, no en la copia de Word:
   - Añade un título claro.
   - Comprueba etiquetas, leyenda y escala.
   - Verifica que el formato regional utiliza coma como separador decimal y EUR cuando corresponda.
5. Copia el gráfico desde Excel.
6. En Word, colócalo en la sección **Matriz competitiva y análisis comparativo** mediante una de estas opciones:
   - **Pegar vínculo**, si el comité debe recibir datos actualizables y el acceso a la fuente está garantizado.
   - **Pegar como imagen**, si el expediente debe congelar la versión para revisión.
7. Debajo del gráfico, añade un pie con:
   - Título del gráfico.
   - Fuente: nombre del archivo de Excel, hoja y fecha de revisión.
   - Nota de interpretación: qué muestra el gráfico y qué no permite concluir.
8. Abre `02_Moodboard_NOVA_Hydrate.pptx`.
9. Selecciona una o dos imágenes representativas del concepto aprobado. Inserta únicamente activos que estén autorizados para uso interno y cuya procedencia esté documentada.
10. Inserta los activos en la sección **Concepto visual y dirección de diseño**.
11. Añade una leyenda bajo cada recurso visual:

   ```text
   Figura X. Referencia visual del concepto NOVA Hydrate.
   Fuente: 02_Moodboard_NOVA_Hydrate.pptx, diapositiva X.
   Uso: evidencia de dirección visual; no representa una especificación final de producción.
   ```

12. En Word, utiliza títulos de figura y referencias cruzadas si el documento contiene varias imágenes o gráficos.
13. Guarda el expediente.

**Resultado esperado:**

El expediente incorpora al menos un gráfico de Excel y uno o dos elementos visuales del moodboard, con títulos, fuentes y contexto interpretativo.

**Verificación:**

- El gráfico coincide con la fuente de Excel.
- Los datos visibles no han sido modificados manualmente en Word.
- Cada imagen y gráfico tiene título, fuente y una explicación breve.
- El documento mantiene una composición legible y no presenta imágenes cortadas.

---

### Paso 5. Obtener acuerdos y acciones desde Teams con Copilot

**Objetivo:** sintetizar una reunión de comité simulada o una transcripción de práctica para completar la sección de decisiones y seguimiento.

**Instrucciones:**

1. Abre Microsoft Teams e ingresa al equipo:

   ```text
   LAB-Copilot-Diseno-Desarrollo
   ```

2. Abre el canal:

   ```text
   Proyecto-NOVA-Hydrate
   ```

3. Realiza una de las siguientes alternativas:

   **Alternativa A: reunión simulada**
   1. Programa o inicia una reunión titulada:

      ```text
      Comité NOVA Hydrate - Validación Ejecutiva
      ```

   2. Añade al menos los roles disponibles en el equipo: facilitación, diseño, negocio y revisión.
   3. Activa la transcripción solo si está permitida por la política corporativa y todos los participantes han sido informados.
   4. Presenta brevemente el reto, evidencia, concepto, viabilidad, riesgos y recomendación preliminar.
   5. Registra decisiones explícitas durante la reunión.

   **Alternativa B: transcripción de práctica disponible**
   1. Abre una reunión anterior del canal con transcripción habilitada.
   2. Verifica que tienes permisos para consultar el resumen y la transcripción.
   3. No exportes ni compartas la transcripción fuera del entorno autorizado.

4. Utiliza Copilot en Teams, en el resumen de reunión o en el contexto habilitado por la organización, con un prompt como el siguiente:

   > Resume únicamente la información presente en la reunión o transcripción sobre NOVA Hydrate. Organiza la respuesta en cinco apartados: 1) decisiones aprobadas, 2) decisiones pendientes, 3) acciones con responsable, 4) riesgos o bloqueos y 5) próximos pasos con fecha si se menciona. No inventes responsables, fechas, cifras ni acuerdos. Si un responsable o fecha no aparece, indica “No especificado”.

5. Revisa el resumen comparándolo con la transcripción o notas de reunión.
6. Clasifica cada elemento obtenido:
   - **Decisión aprobada:** se expresó de forma explícita y cuenta con autoridad o consenso identificado.
   - **Acción:** tiene responsable o necesita asignación.
   - **Pendiente:** necesita validación o información adicional.
   - **Riesgo:** puede afectar plazo, alcance, coste, cumplimiento o viabilidad.
7. Copia únicamente los acuerdos verificados a la sección **Decisiones, acuerdos y próximos pasos** del expediente.
8. Añade una columna `Fuente` a la tabla de decisiones y registra, por ejemplo:

   ```text
   Teams, Comité NOVA Hydrate - Validación Ejecutiva, dd/MM/yyyy
   ```

9. Si no existe una transcripción habilitada, registra en la tabla que la fuente es un acta manual revisada y no atribuyas a Copilot contenidos que no pudo analizar.
10. Publica en el canal de Teams un mensaje breve con el enlace al expediente en revisión y solicita validación de los responsables cuando corresponda.

**Resultado esperado:**

La sección de decisiones del expediente contiene acuerdos, acciones, responsables, fechas y pendientes basados en una fuente de Teams o en un acta de práctica validada.

**Verificación:**

- Cada acuerdo tiene fuente identificable.
- Los elementos sin responsable o fecha se marcan como `No especificado` o `Pendiente de asignación`.
- No se presentan inferencias de Copilot como decisiones oficiales.
- El expediente incluye al menos un próximo paso verificable.

---

### Paso 6. Generar la presentación ejecutiva en PowerPoint con Copilot

**Objetivo:** crear una presentación ejecutiva de 10 a 12 diapositivas basada en el expediente técnico y orientada a una decisión de comité.

**Instrucciones:**

1. Confirma que el expediente técnico está guardado y actualizado.
2. Abre Microsoft PowerPoint.
3. Crea una presentación nueva y guárdala en:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/04_Expediente_Final/
   ```

4. Utiliza el nombre:

   ```text
   04_Presentacion_Comite_NOVA_Hydrate_v1.0.pptx
   ```

5. Comprueba que el idioma de edición es **Español (España)**.
6. Utiliza Copilot en PowerPoint para crear una presentación a partir del expediente técnico, si la capacidad está disponible en tu tenant. Usa un prompt parametrizado como este:

   > Crea una presentación ejecutiva de 10 a 12 diapositivas a partir del documento 04_Expediente_Tecnico_NOVA_Hydrate_v1.0.docx. Audiencia: comité ejecutivo. Propósito: decidir si se aprueba, ajusta o detiene la propuesta NOVA Hydrate. Estructura requerida: portada, reto, evidencia de mercado, oportunidad competitiva, propuesta de valor e identidad verbal, concepto visual, especificaciones preliminares, viabilidad comercial, riesgos y dependencias, acuerdos y próximos pasos, recomendación explícita. Usa mensajes breves, una idea principal por diapositiva, tono profesional y evidencia trazable. No inventes datos, imágenes, responsables, fuentes ni conclusiones. Indica “Pendiente de validación” cuando la fuente no sea concluyente.

7. Si la opción de crear desde documento no está disponible, crea las diapositivas manualmente y utiliza Copilot para generar borradores de contenido por sección.
8. Ajusta la presentación para que contenga entre 10 y 12 diapositivas. Utiliza la siguiente estructura recomendada:

   | Diapositiva | Título orientativo | Contenido esperado |
   |---|---|---|
   | 1 | NOVA Hydrate: decisión requerida | Proyecto, fecha, versión y recomendación preliminar |
   | 2 | Reto y oportunidad | Problema de negocio, público y oportunidad |
   | 3 | Evidencia de mercado | Dos o tres hallazgos verificables |
   | 4 | Posicionamiento competitivo | Gráfico o matriz procedente de Excel |
   | 5 | Propuesta de valor | Beneficio, diferenciación y mensaje principal |
   | 6 | Identidad verbal y concepto visual | Atributos de marca y evidencia del moodboard |
   | 7 | Especificaciones preliminares | Alcance, características y restricciones |
   | 8 | Viabilidad comercial | Supuestos, oportunidad, costes o métricas disponibles |
   | 9 | Riesgos y dependencias | Riesgos principales y mitigaciones |
   | 10 | Decisiones y próximos pasos | Acuerdos, responsables y fechas |
   | 11 | Recomendación para comité | Aprobar, ajustar o detener, con justificación |
   | 12 | Anexo opcional | Fuentes, supuestos críticos o detalle metodológico |

9. Inserta el gráfico competitivo desde Excel en la diapositiva 4. Utiliza la misma versión validada que aparece en el expediente.
10. Inserta una imagen o composición visual del moodboard en la diapositiva 6, con uso moderado de texto.
11. Para cada diapositiva con cifra, gráfico o afirmación relevante, añade una fuente breve en el pie:

   ```text
   Fuente: 03_Matriz_Competitiva_NOVA_Hydrate.xlsx, hoja [nombre], revisado el dd/MM/yyyy.
   ```

12. Revisa los textos generados por Copilot:
   - Sustituye párrafos extensos por mensajes ejecutivos.
   - Elimina repeticiones.
   - Comprueba que la recomendación es consistente con riesgos y evidencia.
   - Evita promesas no demostradas.
   - Mantén la diferencia entre hecho, supuesto y decisión pendiente.
13. Añade notas del orador en las diapositivas 3, 8, 9 y 11 para explicar el contexto de los datos y la decisión requerida.
14. Guarda la presentación.

**Resultado esperado:**

Existe una presentación de 10 a 12 diapositivas, con narrativa ejecutiva, evidencia visual y cuantitativa, riesgos identificados y una recomendación explícita.

**Verificación:**

- La presentación tiene entre 10 y 12 diapositivas.
- Incluye una recomendación clara: aprobar, ajustar o detener.
- El gráfico competitivo coincide con el de Excel.
- No hay diapositivas con texto excesivo, contenido sin fuente o imágenes no autorizadas.
- Las diapositivas de riesgos y próximos pasos son coherentes con el expediente y con Teams.

---

### Paso 7. Refinar la recomendación y realizar revisión ejecutiva

**Objetivo:** comprobar que la documentación y la presentación permiten tomar una decisión fundamentada.

**Instrucciones:**

1. Abre simultáneamente:
   - El expediente técnico en Word.
   - La presentación en PowerPoint.
   - La matriz competitiva en Excel.
   - El resumen o transcripción de Teams, si existe.
2. Revisa la coherencia entre los cuatro entornos:
   - Las cifras de PowerPoint deben coincidir con Excel.
   - Los acuerdos de Word deben coincidir con Teams.
   - La propuesta visual debe coincidir con el moodboard y el concepto seleccionado.
   - La recomendación debe reflejar riesgos, evidencias y viabilidad documentados.
3. Aplica el siguiente criterio para definir la recomendación final:
   - **Aprobar:** existe evidencia suficiente, los riesgos son aceptables o mitigables y hay próximos pasos viables.
   - **Ajustar:** la oportunidad es válida, pero faltan validaciones, responsables, presupuesto, evidencia o definición de alcance.
   - **Detener:** la evidencia contradice la propuesta, los riesgos no son aceptables o la viabilidad no se sostiene.
4. Completa la diapositiva de recomendación con una fórmula clara:

   ```text
   Recomendación: [Aprobar / Ajustar / Detener] la propuesta NOVA Hydrate.
   Justificación: [dos o tres razones verificables].
   Decisión solicitada al comité: [acción concreta].
   ```

5. Utiliza Copilot para revisar claridad, no para sustituir la validación de contenido. Prompt recomendado:

   > Revisa esta presentación como si fueras un comité ejecutivo. Identifica mensajes ambiguos, datos sin fuente, contradicciones entre riesgos y recomendación, y diapositivas que no contribuyen a la decisión. No modifiques cifras ni inventes información. Devuelve una lista priorizada de mejoras.

6. Implementa únicamente las mejoras que puedas verificar con las fuentes.
7. Actualiza la versión de ambos documentos si realizas cambios sustantivos:
   - `v1.0` para primera versión consolidada.
   - `v1.1` para correcciones menores verificadas.
   - `v2.0` si cambia el alcance, la recomendación o una decisión relevante.
8. Actualiza la tabla de control documental y la tabla de contenido del expediente.

**Resultado esperado:**

El expediente y la presentación presentan una recomendación defendible, consistente y respaldada por fuentes identificables.

**Verificación:**

- La recomendación aparece de forma explícita en Word y PowerPoint.
- Todas las cifras críticas pueden localizarse en una fuente.
- Los riesgos no quedan ocultos por mensajes excesivamente optimistas.
- Las decisiones pendientes se muestran como pendientes, no como aprobadas.

---

### Paso 8. Exportar el paquete final y compartirlo para revisión

**Objetivo:** generar versiones no editables, conservar los archivos fuente y compartir el paquete final desde la ubicación corporativa.

**Instrucciones:**

1. Guarda las versiones editables finales en `04_Expediente_Final/`.
2. En Word, exporta el expediente a PDF con el nombre:

   ```text
   04_Expediente_Tecnico_NOVA_Hydrate_v1.0.pdf
   ```

3. En PowerPoint, exporta la presentación a PDF con el nombre:

   ```text
   04_Presentacion_Comite_NOVA_Hydrate_v1.0.pdf
   ```

4. Guarda ambos PDF en:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/Exportaciones_PDF/
   ```

5. Abre los PDF y valida:
   - Portada correcta.
   - Fuentes legibles.
   - Gráficos completos.
   - Paginación correcta.
   - Sin comentarios, notas internas o contenido oculto no destinado al comité.
6. En Teams, publica en el canal `Proyecto-NOVA-Hydrate` un mensaje con enlaces a:
   - Expediente técnico editable.
   - PDF del expediente.
   - Presentación editable.
   - PDF de la presentación.
7. Solicita revisión con una instrucción clara, por ejemplo:

   > Se ha publicado el paquete final de NOVA Hydrate para revisión ejecutiva. Validar antes de la reunión: cifras de matriz competitiva, riesgos críticos, responsables de próximos pasos y recomendación propuesta. Registrar observaciones en el canal antes de la reunión Comité NOVA Hydrate - Validación Ejecutiva.

**Resultado esperado:**

El paquete final está disponible en la biblioteca corporativa, en formato editable y PDF, y se ha comunicado al equipo para revisión.

**Verificación:**

- Existen cuatro archivos finales: dos editables y dos PDF.
- Los enlaces compartidos apuntan a la biblioteca corporativa, no a ubicaciones locales.
- Los PDF se abren correctamente.
- El canal de Teams contiene el aviso de revisión.

---

## Validación y pruebas

Completa la siguiente lista antes de considerar finalizada la práctica.

### Validación del expediente técnico

| Criterio | Resultado esperado | Estado |
|---|---|---|
| Nombre y ubicación | Archivo versionado en `04_Expediente_Final/` | ☐ |
| Estructura | Portada, control documental, tabla de contenido y once secciones | ☐ |
| Resumen ejecutivo | Máximo aproximado de 350 palabras y orientado a decisión | ☐ |
| Trazabilidad | Fuentes identificadas para afirmaciones, gráficos e imágenes | ☐ |
| Evidencia | Diferenciación clara entre hechos, supuestos y pendientes | ☐ |
| Datos de Excel | Gráfico o tabla coherente con el archivo fuente | ☐ |
| Activos visuales | Imágenes del moodboard con fuente y uso documentado | ☐ |
| Riesgos | Riesgos, supuestos, dependencias y mitigaciones identificados | ☐ |
| Acuerdos | Acciones, responsables y fuentes de Teams o acta revisada | ☐ |

### Validación de la presentación ejecutiva

| Criterio | Resultado esperado | Estado |
|---|---|---|
| Número de diapositivas | Entre 10 y 12 diapositivas | ☐ |
| Audiencia | Lenguaje adecuado para comité ejecutivo | ☐ |
| Narrativa | Reto, evidencia, propuesta, viabilidad, riesgos y decisión | ☐ |
| Evidencia competitiva | Gráfico o matriz procedente de Excel | ☐ |
| Concepto visual | Referencia visual coherente con el moodboard | ☐ |
| Fuentes | Cifras y gráficos con fuente breve visible | ☐ |
| Recomendación | Aprobar, ajustar o detener de forma explícita | ☐ |
| Próximos pasos | Responsables, fechas o indicación de pendiente | ☐ |
| Notas del orador | Contexto añadido en diapositivas críticas | ☐ |

### Prueba de coherencia final

Realiza estas cuatro comprobaciones cruzadas:

1. Selecciona tres cifras de PowerPoint y localízalas en Excel o en el caso de negocio.
2. Selecciona dos acuerdos de Word y compáralos con la transcripción, resumen de Teams o acta revisada.
3. Selecciona una afirmación sobre identidad o diseño y localízala en el concepto seleccionado o moodboard.
4. Lee la recomendación final y comprueba que no contradice los riesgos, supuestos o dependencias documentados.

La práctica se considera superada cuando las cuatro comprobaciones pueden completarse sin depender de contenido inventado, referencias ambiguas o archivos fuera de la ubicación corporativa.

## Resolución de problemas

### Problema 1: Copilot no puede crear la presentación desde el expediente técnico

**Síntomas:** la opción para crear una presentación desde un documento no aparece, Copilot no encuentra el archivo de Word o devuelve una respuesta sin acceso al contenido.

**Causa:** el archivo no está guardado en OneDrive para la Empresa o SharePoint, el usuario no tiene permisos suficientes, el servicio de Copilot no está habilitado para esa función en el tenant o el documento aún no se ha sincronizado.

**Solución:**

1. Guarda y cierra el expediente en la biblioteca corporativa.
2. Comprueba que el icono de sincronización de OneDrive indica que no hay cambios pendientes.
3. Verifica que puedes abrir el documento desde el navegador con la misma cuenta corporativa.
4. Revisa permisos de edición sobre el archivo y la carpeta.
5. Reinicia PowerPoint y vuelve a iniciar sesión con la cuenta del tenant autorizado.
6. Si la capacidad sigue sin estar disponible, crea la estructura de diapositivas manualmente y usa Copilot para redactar cada sección a partir de texto copiado y verificado del expediente.

### Problema 2: Los gráficos de Excel se ven desactualizados, cortados o con formato diferente en Word o PowerPoint

**Síntomas:** el gráfico pegado no coincide con Excel, muestra valores antiguos, pierde etiquetas, cambia el separador decimal o aparece recortado en el PDF.

**Causa:** se pegó una copia estática anterior, se utilizó un vínculo a una ruta no accesible, el gráfico no se redimensionó proporcionalmente o existen diferencias de configuración regional entre aplicaciones.

**Solución:**

1. Corrige primero el gráfico en Excel y guarda el archivo fuente.
2. Confirma que Excel utiliza idioma Español (España), moneda EUR y coma como separador decimal.
3. Elimina la copia anterior en Word o PowerPoint.
4. Inserta de nuevo el gráfico mediante **Pegar vínculo** si debe mantenerse actualizado, o como imagen si debe congelarse para comité.
5. Añade un título y fuente debajo del gráfico.
6. Exporta a PDF y revisa el resultado visual antes de compartirlo.

## Limpieza

1. Confirma que todos los archivos finales están en la biblioteca corporativa.
2. Elimina copias temporales o borradores duplicados almacenados fuera de OneDrive o SharePoint, siempre que no estén sujetos a una política de retención.
3. Conserva únicamente las versiones necesarias según la convención de control documental:
   - Versiones mayores para cambios de alcance o decisión.
   - Versiones menores para correcciones verificadas.
4. Cierra Word, Excel, PowerPoint y Teams después de verificar la sincronización.
5. No elimines documentos fuente de las prácticas anteriores, ya que forman parte de la trazabilidad del expediente.
6. Comprueba que los PDF finales están en `Exportaciones_PDF/` y que los editables permanecen en `04_Expediente_Final/`.

## Resumen

En esta práctica consolidaste el proyecto NOVA Hydrate en un expediente técnico trazable y una presentación ejecutiva orientada a decisión. Integraste Word, Excel, Teams y PowerPoint como un flujo de trabajo conectado: Teams aportó acuerdos y acciones; Word formalizó la documentación; Excel proporcionó evidencia analítica; y PowerPoint comunicó la recomendación al comité.

La calidad del resultado depende de tres controles esenciales: fuentes identificables, prompts precisos y revisión humana. Copilot puede acelerar la síntesis, redacción y estructuración, pero no sustituye la validación profesional de datos, decisiones, riesgos, permisos ni contenido confidencial.

### Recursos recomendados

- [Microsoft Copilot para Microsoft 365: información general y capacidades](https://support.microsoft.com/es-es/copilot-microsoft-365)
- [Bienvenido a Copilot en Microsoft Teams](https://support.microsoft.com/es-es/office/bienvenido-a-copilot-en-microsoft-teams-bc9c0d82-6d3e-4dce-8ca4-1fe149da503c)
- [Ayuda y aprendizaje de Microsoft Word](https://support.microsoft.com/es-es/word)
- [Ayuda y aprendizaje de Microsoft Excel](https://support.microsoft.com/es-es/excel)
- [Ayuda y aprendizaje de Microsoft PowerPoint](https://support.microsoft.com/es-es/powerpoint)
