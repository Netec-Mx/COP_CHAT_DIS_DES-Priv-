# Desarrollo de un tablero de concepto (Moodboard) textual y visual parametrizando los estilos estéticos de un producto piloto

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 90 minutos |
| Complejidad | Media |
| Nivel de Bloom | Crear |
| Producto piloto | NOVA Hydrate |
| Entregable principal | `02_Moodboard_NOVA_Hydrate_v1.0.pptx` |
| Entrada obligatoria | `01_Guia_Prompts_NOVA_Hydrate.docx` |
| Ubicación de trabajo | `/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/` |

## Descripción general

En esta práctica desarrollarás un moodboard textual y visual en PowerPoint para la marca piloto **NOVA Hydrate**. Partirás de los parámetros definidos en la Práctica 1 y utilizarás Microsoft 365 Copilot, PowerPoint y, cuando esté disponible, Microsoft Designer para explorar tres rutas estéticas comparables: **Minimalismo técnico**, **Naturaleza urbana** y **Energía cromática**.

El resultado será una presentación trazable que documente descriptores, paletas, materiales, tipografías, estilo fotográfico, escenarios de uso, atributos de empaque, prompts técnicos de mockup y una decisión razonada sobre la ruta visual principal y secundaria. Las salidas generadas por IA se tratarán como hipótesis creativas y deberán validarse con criterios de marca, audiencia, viabilidad, accesibilidad y diferenciación.

## Objetivos de aprendizaje

Al finalizar la práctica, podrás:

- [ ] Transformar los parámetros de marca de NOVA Hydrate en tres direcciones estéticas coherentes y diferenciadas.
- [ ] Aplicar prompts parametrizados con rol, contexto, audiencia, tarea, restricciones y formato de salida.
- [ ] Crear prompts técnicos para imágenes de referencia, fotografía de producto y mockups de empaque.
- [ ] Documentar la procedencia de las imágenes utilizadas, tanto generadas como incorporadas desde fuentes autorizadas.
- [ ] Seleccionar una ruta estética principal y una secundaria mediante una matriz de evaluación razonada.

## Requisitos previos

### Conocimientos requeridos

- Haber completado la Práctica 1 y comprender los parámetros de marca definidos para NOVA Hydrate.
- Conocer conceptos básicos de paleta cromática, contraste, composición, fotografía de producto, empaques y tipografía.
- Comprender que Copilot Chat genera propuestas exploratorias, no evidencia definitiva sobre mercado, tendencias o competencia.
- Saber aplicar el ciclo creativo asistido por IA: definir desafío, aportar contexto, generar alternativas, evaluar, refinar y seleccionar.

### Accesos requeridos

- Cuenta corporativa del tenant `contoso.onmicrosoft.com` o cuenta invitada autorizada.
- Acceso de lectura al archivo `01_Guia_Prompts_NOVA_Hydrate.docx`.
- Acceso de edición a la ruta corporativa:

```text
/OneDrive for Business/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
```

- Acceso a Microsoft PowerPoint, Word, Microsoft 365 Copilot Chat y Microsoft Designer si está habilitado.
- Acceso a la biblioteca corporativa de imágenes aprobadas, si Designer no está disponible.
- Acceso al equipo de Teams `LAB-Copilot-Diseno-Desarrollo` y al canal `Proyecto-NOVA-Hydrate`.

## Entorno de laboratorio

### Hardware de referencia

| Recurso | Requisito |
|---|---|
| Procesador | Intel Core i5 de 11.ª generación, AMD Ryzen 5 5000 Series o superior |
| Memoria | 16 GB mínimo; 32 GB recomendado |
| Almacenamiento | 20 GB libres en SSD |
| Pantalla | 1920 × 1080 mínimo; monitor adicional recomendado |
| Conectividad | 25 Mbps de descarga y 5 Mbps de carga como mínimo |
| Comunicación | Micrófono y cámara funcionales para Teams |

### Software de referencia

| Aplicación o servicio | Versión o línea de referencia |
|---|---|
| Windows 11 Enterprise | 24H2, compilación 26100.6584 |
| Microsoft 365 Apps for enterprise | Versión 2508, compilación 19127.20358 |
| Word, Excel y PowerPoint | Versión 2508, compilación 19127.20358 |
| Microsoft Teams | 25185.1002.3698 |
| Microsoft 365 Copilot | Línea de lanzamiento 2026.08 |
| Microsoft Designer | Línea de lanzamiento 2026.08 |
| Microsoft Edge | 139.0.3405.86 |

### Configuración obligatoria

Antes de crear archivos, verifica la siguiente configuración regional en Windows y Microsoft 365:

| Configuración | Valor obligatorio |
|---|---|
| Idioma | Español (España) |
| Zona horaria | Europe/Madrid |
| Formato de fecha | `dd/MM/yyyy` |
| Moneda | EUR |
| Separador decimal | Coma |

### Estructura de carpetas

