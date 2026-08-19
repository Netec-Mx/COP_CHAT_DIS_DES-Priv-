# Creación de una guía de prompts corporativos parametrizados para la investigación y conceptualización de una nueva marca de producto.

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 60 minutos |
| Complejidad | Media |
| Nivel de Bloom | Crear |

## Descripción general

En esta práctica crearás una guía corporativa de *prompts* parametrizados para el proyecto transversal **NOVA Hydrate**, una línea de botellas térmicas reutilizables orientada a profesionales urbanos de 25 a 40 años. El documento será creado en Microsoft Word y almacenado en OneDrive for Business como fuente de referencia para las siguientes prácticas del curso.

Aplicarás los marcos **Rol-Contexto-Tarea-Formato-Criterios (RCTFC)** y **Objetivo-Contexto-Datos-Instrucciones-Validación (OCDIV)** para diseñar solicitudes reutilizables en investigación de mercado, segmentación, identidad de marca, análisis de riesgos y comunicación ejecutiva. También establecerás controles para diferenciar hipótesis generadas por IA de información que necesita ser validada mediante fuentes confiables.

## Objetivos de aprendizaje

Al finalizar la práctica, podrás:

- [ ] Definir los parámetros estratégicos iniciales de la marca piloto NOVA Hydrate.
- [ ] Aplicar los marcos RCTFC y OCDIV para redactar *prompts* corporativos consistentes.
- [ ] Crear una biblioteca de *prompts* reutilizables para investigación, conceptualización y presentación ejecutiva.
- [ ] Incorporar restricciones, formatos de salida y criterios de calidad en cada solicitud a Copilot.
- [ ] Documentar criterios de verificación para separar hechos, hipótesis, recomendaciones y afirmaciones pendientes de validación.

## Requisitos previos

### Conocimientos necesarios

- Manejo intermedio de Microsoft Word: estilos, tablas, comentarios, encabezados y guardado en OneDrive.
- Comprensión básica de segmentación de mercado, propuesta de valor, sostenibilidad e identidad de marca.
- Conocimiento de que Copilot puede generar hipótesis, borradores y alternativas, pero no sustituye la verificación humana de datos relevantes.
- Capacidad para revisar resultados generados por IA mediante criterios de negocio, audiencia, viabilidad y evidencia.

### Accesos necesarios

- Cuenta corporativa con licencia activa de Microsoft 365 Copilot.
- Acceso a Microsoft Word, Microsoft 365 Copilot Chat y OneDrive for Business.
- Permisos de edición en la biblioteca o ubicación corporativa del proyecto.
- Acceso al tenant corporativo `contoso.onmicrosoft.com`, o una cuenta invitada con permisos explícitos.
- Conexión a Internet estable.

## Entorno de laboratorio

### Configuración de hardware recomendada

| Recurso | Requisito |
|---|---|
| Procesador | Intel Core i5 de 11.ª generación, AMD Ryzen 5 5000 Series o superior |
| Memoria | 16 GB de RAM como mínimo; 32 GB recomendados |
| Almacenamiento | 20 GB libres en SSD |
| Pantalla | 1920 × 1080 píxeles como mínimo; segundo monitor recomendado |
| Red | 25 Mbps de descarga y 5 Mbps de carga como mínimo |
| Periféricos | Micrófono y cámara funcionales para actividades posteriores en Teams |

### Software de referencia

| Componente | Versión o servicio de referencia |
|---|---|
| Sistema operativo | Windows 11 Enterprise 24H2, compilación 26100.6584 |
| Microsoft 365 Apps for enterprise | Versión 2508, compilación 19127.20358 |
| Microsoft Word | Versión 2508, compilación 19127.20358 |
| Microsoft 365 Copilot | Línea de lanzamiento 2026.08 |
| Microsoft Edge | Versión 139.0.3405.86 |
| OneDrive for Business | Asociado al tenant corporativo |

### Configuración corporativa obligatoria

Antes de comenzar, confirma los siguientes valores en las aplicaciones de Microsoft 365:

| Configuración | Valor obligatorio |
|---|---|
| Idioma | Español (España) |
| Zona horaria | Europe/Madrid |
| Formato de fecha | `dd/MM/yyyy` |
| Moneda | EUR (€) |
| Separador decimal | Coma |
| Tenant de referencia | `contoso.onmicrosoft.com` |
| Equipo de Teams | `LAB-Copilot-Diseno-Desarrollo` |
| Canal de trabajo | `Proyecto-NOVA-Hydrate` |
| Reunión de revisión final | `Comité NOVA Hydrate - Validación Ejecutiva` |

### Ruta y estructura de almacenamiento

Todos los archivos deben guardarse en OneDrive for Business. No uses Escritorio, Descargas ni ubicaciones locales no administradas para entregables finales.

Ruta raíz obligatoria:

```text
/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
```

Estructura requerida:

```text
/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
├── 01_Prompts/
├── 02_Moodboard/
├── 03_Caso_Negocio/
├── 04_Expediente_Final/
├── Fuentes_Verificadas/
└── Exportaciones_PDF/
```

Convención obligatoria de nombres:

```text
NN_TipoEntregable_NOVA_Hydrate_vMAJOR.MINOR.ext
```

Archivo que crearás:

```text
01_Guia_Prompts_NOVA_Hydrate_v1.0.docx
```

> **Nota:** La versión `v1.0` identifica el primer borrador controlado. Si posteriormente realizas cambios significativos aprobados, incrementa la versión mayor o menor según las instrucciones del curso, por ejemplo, `v1.1` o `v2.0`.

---

## Procedimiento paso a paso

### Paso 1. Preparar la ubicación corporativa y crear el documento base

**Objetivo:** Crear la estructura de trabajo en OneDrive for Business y generar el documento Word controlado que contendrá la guía de *prompts*.

**Instrucciones:**

1. Inicia sesión en Microsoft 365 con tu cuenta corporativa del tenant autorizado.
2. Abre **OneDrive** desde el iniciador de aplicaciones de Microsoft 365 o desde el icono de OneDrive en Windows.
3. Navega a la ruta:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
   ```

4. Comprueba que existen las carpetas requeridas:
   - `01_Prompts`
   - `02_Moodboard`
   - `03_Caso_Negocio`
   - `04_Expediente_Final`
   - `Fuentes_Verificadas`
   - `Exportaciones_PDF`

5. Si alguna carpeta no existe y tienes permisos para crearla:
   1. Selecciona **Nuevo**.
   2. Selecciona **Carpeta**.
   3. Escribe exactamente el nombre faltante.
   4. Repite hasta completar la estructura.

6. Abre la carpeta:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/01_Prompts/
   ```