Trabaja exclusivamente dentro de la carpeta corporativa del proyecto. Verifica o crea la siguiente estructura:

```text
/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
├── 01_Prompts/
├── 02_Moodboard/
├── 03_Caso_Negocio/
├── 04_Expediente_Final/
├── Fuentes_Verificadas/
└── Exportaciones_PDF/
```

Guarda el entregable de esta práctica en:

```text
/02_Moodboard/02_Moodboard_NOVA_Hydrate_v1.0.pptx
```

> **Importante:** No guardes entregables finales en Escritorio, Descargas, memorias USB ni unidades locales no administradas.

---

## Procedimiento paso a paso

### Paso 1. Verificar la entrada de la Práctica 1 y preparar el espacio de trabajo

**Objetivo:** Confirmar que los parámetros de marca de NOVA Hydrate están disponibles y preparar los archivos de trabajo trazables.

**Instrucciones:**

1. Abre OneDrive for Business con tu cuenta corporativa.
2. Navega a la ruta:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
   ```

3. Confirma que existe el archivo obligatorio:

   ```text
   01_Guia_Prompts_NOVA_Hydrate.docx
   ```

4. Abre el documento en Word.
5. Identifica y anota los parámetros obtenidos en la Práctica 1. Como mínimo, localiza:
   - Propósito o propuesta de valor de NOVA Hydrate.
   - Público objetivo.
   - Personalidad de marca.
   - Tono verbal.
   - Beneficio funcional y emocional.
   - Restricciones de comunicación.
   - Elementos visuales recomendados o que se deben evitar.
   - Criterios de sostenibilidad, accesibilidad o viabilidad definidos.
6. Crea, si no existe, la carpeta:

   ```text
   /02_Moodboard/
   ```

7. Abre PowerPoint y crea una presentación en blanco.
8. Guarda inmediatamente el archivo con el nombre:

   ```text
   02_Moodboard_NOVA_Hydrate_v1.0.pptx
   ```

9. Guarda el archivo dentro de `/02_Moodboard/`.
10. En la primera diapositiva, añade el título:

   ```text
   Moodboard de concepto — NOVA Hydrate
   Práctica 2: Exploración y selección de rutas estéticas
   ```

11. Añade el nombre del participante, fecha en formato `dd/MM/yyyy` y versión `v1.0`.

**Resultado esperado:**

- Archivo de PowerPoint creado en la ubicación corporativa.
- Parámetros de marca de la Práctica 1 disponibles para consulta.
- Primera diapositiva de portada completada.

**Verificación:**

- El nombre del archivo termina en `.pptx` y sigue la convención `NN_TipoEntregable_NOVA_Hydrate_vMAJOR.MINOR.ext`.
- El archivo aparece sincronizado en OneDrive for Business.
- No existen copias finales guardadas en ubicaciones locales no administradas.

---

### Paso 2. Extraer y sintetizar los parámetros de marca con Copilot

**Objetivo:** Convertir la información de la guía de prompts en un brief visual operativo para el moodboard.

**Instrucciones:**

1. Con el documento `01_Guia_Prompts_NOVA_Hydrate.docx` abierto, utiliza Copilot en Word o Microsoft 365 Copilot Chat.
2. Si utilizas Copilot Chat, adjunta el documento corporativo o referencia el archivo desde OneDrive, según las capacidades habilitadas en tu tenant.
3. Introduce el siguiente prompt. Sustituye los campos entre corchetes con datos reales de la Práctica 1 cuando sea necesario:

```text
Actúa como estratega de marca y director de arte para productos de consumo.

Analiza el documento "01_Guia_Prompts_NOVA_Hydrate.docx" y crea un brief visual
operativo para el desarrollo de un moodboard de NOVA Hydrate.

Contexto: NOVA Hydrate es [describir producto y propuesta de valor según la Práctica 1].
Público objetivo: [describir audiencia, hábitos, motivaciones y contexto].
Objetivo: traducir los parámetros de marca en rutas visuales comparables para un empaque
y comunicación digital de producto.

Identifica y organiza:
1. atributos de marca obligatorios;
2. emociones que se deben activar;
3. códigos visuales recomendados;
4. elementos visuales, verbales o culturales que se deben evitar;
5. requisitos de accesibilidad y legibilidad;
6. restricciones de viabilidad de empaque, impresión o producción;
7. preguntas que requieren validación externa antes de tomar una decisión.

Presenta la salida en una tabla con las columnas:
Categoría, parámetro, implicación visual, riesgo si no se cumple y acción recomendada.