7. Selecciona **Nuevo > Documento de Word**.
8. Asigna inicialmente el nombre:

   ```text
   01_Guia_Prompts_NOVA_Hydrate_v1.0
   ```

9. Abre el documento en la aplicación de escritorio de Word, si está disponible:
   1. En Word para la Web, selecciona **Abrir en la aplicación de escritorio**.
   2. Confirma que Word muestra tu cuenta corporativa en la esquina superior derecha.
   3. Comprueba que el icono de guardado indica que el archivo se almacena en OneDrive.

10. Selecciona **Archivo > Opciones > Idioma** y confirma que el idioma de edición sea **Español (España)**.
11. En **Archivo > Opciones > Avanzadas**, revisa que el uso de separadores del sistema esté habilitado. La configuración regional del equipo debe usar coma como separador decimal.
12. Inserta al inicio del documento el siguiente título y aplícale el estilo **Título**:

   ```text
   Guía corporativa de prompts parametrizados
   NOVA Hydrate
   ```

13. Debajo del título, agrega esta ficha de control:

   | Campo | Valor |
   |---|---|
   | Proyecto | NOVA Hydrate |
   | Entregable | Guía corporativa de prompts parametrizados |
   | Versión | v1.0 |
   | Fecha | [Inserta la fecha actual en formato dd/MM/yyyy] |
   | Autor/a | [Tu nombre y apellidos] |
   | Ubicación | `/01_Prompts/01_Guia_Prompts_NOVA_Hydrate_v1.0.docx` |
   | Estado | Borrador para validación |
   | Clasificación | Uso interno del curso |

14. Guarda el documento con **Ctrl+S**.

**Resultado esperado:**

Existe un archivo Word llamado `01_Guia_Prompts_NOVA_Hydrate_v1.0.docx` dentro de la carpeta `01_Prompts`, con título, ficha de control y guardado activo en OneDrive for Business.

**Verificación:**

- El nombre del documento sigue la convención corporativa.
- La ruta del archivo contiene `NOVA_Hydrate/01_Prompts`.
- El documento no está guardado en Escritorio, Descargas ni una unidad local.
- La fecha utiliza el formato `dd/MM/yyyy`.
- El idioma de edición mostrado por Word es Español (España).

---

### Paso 2. Definir el reto de innovación y los parámetros maestros de NOVA Hydrate

**Objetivo:** Establecer los datos base que se reutilizarán como variables en todos los *prompts* de la guía.

**Instrucciones:**

1. Después de la ficha de control, inserta un salto de página con **Ctrl+Intro**.
2. Escribe el encabezado de nivel 1:

   ```text
   1. Reto de innovación y parámetros maestros
   ```

3. Agrega el siguiente texto introductorio:

   > NOVA Hydrate es una marca piloto de botellas térmicas reutilizables diseñada para responder a necesidades de hidratación cotidiana, movilidad urbana y reducción del uso de envases de un solo uso. Los parámetros de esta sección son obligatorios y deben reutilizarse de forma consistente en las solicitudes dirigidas a Copilot.

4. Inserta una tabla con tres columnas: **Parámetro**, **Valor inicial** y **Uso en prompts**.
5. Completa la tabla con los siguientes valores. Puedes adaptar los elementos marcados como preliminares durante una iteración posterior, pero no debes eliminar el carácter de hipótesis si no existe evidencia validada.

| Parámetro | Valor inicial | Uso en prompts |
|---|---|---|
| `[MARCA]` | NOVA Hydrate | Nombre temporal del proyecto y referencia en entregables |
| `[PRODUCTO]` | Línea de botellas térmicas reutilizables | Define la categoría de producto |
| `[MERCADO]` | España, con foco inicial en grandes áreas urbanas | Delimita geografía y evita generalizaciones globales |
| `[SEGMENTO_PRINCIPAL]` | Profesionales urbanos de 25 a 40 años | Delimita audiencia principal |
| `[NECESIDAD]` | Mantener bebidas a temperatura adecuada durante desplazamientos, trabajo híbrido y actividades cotidianas | Orienta necesidades funcionales y de contexto |
| `[PROPUESTA_VALOR_PRELIMINAR]` | Hidratación reutilizable, funcional y estética para rutinas urbanas exigentes | Debe tratarse como hipótesis inicial |
| `[RANGO_PRECIO]` | 25 € a 45 € | Orienta el posicionamiento de valor medio-alto accesible |
| `[CANALES]` | Comercio electrónico propio, marketplaces seleccionados, tiendas de diseño, gimnasios corporativos y puntos de venta urbanos | Limita recomendaciones de distribución |
| `[TONO_MARCA]` | Claro, optimista, contemporáneo, útil y responsable; evitar tono moralizante | Orienta identidad verbal |
| `[COMPETIDORES_INICIALES]` | Marcas de botellas térmicas reutilizables, marcas de *lifestyle* urbano y productos promocionales de bajo coste | Punto de partida; requiere identificación y validación específica |
| `[RESTRICCIONES_SOSTENIBILIDAD]` | Evitar afirmaciones ambientales absolutas; priorizar durabilidad, reutilización, reparabilidad, materiales trazables y embalaje reducido | Limita mensajes y afirmaciones comerciales |
| `[OBJETIVO_NEGOCIO]` | Explorar una propuesta diferenciada y viable para una marca emergente | Criterio para priorizar recomendaciones |
| `[IDIOMA_SALIDA]` | Español (España) | Consistencia lingüística |
| `[AUDIENCIA_EJECUTIVA]` | Responsables de diseño, marketing, negocio y sostenibilidad | Ajusta resúmenes y presentaciones |
| `[FECHA_CORTE]` | [Fecha actual] | Indica el límite temporal de investigación y revisión |

6. Agrega, después de la tabla, el encabezado de nivel 2:

   ```text
   1.1 Reglas de uso de parámetros
   ```