No presentes afirmaciones de mercado como hechos si no están respaldadas por fuentes del documento.
```

4. Revisa la respuesta de Copilot.
5. Corrige cualquier interpretación inconsistente con el documento original.
6. En PowerPoint, crea la diapositiva 2 con el título:

   ```text
   Brief visual operativo: parámetros de NOVA Hydrate
   ```

7. Resume en la diapositiva entre seis y diez parámetros clave. Utiliza una tabla o bloques visuales, no párrafos extensos.
8. Incluye una nota al pie:

   ```text
   Fuente: síntesis del documento 01_Guia_Prompts_NOVA_Hydrate.docx. Las propuestas de Copilot se revisaron y validaron por el participante.
   ```

**Resultado esperado:**

- Diapositiva 2 con un brief visual claro y accionable.
- Lista de restricciones que orientará la creación de las tres rutas estéticas.
- Separación explícita entre parámetros confirmados e hipótesis que requieren validación.

**Verificación:**

- La diapositiva incluye audiencia, propósito, atributos de marca, restricciones y criterios de accesibilidad.
- No se presentan tendencias, datos de competencia o afirmaciones de mercado sin fuente verificable.
- Los parámetros de la diapositiva coinciden con el documento de la Práctica 1.

---

### Paso 3. Generar alternativas de dirección estética mediante brainstorming asistido

**Objetivo:** Producir propuestas divergentes para las tres rutas obligatorias sin adoptar la primera respuesta generada por IA.

**Instrucciones:**

1. Abre Microsoft 365 Copilot Chat.
2. Utiliza el siguiente prompt parametrizado:

```text
Actúa como director de arte especializado en marcas de bebidas funcionales y empaques
de consumo contemporáneo.

Contexto del proyecto:
NOVA Hydrate es [describir producto, promesa y personalidad de marca].
El público objetivo es [describir audiencia de la Práctica 1].
La marca debe comunicar [beneficios y tono], evitando [códigos, clichés o elementos prohibidos].

Tarea:
Desarrolla tres rutas estéticas claramente diferenciadas para un moodboard de concepto:
1. "Minimalismo técnico"
2. "Naturaleza urbana"
3. "Energía cromática"

Para cada ruta, incluye:
- concepto rector en una frase;
- cinco descriptores visuales;
- intención emocional;
- paleta de cinco colores con nombre, código HEX y función;
- materiales o acabados de empaque;
- tipografías de referencia o características tipográficas;
- recursos gráficos;
- estilo fotográfico;
- escenarios de uso;
- atributos de empaque;
- riesgos de percepción;
- recomendación de accesibilidad y legibilidad.

Restricciones:
- Evita clichés fitness agresivos, promesas de salud no verificables y estereotipos de género.
- Prioriza claridad de información, escalabilidad de la gama y viabilidad para empaque.
- Diferencia las tres rutas de forma real; no cambies únicamente los colores.
- No atribuyas tendencias o preferencias de consumidores sin indicar que requieren validación.

Formato de salida:
Presenta una tabla comparativa seguida de una lista de riesgos y preguntas de validación.
```

3. Revisa si las tres rutas son realmente distintas. Evalúa especialmente:
   - Diferencia conceptual.
   - Diferencia cromática.
   - Diferencia en materiales y acabados.
   - Diferencia en tono fotográfico.
   - Diferencia en códigos culturales y visuales.
4. Si las propuestas son demasiado similares, utiliza este prompt de refinamiento:

```text
Las tres rutas anteriores son insuficientemente diferenciadas. Reformula las propuestas
para aumentar el contraste conceptual entre ellas.

Mantén los parámetros de NOVA Hydrate, pero asegura que:
- "Minimalismo técnico" priorice precisión, estructura, claridad y funcionalidad;
- "Naturaleza urbana" combine materialidad sostenible, entorno cotidiano y vegetación integrada;
- "Energía cromática" exprese dinamismo, optimismo y modularidad sin usar neón agresivo.

Indica en cada ruta qué decisión visual la hace incompatible con las otras dos.
```

5. Crea las diapositivas 3, 4 y 5 en PowerPoint:
   - Diapositiva 3: `Ruta 1 — Minimalismo técnico`
   - Diapositiva 4: `Ruta 2 — Naturaleza urbana`
   - Diapositiva 5: `Ruta 3 — Energía cromática`
6. En cada diapositiva incorpora, como mínimo:
   - Concepto rector.
   - Cinco descriptores.
   - Intención emocional.
   - Riesgo de percepción principal.
   - Una frase de diferenciación respecto a las otras rutas.

**Resultado esperado:**

- Tres rutas estéticas iniciales diferenciadas.
- Cada ruta contiene una base conceptual y visual justificable.
- Las rutas responden al público, al propósito de marca y a las restricciones del proyecto.

**Verificación:**

- Cada ruta puede explicarse en una frase distinta sin depender solo de los colores.
- Se identifican riesgos de percepción, por ejemplo: frialdad excesiva, apariencia poco premium, sobrecarga visual o confusión con categorías competidoras.
- Las propuestas no contienen afirmaciones comerciales o de salud no verificadas.

---

### Paso 4. Construir la paleta, los materiales, las tipografías y los atributos de empaque

**Objetivo:** Traducir cada ruta conceptual a decisiones visuales específicas y comparables.

**Instrucciones:**

1. Para cada ruta, solicita a Copilot una ampliación técnica. Utiliza el siguiente prompt y ejecútalo tres veces, sustituyendo `[NOMBRE DE LA RUTA]`:

```text
Actúa como diseñador de empaques y especialista en sistemas visuales accesibles.