7. Incluye estas reglas como lista con viñetas:

   - Usar los nombres de variables entre corchetes cuando el *prompt* vaya a reutilizarse en otros proyectos o versiones.
   - Sustituir las variables por datos confirmados antes de ejecutar solicitudes críticas.
   - Identificar explícitamente los valores preliminares como hipótesis.
   - No afirmar beneficios ambientales, precios de competencia, cuotas de mercado ni tendencias como hechos sin fuente verificable.
   - Registrar fuentes y evidencias validadas en la carpeta `Fuentes_Verificadas`.
   - Solicitar a Copilot que separe hechos, hipótesis, recomendaciones y preguntas pendientes.
   - Priorizar siempre la decisión humana cuando exista incertidumbre, impacto reputacional, riesgo regulatorio o implicación comercial.

8. Guarda el archivo.

**Resultado esperado:**

El documento contiene una sección de parámetros maestros que define de forma reutilizable el producto, el mercado, la audiencia, los canales, el rango de precio, el tono y las restricciones de sostenibilidad de NOVA Hydrate.

**Verificación:**

- La tabla contiene al menos 15 parámetros.
- Los campos preliminares se identifican como hipótesis o valores iniciales.
- Las restricciones de sostenibilidad prohíben afirmaciones absolutas o no verificadas.
- El mercado se limita inicialmente a España y a entornos urbanos, en lugar de asumir un mercado global.

---

### Paso 3. Documentar los marcos corporativos de prompting

**Objetivo:** Incorporar los dos marcos de prompting utilizados en la práctica y relacionarlos con las necesidades del proyecto.

**Instrucciones:**

1. Inserta un salto de página.
2. Crea el encabezado de nivel 1:

   ```text
   2. Marcos corporativos para diseñar prompts
   ```

3. Agrega un breve párrafo:

   > Los prompts de esta guía no son preguntas genéricas. Cada solicitud debe proporcionar contexto suficiente, definir una tarea concreta, establecer límites y pedir un resultado utilizable. Copilot acelera la exploración y organización de alternativas; la revisión de evidencia, la interpretación y la decisión final son responsabilidad del equipo humano.

4. Crea el encabezado de nivel 2:

   ```text
   2.1 Marco Rol-Contexto-Tarea-Formato-Criterios (RCTFC)
   ```

5. Inserta una tabla con las siguientes columnas y contenido:

| Componente | Pregunta de control | Aplicación en NOVA Hydrate |
|---|---|---|
| Rol | ¿Desde qué especialidad debe responder Copilot? | Estratega de marca, analista de tendencias, investigador de consumo o asesor de comunicación ejecutiva |
| Contexto | ¿Qué información necesita conocer? | Producto, mercado español, segmento urbano, canales, precio, tono y restricciones |
| Tarea | ¿Qué debe producir o analizar? | Comparar, proponer, segmentar, resumir, identificar riesgos o formular preguntas |
| Formato | ¿Cómo se debe presentar la respuesta? | Tabla, matriz, lista priorizada, esquema de diapositivas o resumen ejecutivo |
| Criterios | ¿Cómo se evaluará la calidad? | Diferenciación, viabilidad, claridad, trazabilidad, utilidad ejecutiva y rigor |

6. Debajo de la tabla, incluye esta plantilla reutilizable:

   ```text
   Rol:
   Actúa como [ROL].

   Contexto:
   Estamos desarrollando [MARCA], una [PRODUCTO] para [SEGMENTO_PRINCIPAL] en [MERCADO].
   La propuesta de valor preliminar es [PROPUESTA_VALOR_PRELIMINAR].
   El rango de precio previsto es [RANGO_PRECIO].
   Los canales considerados son [CANALES].
   El tono de marca es [TONO_MARCA].
   Debes respetar [RESTRICCIONES_SOSTENIBILIDAD].

   Tarea:
   [TAREA_ESPECÍFICA].

   Formato:
   Presenta el resultado como [FORMATO_DE_SALIDA].

   Criterios:
   Prioriza [CRITERIOS_DE_CALIDAD].
   Diferencia claramente hechos verificados, hipótesis, recomendaciones y preguntas pendientes.
   No inventes datos, fuentes, competidores, precios ni afirmaciones de sostenibilidad.
   Responde en [IDIOMA_SALIDA].
   ```

7. Crea el encabezado de nivel 2:

   ```text
   2.2 Marco Objetivo-Contexto-Datos-Instrucciones-Validación (OCDIV)
   ```

8. Inserta una segunda tabla:

| Componente | Propósito | Aplicación en NOVA Hydrate |
|---|---|---|
| Objetivo | Define la decisión o resultado perseguido | Preparar información para decidir un posicionamiento inicial |
| Contexto | Describe el entorno de negocio y audiencia | Marca emergente de hidratación reutilizable urbana |
| Datos | Delimita las entradas disponibles y sus límites | Parámetros maestros, fuentes aportadas, fecha de corte |
| Instrucciones | Establece la acción, estructura y restricciones | Analizar, proponer, comparar y entregar en una tabla |
| Validación | Exige distinguir evidencia de hipótesis | Solicitar fuentes, nivel de confianza y preguntas abiertas |

9. Agrega la siguiente plantilla OCDIV:

   ```text
   Objetivo:
   Ayudar a [AUDIENCIA_EJECUTIVA] a decidir [DECISIÓN_O_ENTREGABLE].

   Contexto:
   [MARCA] desarrolla [PRODUCTO] para [SEGMENTO_PRINCIPAL] en [MERCADO].

   Datos:
   Usa únicamente los parámetros proporcionados y las fuentes adjuntas o citadas.
   Fecha de corte: [FECHA_CORTE].
   Si falta información, indícalo como limitación.

   Instrucciones:
   [INSTRUCCIÓN_PRINCIPAL].
   Considera [RANGO_PRECIO], [CANALES], [TONO_MARCA] y [RESTRICCIONES_SOSTENIBILIDAD].

   Validación:
   Clasifica cada afirmación como: Hecho verificado, Hipótesis, Recomendación o Pregunta pendiente.
   Indica qué evidencia adicional sería necesaria para validar conclusiones relevantes.
   No presentes inferencias como datos confirmados.
   ```

10. Añade un cuadro de texto o una nota destacada titulada **Principio de revisión humana**, con este contenido:

    > Antes de incorporar una salida de Copilot a un documento ejecutivo, el equipo debe comprobar la coherencia con los parámetros del proyecto, revisar la calidad de las fuentes, eliminar afirmaciones no demostradas y documentar las decisiones tomadas.

11. Guarda el documento.

**Resultado esperado:**

La guía contiene una explicación operativa de los marcos RCTFC y OCDIV, junto con plantillas parametrizadas que se pueden copiar y adaptar en Copilot Chat o Copilot en Word.

**Verificación:**

- Ambos marcos están incluidos y diferenciados.
- Cada marco contempla contexto, tarea o instrucciones, formato o estructura, restricciones y validación.
- Las plantillas incluyen variables entre corchetes.
- La guía afirma explícitamente que Copilot no sustituye la revisión profesional.

---

### Paso 4. Crear prompts para investigación de mercado y necesidades del cliente

**Objetivo:** Diseñar prompts reutilizables para investigar tendencias, segmentación, necesidades y oportunidades de mercado sin confundir hipótesis con evidencia.

**Instrucciones:**

1. Inserta un salto de página.
2. Crea el encabezado de nivel 1:

   ```text
   3. Biblioteca de prompts parametrizados
   ```

3. Crea el encabezado de nivel 2:

   ```text
   3.1 Investigación de tendencias y contexto de mercado
   ```

4. Inserta una tabla con las columnas: **Código**, **Propósito**, **Marco**, **Prompt parametrizado** y **Salida esperada**.
5. Completa la primera fila con el siguiente prompt:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-01 | Formular hipótesis de tendencias relevantes | OCDIV | **Objetivo:** identificar tendencias que puedan influir en la adopción de [PRODUCTO] por [SEGMENTO_PRINCIPAL] en [MERCADO]. **Contexto:** [MARCA] explora una propuesta de valor basada en [PROPUESTA_VALOR_PRELIMINAR]. **Datos:** no asumas acceso a datos de mercado en tiempo real; usa solo información aportada, conocimiento general claramente delimitado o fuentes citadas. **Instrucciones:** propone hasta cinco tendencias o cambios de comportamiento potencialmente relevantes. Para cada una, explica la relación con el producto, el posible impacto, el nivel de confianza y una pregunta de investigación que permita validarla. **Validación:** clasifica cada elemento como hecho verificado, hipótesis o recomendación. No inventes estadísticas ni estudios. | Tabla con tendencia, relación con NOVA Hydrate, tipo de afirmación, impacto, confianza y pregunta de validación |

6. Agrega una segunda fila para segmentación:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-02 | Proponer segmentos de cliente prioritarios | RCTFC | **Rol:** actúa como investigador de comportamiento del consumidor. **Contexto:** [MARCA] desarrolla [PRODUCTO] para [SEGMENTO_PRINCIPAL] en [MERCADO], con rango de precio [RANGO_PRECIO] y canales [CANALES]. **Tarea:** propone tres microsegmentos prioritarios dentro del público urbano de 25 a 40 años. Describe su contexto de uso, motivaciones, barreras, criterios de compra y canal más probable. **Formato:** tabla comparativa. **Criterios:** evita asumir datos demográficos no aportados; distingue observaciones plausibles de hipótesis que requieren entrevistas o encuestas. | Tabla con microsegmento, situación de uso, motivaciones, barreras, canal y validación requerida |

7. Crea el encabezado de nivel 2:

   ```text
   3.2 Necesidades del cliente y oportunidades de producto
   ```

8. Añade el prompt P-03:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-03 | Identificar necesidades funcionales, emocionales y sociales | RCTFC | **Rol:** actúa como especialista en investigación de experiencia de cliente. **Contexto:** el producto es [PRODUCTO], dirigido a [SEGMENTO_PRINCIPAL]. La necesidad general es [NECESIDAD]. **Tarea:** identifica necesidades funcionales, emocionales y sociales relacionadas con hidratación, movilidad urbana, trabajo híbrido y uso de productos reutilizables. **Formato:** matriz de necesidades con columnas: necesidad, evidencia disponible, hipótesis, posible respuesta de producto, riesgo y método de validación. **Criterios:** no atribuyas necesidades al público como hechos si no existe evidencia; prioriza necesidades accionables para una marca emergente. | Matriz de necesidades y métodos de validación |

9. Añade el prompt P-04:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-04 | Preparar preguntas de investigación primaria | OCDIV | **Objetivo:** preparar una entrevista exploratoria para validar necesidades y barreras de [SEGMENTO_PRINCIPAL]. **Contexto:** se investiga la posible aceptación de [PRODUCTO] de [MARCA] en [MERCADO]. **Datos:** usa los parámetros maestros y las hipótesis identificadas en P-02 y P-03. **Instrucciones:** genera diez preguntas abiertas, neutrales y no sugestivas. Agrúpalas en hábitos, problemas actuales, criterios de compra, sostenibilidad y percepción de valor. **Validación:** indica qué hipótesis intenta comprobar cada pregunta y evita preguntas que den por hecho que la persona desea comprar el producto. | Guion de entrevista con pregunta, categoría e hipótesis asociada |

10. Agrega, bajo la tabla, una nota:

    > Los resultados de P-01, P-02 y P-03 no constituyen investigación de mercado validada. Deben utilizarse para definir búsquedas, entrevistas, encuestas o análisis de fuentes. Las evidencias verificadas deben archivarse con fecha, URL o referencia documental, autor, entidad emisora y síntesis en la carpeta `Fuentes_Verificadas`.

11. Guarda el documento.

**Resultado esperado:**

La guía incluye al menos cuatro prompts reutilizables para tendencias, segmentación, necesidades y preparación de investigación primaria.

**Verificación:**

- Cada prompt indica un objetivo o tarea específica.
- Ningún prompt solicita a Copilot inventar datos de mercado.
- Todos los prompts incluyen mecanismos de validación, preguntas abiertas o clasificación de afirmaciones.
- La salida esperada puede reutilizarse posteriormente en la matriz competitiva y el caso de negocio.

---

### Paso 5. Crear prompts para posicionamiento, identidad verbal y exploración de marca

**Objetivo:** Desarrollar prompts para generar y evaluar territorios de marca, nombres, tono de voz y mensajes de valor alineados con la estrategia preliminar.

**Instrucciones:**

1. Crea el encabezado de nivel 2:

   ```text
   3.3 Territorios de marca y posicionamiento
   ```