Desarrolla la ruta estética "[NOMBRE DE LA RUTA]" para NOVA Hydrate usando los parámetros
de marca definidos anteriormente.

Genera una especificación de moodboard con:
1. paleta de cinco colores: nombre, HEX, uso principal y contraste recomendado;
2. dos materiales base de empaque y dos acabados posibles;
3. dos estilos tipográficos de referencia y criterios de legibilidad;
4. recursos gráficos permitidos;
5. recursos gráficos que se deben evitar;
6. composición frontal sugerida para una botella o lata;
7. jerarquía de información para nombre, sabor, beneficio y volumen;
8. recomendación de accesibilidad para tamaño de texto, contraste y códigos de sabor.

Restricciones:
- Debe ser viable para impresión comercial y reproducción digital.
- No dependas exclusivamente del color para diferenciar sabores o variantes.
- No indiques certificaciones, materiales o beneficios ambientales si no están confirmados.
- Si propones un material o acabado de riesgo, indícalo como hipótesis sujeta a validación.

Devuelve una tabla técnica concisa.
```

2. Selecciona las propuestas que mejor se ajusten a la guía de prompts de la Práctica 1.
3. En PowerPoint, amplía las diapositivas 3, 4 y 5 con los siguientes bloques:
   - Paleta cromática con muestras de color y códigos HEX.
   - Materiales y acabados.
   - Tipografías de referencia.
   - Recursos gráficos.
   - Atributos de empaque.
4. Para las muestras de color:
   - Inserta cinco rectángulos por ruta.
   - Añade debajo el nombre del color y su código HEX.
   - Asegura contraste suficiente entre texto y fondo.
5. Para las tipografías:
   - No es obligatorio instalar tipografías nuevas.
   - Si una fuente propuesta no está disponible, utiliza una alternativa de Microsoft 365 y documenta la equivalencia.
   - Ejemplo: una sans serif geométrica puede representarse mediante Aptos, Avenir Next si está disponible, o una fuente corporativa aprobada.
6. Añade una nota breve de accesibilidad en cada ruta, por ejemplo:

   ```text
   Accesibilidad: el sabor se identificará mediante texto, icono y patrón; el color no será el único indicador.
   ```

**Resultado esperado:**

- Tres diapositivas de ruta con componentes visuales concretos.
- Paletas con códigos reproducibles.
- Consideraciones de accesibilidad y viabilidad visibles.

**Verificación:**

- Cada ruta incluye cinco colores, materiales, acabados, tipografías, recursos gráficos y atributos de empaque.
- El color no es el único elemento de diferenciación de producto.
- No se presentan materiales sostenibles o certificaciones como hechos sin confirmación documental.

---

### Paso 5. Redactar prompts técnicos de fotografía de producto y mockup

**Objetivo:** Crear solicitudes reproducibles para generar o encargar imágenes de referencia visual.

**Instrucciones:**

1. Crea la diapositiva 6 con el título:

   ```text
   Prompts técnicos de referencia visual y mockup
   ```

2. Utiliza Copilot Chat para generar un prompt técnico por cada ruta. Usa esta estructura:

```text
Actúa como director de fotografía de producto y especialista en prompts para generación visual.

Proyecto: NOVA Hydrate.
Ruta estética: [NOMBRE DE LA RUTA].
Producto: [botella, lata u otro formato definido en la Práctica 1].
Audiencia: [audiencia definida].
Objetivo de imagen: crear una referencia visual de empaque y contexto de uso para un moodboard,
no una afirmación comercial ni una pieza final de campaña.

Define un prompt técnico que incluya:
- sujeto principal;
- forma y material del envase;
- composición;
- ángulo de cámara;
- iluminación;
- fondo y entorno;
- paleta cromática;
- textura y materiales;
- estilo fotográfico;
- espacio negativo para texto;
- nivel de realismo;
- elementos que deben excluirse;
- relación de aspecto recomendada.

Restricciones:
- No usar logotipos de terceros, marcas existentes ni personajes protegidos.
- No usar texto pequeño ilegible dentro de la imagen.
- No presentar declaraciones de salud, certificaciones ni claims no verificados.
- Evitar representaciones estereotipadas de edad, género, origen o capacidad.
- Evitar el estilo de una marca, fotógrafo o artista vivo identificable.