2. Agrega el prompt P-05:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-05 | Proponer territorios de posicionamiento | RCTFC | **Rol:** actúa como estratega de marca especializado en productos de consumo sostenible. **Contexto:** [MARCA] es una [PRODUCTO] para [SEGMENTO_PRINCIPAL] en [MERCADO]. La propuesta de valor inicial es [PROPUESTA_VALOR_PRELIMINAR], el precio previsto es [RANGO_PRECIO] y el tono es [TONO_MARCA]. **Tarea:** propone tres territorios de posicionamiento claramente diferenciados. Para cada territorio, define promesa de marca, público prioritario, beneficio funcional, beneficio emocional, códigos visuales sugeridos, oportunidad comercial y riesgo de diferenciación. **Formato:** tabla comparativa. **Criterios:** evita clichés de sostenibilidad, no uses afirmaciones ambientales absolutas y señala los supuestos utilizados. | Tabla con tres territorios de marca y sus riesgos |

3. Agrega el prompt P-06:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-06 | Evaluar territorios de marca | OCDIV | **Objetivo:** ayudar a [AUDIENCIA_EJECUTIVA] a seleccionar un territorio de marca inicial para [MARCA]. **Contexto:** compara los territorios propuestos para [PRODUCTO] dirigido a [SEGMENTO_PRINCIPAL]. **Datos:** utiliza únicamente los tres territorios proporcionados en el contenido adjunto. **Instrucciones:** evalúa cada territorio según claridad para el público, viabilidad para una marca emergente, coherencia con [RANGO_PRECIO], potencial de diferenciación y consistencia con [RESTRICCIONES_SOSTENIBILIDAD]. **Validación:** asigna valoración alta, media o baja; justifica cada valoración en dos frases; identifica la evidencia que faltaría para tomar una decisión definitiva. | Matriz de evaluación cualitativa y recomendación condicionada |

4. Crea el encabezado de nivel 2:

   ```text
   3.4 Naming, tono de voz y mensajes de valor
   ```

5. Agrega el prompt P-07:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-07 | Generar opciones de nombres y criterios de revisión | RCTFC | **Rol:** actúa como consultor de naming para marcas de consumo. **Contexto:** la marca se relaciona con [PRODUCTO], movilidad urbana, hidratación y reutilización. El tono deseado es [TONO_MARCA]. **Tarea:** propón hasta diez alternativas de nombre distintas de [MARCA] para exploración interna. Para cada alternativa, explica la idea conceptual, pronunciación aproximada en español, asociación emocional, posibles riesgos semánticos y cuestiones que requieren revisión legal o de disponibilidad digital. **Formato:** tabla. **Criterios:** no afirmes que un nombre está disponible legalmente, como dominio o en redes sociales; evita nombres demasiado descriptivos, confusos o que sugieran beneficios ambientales no demostrables. | Tabla de nombres candidatos y riesgos de validación |

6. Agrega el prompt P-08:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-08 | Definir tono de voz y mensajes de valor | RCTFC | **Rol:** actúa como director/a de identidad verbal. **Contexto:** [MARCA] ofrece [PRODUCTO] para [SEGMENTO_PRINCIPAL], con tono [TONO_MARCA]. **Tarea:** crea una guía verbal inicial con cinco atributos de voz, cinco principios de redacción, cinco expresiones recomendadas, cinco expresiones a evitar y tres mensajes de valor. **Formato:** tabla con categoría, propuesta, justificación y riesgo de interpretación. **Criterios:** usa español de España, evita promesas absolutas, tono moralizante y afirmaciones de sostenibilidad no verificadas. Los mensajes deben ser compatibles con un precio de [RANGO_PRECIO]. | Mini guía de identidad verbal y mensajes de valor |

7. Agrega un párrafo de control:

   > Las propuestas de nombres, eslóganes, mensajes, colores, símbolos o referencias visuales son materiales de exploración. Antes de su uso externo, deben pasar por revisión legal, lingüística, cultural, de propiedad intelectual y de disponibilidad en los canales digitales aplicables.

8. Guarda el documento.

**Resultado esperado:**

La guía incluye prompts para conceptualizar y comparar territorios de marca, explorar nombres y establecer una identidad verbal inicial.

**Verificación:**

- El prompt de territorios propone alternativas comparables y no solo una lista de ideas.
- El prompt de evaluación usa criterios de negocio y no presenta una recomendación como decisión definitiva.
- El prompt de naming exige revisión legal y de disponibilidad.
- El prompt de tono de voz evita promesas ambientales no demostrables.

---

### Paso 6. Crear prompts para análisis competitivo, riesgos y comunicación ejecutiva

**Objetivo:** Preparar solicitudes que alimenten la futura matriz competitiva, el caso de negocio y la presentación ejecutiva del proyecto.

**Instrucciones:**

1. Crea el encabezado de nivel 2:

   ```text
   3.5 Análisis competitivo y riesgos
   ```

2. Agrega el prompt P-09:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-09 | Diseñar una matriz competitiva verificable | OCDIV | **Objetivo:** preparar una estructura de análisis competitivo para [MARCA]. **Contexto:** [MARCA] desarrolla [PRODUCTO] para [SEGMENTO_PRINCIPAL] en [MERCADO]. Los competidores iniciales son [COMPETIDORES_INICIALES]. **Datos:** no supongas características, precios, certificaciones ni posicionamientos sin una fuente aportada. **Instrucciones:** crea una matriz con columnas para competidor, categoría, propuesta de valor declarada, rango de precio observado, canal, atributos de producto, evidencia disponible, fecha de consulta, nivel de confianza y vacíos de información. **Validación:** marca como “pendiente de verificar” cualquier campo sin fuente primaria o secundaria confiable. | Plantilla de matriz competitiva para Excel |

3. Agrega el prompt P-10:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-10 | Identificar riesgos iniciales | RCTFC | **Rol:** actúa como asesor de riesgos de producto y marca para una empresa emergente. **Contexto:** [MARCA] evalúa lanzar [PRODUCTO] en [MERCADO], mediante [CANALES], con precio [RANGO_PRECIO] y restricciones [RESTRICCIONES_SOSTENIBILIDAD]. **Tarea:** identifica riesgos iniciales en las dimensiones de mercado, producto, sostenibilidad, comunicación, operaciones y reputación. **Formato:** matriz de riesgos con riesgo, supuesto asociado, probabilidad cualitativa, impacto cualitativo, señal de alerta, acción de mitigación y responsable sugerido. **Criterios:** diferencia riesgos basados en hechos aportados de riesgos hipotéticos; evita lenguaje alarmista y no ofrezcas asesoramiento legal concluyente. | Matriz de riesgos iniciales |

4. Crea el encabezado de nivel 2:

   ```text
   3.6 Resumen ejecutivo y preparación de presentación
   ```

5. Agrega el prompt P-11:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-11 | Preparar un resumen ejecutivo | OCDIV | **Objetivo:** redactar un resumen ejecutivo para [AUDIENCIA_EJECUTIVA] sobre el avance inicial de [MARCA]. **Contexto:** el proyecto explora [PRODUCTO] para [SEGMENTO_PRINCIPAL] en [MERCADO]. **Datos:** utiliza exclusivamente los hallazgos, hipótesis, fuentes y decisiones incluidas en el documento o texto adjunto. **Instrucciones:** redacta un resumen de máximo 250 palabras con reto, oportunidad, propuesta preliminar, principales hipótesis, riesgos, evidencia disponible, decisiones requeridas y siguientes pasos. **Validación:** etiqueta cualquier conclusión no respaldada como hipótesis; no añadas cifras, fuentes ni decisiones inexistentes. | Resumen ejecutivo estructurado de máximo 250 palabras |

6. Agrega el prompt P-12:

| Código | Propósito | Marco | Prompt parametrizado | Salida esperada |
|---|---|---|---|---|
| P-12 | Proponer estructura de presentación ejecutiva | RCTFC | **Rol:** actúa como consultor de comunicación ejecutiva. **Contexto:** debemos presentar el proyecto [MARCA] a [AUDIENCIA_EJECUTIVA]. La información disponible incluye parámetros maestros, hallazgos verificados, hipótesis, territorios de marca, riesgos y decisiones pendientes. **Tarea:** propone una estructura de ocho diapositivas para PowerPoint. **Formato:** tabla con número de diapositiva, título, mensaje clave, evidencia necesaria, visual recomendado y decisión o pregunta asociada. **Criterios:** cada diapositiva debe comunicar una idea principal; separar evidencia de hipótesis; evitar sobrecargar texto; priorizar decisiones que puedan tratarse en la reunión `Comité NOVA Hydrate - Validación Ejecutiva`. | Guion de ocho diapositivas para PowerPoint |

7. Inserta un encabezado de nivel 1:

   ```text
   4. Criterios de verificación y trazabilidad
   ```

8. Crea una tabla con estas columnas: **Tipo de contenido**, **Definición**, **Tratamiento permitido**, **Evidencia requerida** y **Destino de almacenamiento**.

| Tipo de contenido | Definición | Tratamiento permitido | Evidencia requerida | Destino de almacenamiento |
|---|---|---|---|---|
| Hecho verificado | Información respaldada por una fuente identificable y revisada | Puede incluirse como hecho con cita y fecha | Fuente primaria, fuente institucional, estudio confiable o evidencia documental | `Fuentes_Verificadas` |
| Hipótesis | Suposición razonable que todavía no se ha comprobado | Debe etiquetarse como hipótesis y convertirse en pregunta de investigación | Plan de validación, entrevista, encuesta o búsqueda documental | Documento de trabajo y registro de validación |
| Recomendación | Propuesta de acción basada en objetivos, evidencia disponible y criterio profesional | Puede presentarse con justificación, condiciones y riesgos | Relación clara con evidencia o supuestos | Guía, caso de negocio o expediente |
| Pregunta pendiente | Información crítica que falta para tomar una decisión | Debe asignarse a un responsable y método de investigación | No aplica; requiere plan de obtención | Registro de decisiones o plan de investigación |
| Afirmación no aceptable | Dato inventado, fuente inexistente, beneficio absoluto o conclusión sin soporte | Debe eliminarse o reformularse como hipótesis | No disponible o no verificable | No almacenar como evidencia |

9. Agrega esta lista de comprobación antes de usar cualquier salida de Copilot:

   - ¿La respuesta responde al rol, contexto, tarea y formato solicitados?
   - ¿Se mantuvieron los parámetros maestros de NOVA Hydrate?
   - ¿Se separaron hechos verificados, hipótesis, recomendaciones y preguntas pendientes?
   - ¿Existen fuentes reales y accesibles para las afirmaciones relevantes?
   - ¿La respuesta evita promesas ambientales, legales, sanitarias o comerciales no demostradas?
   - ¿El resultado es útil para una decisión, un documento o una investigación posterior?
   - ¿Se registró la fecha de consulta y el nivel de confianza cuando corresponde?

10. Guarda el documento.

**Resultado esperado:**

La guía contiene prompts para análisis competitivo, riesgos, resumen ejecutivo y estructura de presentación, además de una política práctica de verificación y trazabilidad.

**Verificación:**

- La plantilla competitiva contempla fuente, fecha de consulta y nivel de confianza.
- El análisis de riesgos incluye supuestos, probabilidad, impacto y mitigación.
- El resumen ejecutivo limita la extensión y exige trazabilidad.
- La estructura de presentación separa evidencia de hipótesis.
- La tabla de criterios de verificación contiene, como mínimo, hecho verificado, hipótesis, recomendación y pregunta pendiente.

---

### Paso 7. Probar un prompt con Copilot y documentar una iteración

**Objetivo:** Validar que la guía produce solicitudes claras, utilizables y mejorables mediante interacción iterativa con Copilot.

**Instrucciones:**

1. Selecciona el prompt **P-05: Proponer territorios de posicionamiento**.
2. Copia el texto del prompt en Microsoft 365 Copilot Chat o en Copilot dentro de Word.
3. Sustituye las variables principales por los valores definidos en la sección de parámetros maestros:
   - `[MARCA]`: NOVA Hydrate
   - `[PRODUCTO]`: línea de botellas térmicas reutilizables
   - `[SEGMENTO_PRINCIPAL]`: profesionales urbanos de 25 a 40 años
   - `[MERCADO]`: España, con foco inicial en grandes áreas urbanas
   - `[RANGO_PRECIO]`: 25 € a 45 €
   - `[TONO_MARCA]`: claro, optimista, contemporáneo, útil y responsable
   - `[RESTRICCIONES_SOSTENIBILIDAD]`: evitar afirmaciones ambientales absolutas; priorizar durabilidad, reutilización, reparabilidad, materiales trazables y embalaje reducido