Devuelve:
1. un prompt principal;
2. un prompt alternativo;
3. una lista de exclusiones;
4. criterios de revisión antes de usar la imagen.
```

3. Revisa los prompts generados y conserva uno por ruta.
4. Incluye en la diapositiva 6 una versión resumida de cada prompt, identificada como:
   - `Prompt R1 — Minimalismo técnico`
   - `Prompt R2 — Naturaleza urbana`
   - `Prompt R3 — Energía cromática`
5. Copia la versión completa de los tres prompts en las notas del orador de la diapositiva o en un documento complementario dentro de:

   ```text
   /01_Prompts/
   ```

6. Si creas el documento complementario, guárdalo como:

   ```text
   02_Prompts_Moodboard_NOVA_Hydrate_v1.0.docx
   ```

7. Añade en la diapositiva una advertencia:

   ```text
   Las imágenes generadas o seleccionadas son referencias de exploración. Su uso final requiere revisión de licencias, originalidad, coherencia de marca y viabilidad de producción.
   ```

**Resultado esperado:**

- Tres prompts técnicos reutilizables y trazables.
- Cada prompt contiene contexto, restricciones y criterios de exclusión.
- Las imágenes se plantean como referencias, no como evidencia de mercado ni arte final aprobado.

**Verificación:**

- Cada prompt especifica composición, iluminación, entorno, relación de aspecto y exclusiones.
- Los prompts no solicitan imitar marcas, artistas o fotógrafos identificables.
- Los prompts evitan claims de salud y certificaciones no verificadas.

---

### Paso 6. Generar o incorporar imágenes de referencia autorizadas

**Objetivo:** Obtener referencias visuales coherentes con cada ruta y documentar su procedencia.

**Instrucciones:**

1. Determina cuál de las siguientes modalidades está disponible en tu entorno:
   - **Modalidad A:** Microsoft Designer habilitado.
   - **Modalidad B:** Biblioteca corporativa de imágenes aprobadas.
2. Si Microsoft Designer está habilitado:
   1. Abre Microsoft Designer con tu cuenta corporativa.
   2. Introduce el prompt técnico de la ruta 1.
   3. Genera varias variaciones.
   4. Selecciona una o dos imágenes que cumplan los criterios de marca.
   5. Repite el proceso para las rutas 2 y 3.
   6. Descarga o inserta las imágenes según las políticas corporativas.
   7. Guarda los recursos exportados en:

      ```text
      /02_Moodboard/
      ```

   8. Utiliza nombres trazables, por ejemplo:

      ```text
      02_ReferenciaVisual_R1_NOVA_Hydrate_v1.0.png
      02_ReferenciaVisual_R2_NOVA_Hydrate_v1.0.png
      02_ReferenciaVisual_R3_NOVA_Hydrate_v1.0.png
      ```

3. Si Microsoft Designer no está habilitado:
   1. Accede a la biblioteca corporativa de imágenes aprobadas.
   2. Busca imágenes compatibles con cada ruta mediante términos descriptivos, no mediante marcas de terceros.
   3. Selecciona imágenes con licencia o autorización clara para uso interno.
   4. Copia o registra la URL, identificador interno, autor si procede y tipo de licencia.
   5. Guarda la evidencia de procedencia en un documento dentro de:

      ```text
      /Fuentes_Verificadas/
      ```

   6. Usa el nombre:

      ```text
      02_Fuentes_Visuales_NOVA_Hydrate_v1.0.docx
      ```

4. Crea las diapositivas 7, 8 y 9:
   - Diapositiva 7: moodboard visual de `Minimalismo técnico`.
   - Diapositiva 8: moodboard visual de `Naturaleza urbana`.
   - Diapositiva 9: moodboard visual de `Energía cromática`.
5. En cada diapositiva incorpora:
   - Entre tres y seis referencias visuales.
   - La paleta cromática correspondiente.
   - Materiales o texturas.
   - Una miniatura o representación de empaque.
   - Una frase de concepto rector.
   - Una leyenda de procedencia.
6. Usa la siguiente leyenda según el caso:

   **Para imágenes generadas:**

   ```text
   Procedencia: imagen de referencia generada con Microsoft Designer el dd/MM/yyyy a partir de un prompt documentado. Uso: exploración interna.
   ```

   **Para imágenes de biblioteca autorizada:**

   ```text
   Procedencia: biblioteca corporativa aprobada. Identificador o URL: [dato]. Licencia/permiso: [dato]. Uso: exploración interna.
   ```

7. Evalúa cada imagen antes de incorporarla:
   - ¿Es coherente con la ruta?
   - ¿El envase parece físicamente plausible?
   - ¿Hay texto ilegible o marcas accidentales?
   - ¿Hay elementos visuales que puedan inducir a error?
   - ¿Representa personas o contextos de forma inclusiva?
   - ¿Se entiende como referencia y no como diseño final aprobado?

**Resultado esperado:**

- Tres moodboards visuales, uno por ruta.
- Todas las imágenes tienen procedencia documentada.
- Las imágenes son consistentes con la paleta, los materiales y el tono de cada ruta.

**Verificación:**

- Cada diapositiva contiene referencias suficientes para expresar una dirección visual.
- No se utilizan imágenes sin procedencia identificable.
- No se incorporan marcas de terceros, logotipos accidentales o claims no validados.
- La fecha de generación o consulta se registra con formato `dd/MM/yyyy`.

---

### Paso 7. Comparar las rutas mediante criterios de decisión

**Objetivo:** Aplicar convergencia creativa y seleccionar una ruta principal y una secundaria con argumentos verificables.

**Instrucciones:**

1. Crea la diapositiva 10 con el título:

   ```text
   Matriz de evaluación de rutas estéticas
   ```

2. Inserta una tabla con las siguientes columnas:

   | Criterio | Peso | Minimalismo técnico | Naturaleza urbana | Energía cromática |
   |---|---:|---:|---:|---:|

3. Utiliza los siguientes criterios y pesos:

   | Criterio | Peso |
   |---|---:|
   | Coherencia con la marca NOVA Hydrate | 25 % |
   | Adecuación al público objetivo | 20 % |
   | Diferenciación visual | 15 % |
   | Viabilidad de empaque y producción | 15 % |
   | Accesibilidad y legibilidad | 10 % |
   | Escalabilidad para sabores, formatos y canales | 10 % |
   | Riesgo de percepción | 5 % |

4. Puntúa cada ruta de 1 a 5:
   - **1:** insuficiente o alto riesgo.
   - **2:** débil; requiere cambios relevantes.
   - **3:** aceptable; requiere validación.
   - **4:** sólida; ajustes menores.
   - **5:** muy sólida; alta adecuación al criterio.
5. Calcula el resultado ponderado. Puedes realizar el cálculo manualmente o utilizar Excel como apoyo.
6. Si utilizas Excel, crea un archivo temporal de cálculo en `/03_Caso_Negocio/` o en una ubicación permitida del proyecto. No es necesario entregarlo como producto final de esta práctica salvo que el instructor lo solicite.
7. Solicita a Copilot una revisión crítica con este prompt:

```text
Actúa como revisor crítico de diseño estratégico.