4. Envía el prompt.
5. Revisa el resultado antes de copiarlo al documento. Comprueba especialmente:
   - Si propone exactamente tres territorios diferenciados.
   - Si cada territorio incluye promesa, audiencia, beneficios, códigos visuales, oportunidad y riesgo.
   - Si diferencia supuestos de hechos.
   - Si evita cifras, certificaciones o afirmaciones ambientales no justificadas.

6. Si el resultado es demasiado genérico, utiliza una segunda instrucción de refinamiento. Copia y adapta este ejemplo:

   ```text
   Reduce la propuesta a tres territorios claramente distintos y evita expresiones genéricas como “sostenible”, “premium” o “innovador” sin explicarlas. Para cada territorio, indica qué necesidad urbana concreta atiende, qué elemento lo diferencia de una botella térmica convencional y qué supuesto debe validarse con usuarios o fuentes de mercado. Mantén el formato de tabla.
   ```

7. Inserta un salto de página en la guía y crea el encabezado de nivel 1:

   ```text
   5. Registro de prueba e iteración
   ```

8. Inserta una tabla con las columnas: **Elemento**, **Registro**.
9. Completa los siguientes campos:

| Elemento | Registro |
|---|---|
| Prompt probado | P-05: Proponer territorios de posicionamiento |
| Herramienta utilizada | Microsoft 365 Copilot Chat o Copilot en Word |
| Fecha de prueba | [dd/MM/yyyy] |
| Variables sustituidas | [Lista breve de variables utilizadas] |
| Calidad inicial de la respuesta | [Alta / Media / Baja] |
| Problemas detectados | [Ejemplo: territorios poco diferenciados, falta de riesgos, supuestos no explícitos] |
| Instrucción de refinamiento | [Pega la instrucción usada] |
| Cambio observado | [Describe en 2 o 3 frases] |
| Decisión | [Ejemplo: conservar prompt P-05 con ajuste de refinamiento] |
| Validación pendiente | [Ejemplo: validar territorios con entrevistas a usuarios] |

10. No copies respuestas completas de Copilot que contengan datos sin validar como si fueran evidencia. Si deseas conservar una salida para revisión, identifícala claramente como **borrador generado por IA**.
11. Guarda el documento y verifica que la sincronización de OneDrive se haya completado.

**Resultado esperado:**

El documento contiene un registro de prueba que demuestra una interacción iterativa: solicitud inicial, revisión crítica, refinamiento y decisión documentada.

**Verificación:**

- Se probó al menos un prompt de la biblioteca.
- El registro incluye fecha, herramienta, problema detectado y refinamiento.
- La salida de Copilot no se presenta como evidencia de mercado sin verificación.
- Se documenta al menos una validación pendiente.

---

### Paso 8. Revisar el formato, generar el PDF y preparar la entrega

**Objetivo:** Comprobar la calidad documental, mantener la trazabilidad de la versión y exportar una copia en PDF para revisión.

**Instrucciones:**

1. Revisa la estructura final del documento. Debe incluir, como mínimo:
   1. Ficha de control.
   2. Reto de innovación y parámetros maestros.
   3. Marcos RCTFC y OCDIV.
   4. Biblioteca de prompts.
   5. Criterios de verificación y trazabilidad.
   6. Registro de prueba e iteración.

2. En Word, aplica estilos consistentes:
   - **Título** para la portada.
   - **Encabezado 1** para secciones principales.
   - **Encabezado 2** para subsecciones.
   - Texto normal para explicaciones y prompts.
   - Tablas con encabezados visibles.

3. Inserta una tabla de contenido automática:
   1. Coloca el cursor después de la portada y ficha de control.
   2. Selecciona **Referencias > Tabla de contenido**.
   3. Elige una tabla automática.
   4. Actualiza la tabla si Word lo solicita.

4. Revisa la ortografía con **Revisar > Editor**.
5. Comprueba que todas las variables entre corchetes están justificadas:
   - Deben mantenerse como variables en las plantillas reutilizables.
   - Deben sustituirse solo en los ejemplos o pruebas ejecutadas.

6. Selecciona **Archivo > Guardar**.
7. Exporta una copia en PDF:
   1. Selecciona **Archivo > Exportar > Crear documento PDF/XPS** o **Archivo > Guardar como**.
   2. Selecciona el formato **PDF**.
   3. Guarda el archivo en:

      ```text
      /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/Exportaciones_PDF/
      ```

   4. Usa este nombre:

      ```text
      01_Guia_Prompts_NOVA_Hydrate_v1.0.pdf
      ```

8. Abre el PDF generado y comprueba:
   - Que la tabla de contenido funciona o muestra los títulos.
   - Que las tablas no están cortadas de forma ilegible.
   - Que los prompts son legibles.
   - Que la información de control y versión aparece correctamente.

9. Regresa a OneDrive y comprueba que existen ambos archivos:
   - `01_Prompts/01_Guia_Prompts_NOVA_Hydrate_v1.0.docx`
   - `Exportaciones_PDF/01_Guia_Prompts_NOVA_Hydrate_v1.0.pdf`

**Resultado esperado:**

El entregable Word está completo, estructurado, guardado en OneDrive y acompañado por una copia PDF de revisión.

**Verificación:**

- El archivo `.docx` y el archivo `.pdf` tienen el mismo número de versión.
- Ambos archivos están en las carpetas corporativas correctas.
- El documento tiene tabla de contenido y encabezados estructurados.
- No hay errores ortográficos críticos, tablas ilegibles ni afirmaciones no verificadas presentadas como hechos.

---

## Validación y pruebas

Realiza la siguiente validación final antes de considerar terminada la práctica.

| Criterio de aceptación | Método de comprobación | Resultado esperado |
|---|---|---|
| Ubicación corporativa correcta | Revisar ruta en OneDrive | El DOCX está en `01_Prompts` y el PDF en `Exportaciones_PDF` |
| Convención de nombre aplicada | Comparar nombre del archivo con la norma | `01_Guia_Prompts_NOVA_Hydrate_v1.0.docx` |
| Parámetros maestros completos | Revisar tabla de parámetros | Incluye producto, mercado, segmento, valor, precio, canales, tono, competidores y sostenibilidad |
| Uso de RCTFC | Revisar sección 2.1 | Existe una plantilla con rol, contexto, tarea, formato y criterios |
| Uso de OCDIV | Revisar sección 2.2 | Existe una plantilla con objetivo, contexto, datos, instrucciones y validación |
| Biblioteca de prompts | Contar códigos P-01 a P-12 | Existen al menos 12 prompts clasificados por propósito |
| Rigor de investigación | Revisar prompts P-01 a P-04 y P-09 | Se exige no inventar datos y clasificar el tipo de afirmación |
| Identidad de marca | Revisar prompts P-05 a P-08 | Incluye territorios, evaluación, naming y tono de voz |
| Riesgos y comunicación ejecutiva | Revisar P-10 a P-12 | Incluye matriz de riesgos, resumen ejecutivo y guion de presentación |
| Trazabilidad | Revisar sección 4 | Distingue hechos, hipótesis, recomendaciones y preguntas pendientes |
| Interacción iterativa | Revisar sección 5 | Hay evidencia de prueba, refinamiento y decisión |
| Calidad documental | Abrir DOCX y PDF | El contenido es legible, coherente y está correctamente versionado |

### Prueba funcional recomendada

Ejecuta nuevamente P-11 con un texto breve que contenga una mezcla de hechos, hipótesis y preguntas pendientes. Comprueba que Copilot:

1. No agrega cifras inexistentes.
2. Mantiene el límite de 250 palabras.
3. Señala las hipótesis como tales.
4. Incluye decisiones requeridas y siguientes pasos.
5. No convierte recomendaciones en hechos confirmados.

Si no cumple alguno de estos puntos, ajusta el prompt P-11 antes de cerrar la versión `v1.0`.

## Resolución de problemas

### Incidencia 1: Copilot produce respuestas genéricas o no respeta el formato solicitado

**Síntomas:**

- Copilot responde con párrafos extensos en lugar de una tabla.
- Las propuestas no se relacionan con profesionales urbanos de 25 a 40 años.
- La respuesta utiliza términos genéricos como “innovador”, “premium” o “sostenible” sin justificación.
- No separa hechos, hipótesis y recomendaciones.

**Causa probable:**

El prompt no contiene suficiente contexto, no especifica el formato de salida o no incluye criterios de validación explícitos. También puede haberse copiado una plantilla sin sustituir las variables principales.

**Solución:**

1. Comprueba que las variables `[PRODUCTO]`, `[SEGMENTO_PRINCIPAL]`, `[MERCADO]`, `[RANGO_PRECIO]` y `[RESTRICCIONES_SOSTENIBILIDAD]` estén sustituidas en la prueba.
2. Añade una instrucción precisa, por ejemplo:

   ```text
   Devuelve exclusivamente una tabla con las columnas indicadas. Limita la respuesta a tres propuestas. Para cada propuesta, separa “Hipótesis” de “Evidencia disponible” y señala una pregunta de validación.
   ```

3. Añade un criterio de calidad vinculado a la decisión, por ejemplo:

   ```text
   Prioriza alternativas viables para una marca emergente con precio de 25 € a 45 € y canales de comercio electrónico y venta urbana.
   ```

4. Registra el refinamiento en la sección **Registro de prueba e iteración**.

### Incidencia 2: El documento no se sincroniza en OneDrive o se guarda en una ubicación no permitida

**Síntomas:**

- Word muestra “Guardado en este equipo” en lugar de una ubicación corporativa.
- El archivo no aparece en OneDrive para la Web.
- Se observan conflictos de copia, iconos de sincronización pendientes o nombres duplicados.
- El PDF se encuentra en Descargas o Escritorio.

**Causa probable:**

El documento se creó localmente, OneDrive no ha iniciado sesión con la cuenta corporativa correcta, hay un conflicto de sincronización o se utilizó una ruta distinta de la estructura obligatoria.

**Solución:**

1. En Word, selecciona **Archivo > Guardar una copia**.
2. Elige **OneDrive - Contoso** o la biblioteca corporativa autorizada.
3. Navega manualmente a:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/01_Prompts/
   ```

4. Guarda el archivo con el nombre exacto:

   ```text
   01_Guia_Prompts_NOVA_Hydrate_v1.0.docx
   ```

5. Abre OneDrive para la Web y confirma que el archivo aparece en la ruta correcta.
6. Si existe un conflicto, conserva la versión más reciente revisando fecha y contenido; renombra las copias no definitivas como borradores y elimina únicamente las versiones duplicadas que no deban conservarse.
7. Repite la exportación del PDF directamente en la carpeta `Exportaciones_PDF`.

## Limpieza

1. Cierra Copilot Chat, Word y cualquier documento de prueba que no sea necesario.
2. Verifica que OneDrive haya terminado de sincronizar el archivo Word y el PDF.
3. Elimina archivos temporales locales creados fuera de OneDrive, siempre que no contengan información necesaria para el curso.
4. No elimines:
   - `01_Guia_Prompts_NOVA_Hydrate_v1.0.docx`
   - `01_Guia_Prompts_NOVA_Hydrate_v1.0.pdf`
   - Fuentes o registros de validación que hayan sido aprobados.
5. Si compartiste el documento para revisión, confirma que los permisos se limiten a participantes autorizados del proyecto.
6. Deja preparada la carpeta `02_Moodboard` para la siguiente práctica, que reutilizará los parámetros de producto, audiencia, tono y territorios de marca definidos en esta guía.

## Resumen

En esta práctica has creado una guía corporativa versionada para diseñar y reutilizar *prompts* en el proyecto NOVA Hydrate. Has definido parámetros maestros de marca, aplicado los marcos RCTFC y OCDIV, creado una biblioteca de doce prompts y establecido criterios para distinguir evidencia verificable de hipótesis generadas por IA.

La guía será la fuente de parámetros para el moodboard de la siguiente práctica, la matriz competitiva y el caso de negocio, así como para el expediente técnico final y la presentación ejecutiva. Recuerda que el valor de Copilot no reside en aceptar automáticamente sus respuestas, sino en usarlo de forma iterativa para formular alternativas, estructurar información, identificar vacíos y reforzar el criterio profesional.

### Recursos opcionales

- [Guía de Microsoft sobre Copilot en Word](https://support.microsoft.com/es-es/topic/bienvenido-a-copilot-en-word-2135e85f-a467-463b-b2f0-6b3f00cc4c5f)
- [Principios de interacción persona-IA de Microsoft](https://www.microsoft.com/en-us/research/project/guidelines-for-human-ai-interaction/)
- [Design Council: Double Diamond](https://www.designcouncil.org.uk/our-resources/framework-for-innovation/)