A continuación se presenta una matriz de evaluación de tres rutas estéticas para NOVA Hydrate:
[pegar tabla con puntuaciones y observaciones].

Analiza la decisión sin modificar las puntuaciones arbitrariamente.
Identifica:
1. posibles sesgos en la evaluación;
2. criterios que se hayan valorado dos veces;
3. riesgos de accesibilidad, viabilidad o diferenciación;
4. datos que requieren validación externa;
5. preguntas que debería responder un equipo de negocio antes de aprobar la ruta.

No declares una ruta ganadora basándote en tendencias o supuestos de mercado no verificados.
Presenta observaciones en una lista priorizada.
```

8. Ajusta la matriz solo si puedes justificar el cambio con evidencia del brief o una observación de diseño concreta.
9. Crea la diapositiva 11 con el título:

   ```text
   Selección recomendada: ruta principal y ruta secundaria
   ```

10. Documenta:
    - Ruta principal seleccionada.
    - Ruta secundaria seleccionada.
    - Tres razones de selección.
    - Dos riesgos o aspectos por validar.
    - Próximo paso para la Práctica 3.

11. Utiliza una redacción similar a esta:

```text
Ruta principal: [nombre de la ruta].
Justificación: ofrece la mejor combinación de coherencia con NOVA Hydrate, legibilidad,
escalabilidad y diferenciación dentro de las restricciones actuales.

Ruta secundaria: [nombre de la ruta].
Justificación: conserva atributos valiosos para futuras iteraciones o segmentos específicos,
pero presenta [riesgo o limitación] que requiere validación.

Aspectos pendientes: validar percepción del público, factibilidad de acabados y diferenciación
frente a competidores mediante fuentes actuales y evidencia comercial.
```

**Resultado esperado:**

- Matriz ponderada de decisión.
- Una ruta principal y una ruta secundaria seleccionadas.
- Argumentación basada en criterios de diseño y negocio, no en preferencia personal aislada.

**Verificación:**

- La selección está conectada con los parámetros de marca de la Práctica 1.
- Los riesgos pendientes se expresan como hipótesis de validación.
- Se distinguen claramente las ideas generadas por IA de las decisiones tomadas por el participante.

---

### Paso 8. Revisar la presentación, registrar la decisión y exportar el entregable

**Objetivo:** Validar la calidad, trazabilidad y preparación del moodboard para la Práctica 3.

**Instrucciones:**

1. Revisa que la presentación contenga como mínimo las siguientes diapositivas:

   | Diapositiva | Contenido |
   |---:|---|
   | 1 | Portada y control de versión |
   | 2 | Brief visual operativo |
   | 3 | Ruta 1: Minimalismo técnico |
   | 4 | Ruta 2: Naturaleza urbana |
   | 5 | Ruta 3: Energía cromática |
   | 6 | Prompts técnicos de referencia visual y mockup |
   | 7 | Moodboard visual: Minimalismo técnico |
   | 8 | Moodboard visual: Naturaleza urbana |
   | 9 | Moodboard visual: Energía cromática |
   | 10 | Matriz de evaluación |
   | 11 | Selección de ruta principal y secundaria |

2. Revisa la ortografía y el uso consistente de español de España.
3. Comprueba que las fechas siguen el formato `dd/MM/yyyy`.
4. Comprueba que los códigos de color HEX están escritos correctamente.
5. Verifica que las diapositivas tienen contraste suficiente entre texto y fondo.
6. Ejecuta la comprobación de accesibilidad en PowerPoint:
   1. Ve a **Revisar**.
   2. Selecciona **Comprobar accesibilidad**.
   3. Corrige problemas de texto alternativo, orden de lectura, contraste o títulos de diapositiva cuando corresponda.
7. Añade texto alternativo a las imágenes esenciales:
   1. Selecciona una imagen.
   2. Haz clic con el botón derecho.
   3. Selecciona **Ver texto alternativo**.
   4. Describe la función de la imagen dentro del moodboard, no solo su apariencia.
8. Guarda la versión final de PowerPoint.
9. Exporta una copia en PDF:
   1. En PowerPoint, selecciona **Archivo** > **Exportar** > **Crear documento PDF/XPS**.
   2. Guarda el PDF en:

      ```text
      /Exportaciones_PDF/
      ```

   3. Usa el nombre:

      ```text
      02_Moodboard_NOVA_Hydrate_v1.0.pdf
      ```

10. Abre Microsoft Teams.
11. Navega al equipo `LAB-Copilot-Diseno-Desarrollo` y al canal `Proyecto-NOVA-Hydrate`.
12. Publica un mensaje breve con:
    - Enlace al archivo PowerPoint.
    - Enlace al PDF.
    - Ruta principal seleccionada.
    - Ruta secundaria seleccionada.
    - Dos elementos que se validarán en la Práctica 3.

    Ejemplo:

```text
Moodboard NOVA Hydrate completado y disponible en OneDrive:
[enlace al archivo]

Ruta principal seleccionada: [ruta].
Ruta secundaria: [ruta].

Para la Práctica 3 se validarán:
1. diferenciación frente a competidores;
2. viabilidad comercial y percepción de la audiencia.
```

**Resultado esperado:**

- Presentación final revisada, accesible y almacenada en OneDrive.
- Copia PDF exportada.
- Decisión registrada en Teams para mantener trazabilidad colaborativa.

**Verificación:**

- Existen los archivos `.pptx` y `.pdf` en las carpetas requeridas.
- Las imágenes incluyen procedencia.
- La presentación no contiene afirmaciones de mercado, competencia o sostenibilidad sin una fuente verificable.
- El canal de Teams contiene el enlace y el resumen de la decisión.

---

## Validación y pruebas

Utiliza la siguiente lista de control antes de marcar la práctica como completada.

| Área de validación | Criterio de aceptación | Estado |
|---|---|---|
| Archivo de entrada | Se utilizó `01_Guia_Prompts_NOVA_Hydrate.docx` como fuente de parámetros de marca. | ☐ |
| Almacenamiento | El PowerPoint está guardado en `/02_Moodboard/` dentro de OneDrive for Business. | ☐ |
| Convención de nombre | El archivo se llama `02_Moodboard_NOVA_Hydrate_v1.0.pptx`. | ☐ |
| Rutas creativas | Se desarrollaron Minimalismo técnico, Naturaleza urbana y Energía cromática. | ☐ |
| Descriptores | Cada ruta contiene concepto rector, descriptores e intención emocional. | ☐ |
| Paletas | Cada ruta incluye cinco colores con códigos HEX y función visual. | ☐ |
| Materialidad | Cada ruta documenta materiales, acabados y consideraciones de viabilidad. | ☐ |
| Tipografía | Cada ruta propone referencias tipográficas y criterios de legibilidad. | ☐ |
| Fotografía | Cada ruta define estilo fotográfico, composición y escenarios de uso. | ☐ |
| Empaque | Cada ruta documenta atributos de empaque y jerarquía de información. | ☐ |
| Prompts | Existen tres prompts técnicos completos, uno por ruta. | ☐ |
| Procedencia visual | Todas las imágenes incluyen leyenda de generación o fuente autorizada. | ☐ |
| Riesgos | Cada ruta identifica al menos un riesgo de percepción o viabilidad. | ☐ |
| Accesibilidad | Se evita depender solo del color; se ejecutó el comprobador de accesibilidad. | ☐ |
| Selección | Se definió una ruta principal y una secundaria mediante matriz ponderada. | ☐ |
| Trazabilidad | La decisión se publicó en el canal `Proyecto-NOVA-Hydrate`. | ☐ |
| Exportación | Existe un PDF en `/Exportaciones_PDF/`. | ☐ |

### Prueba de coherencia final

Presenta el moodboard durante dos minutos a un compañero o al instructor y responde:

1. ¿Se pueden distinguir las tres rutas sin leer todos los textos?
2. ¿La ruta principal parece coherente con el propósito y audiencia de NOVA Hydrate?
3. ¿Se entiende por qué la ruta secundaria no fue seleccionada como principal?
4. ¿Las imágenes pueden rastrearse a una generación documentada o a una fuente autorizada?
5. ¿Qué decisiones requieren investigación comercial o competitiva adicional en la Práctica 3?

Si no puedes responder alguna pregunta con evidencia de la presentación, ajusta el archivo antes de finalizar.

## Solución de problemas

### Problema 1: Copilot genera rutas demasiado parecidas o genéricas

**Síntomas:** Las tres rutas usan paletas similares, los mismos materiales, fotografías equivalentes o descripciones intercambiables como “moderno”, “fresco” y “premium”.

**Causa:** El prompt no contiene restricciones suficientes o no exige diferencias explícitas entre las rutas.

**Solución:**

1. Revisa que el prompt incluya audiencia, propósito, restricciones y riesgos.
2. Solicita una reformulación que obligue a diferenciar composición, materialidad, tono fotográfico y códigos gráficos, no solo color.
3. Indica qué elemento debe priorizar cada ruta:
   - Minimalismo técnico: estructura, precisión y claridad.
   - Naturaleza urbana: materialidad cotidiana, sostenibilidad validable y entorno urbano.
   - Energía cromática: dinamismo, modularidad y optimismo controlado.
4. Documenta en cada diapositiva una decisión visual incompatible con las otras rutas.

### Problema 2: Microsoft Designer no está disponible o las imágenes no se pueden usar

**Síntomas:** No aparece la opción de Designer, el acceso está restringido por políticas corporativas, o una imagen no tiene licencia o procedencia verificable.

**Causa:** La habilitación de Microsoft Designer depende de la licencia, configuración del tenant y políticas de seguridad; además, las imágenes externas pueden tener restricciones de uso.

**Solución:**

1. No intentes utilizar cuentas personales ni repositorios no autorizados.
2. Usa la biblioteca corporativa de imágenes aprobadas.
3. Registra para cada recurso la URL o identificador interno, fecha de consulta, licencia o permiso y finalidad de uso.
4. Guarda esta evidencia en `02_Fuentes_Visuales_NOVA_Hydrate_v1.0.docx` dentro de `/Fuentes_Verificadas/`.
5. Si no existe una imagen adecuada, utiliza bloques de color, texturas autorizadas, diagramas de composición y mockups esquemáticos; indica claramente que son referencias conceptuales.

## Limpieza

1. Confirma que la versión final del PowerPoint está guardada en:

   ```text
   /02_Moodboard/02_Moodboard_NOVA_Hydrate_v1.0.pptx
   ```

2. Confirma que el PDF está guardado en:

   ```text
   /Exportaciones_PDF/02_Moodboard_NOVA_Hydrate_v1.0.pdf
   ```

3. Mantén los prompts completos en las notas del orador o en el documento de prompts de `/01_Prompts/`.
4. Mantén la documentación de fuentes visuales dentro de `/Fuentes_Verificadas/`.
5. Elimina únicamente borradores duplicados, exportaciones fallidas o recursos no utilizados que estén fuera de la estructura corporativa.
6. No elimines:
   - El archivo de la Práctica 1.
   - Las fuentes visuales documentadas.
   - Los prompts utilizados.
   - El mensaje de decisión publicado en Teams.
7. Cierra Word, PowerPoint, Designer y Copilot Chat cuando hayas comprobado la sincronización de OneDrive.

## Resumen

En esta práctica utilizaste Microsoft 365 Copilot como apoyo para la divergencia creativa y aplicaste criterio profesional para la convergencia y selección de una propuesta. Convertiste el brief de NOVA Hydrate en tres rutas estéticas comparables, desarrollaste componentes visuales y prompts técnicos, documentaste la procedencia de referencias visuales y seleccionaste una ruta principal con una matriz de criterios.

El archivo `02_Moodboard_NOVA_Hydrate_v1.0.pptx` será la base conceptual de la Práctica 3, donde la ruta seleccionada se someterá a validación comercial, análisis competitivo y argumentación ejecutiva. Recuerda que las propuestas de Copilot y Designer son insumos de exploración: las decisiones finales requieren revisión de marca, accesibilidad, viabilidad, licencias y evidencia actualizada.

### Recursos opcionales

- [Microsoft Support: información y uso de Microsoft Copilot](https://support.microsoft.com/es-es/copilot)
- [Microsoft Learn: introducción a Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/)
- [Design Council: Double Diamond](https://www.designcouncil.org.uk/our-resources/framework-for-innovation/)
- [Nielsen Norman Group: ideación en el proceso de diseño](https://www.nngroup.com/articles/ux-ideation/)
