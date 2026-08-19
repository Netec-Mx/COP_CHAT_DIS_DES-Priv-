# Construcción del caso de negocio y la matriz competitiva que valide comercialmente el lanzamiento del diseño desarrollado.

## 1. Metadatos

| Elemento | Valor |
|---|---|
| Duración | 90 minutos |
| Complejidad | Alta |
| Nivel de Bloom | Crear |
| Modalidad | Individual con revisión colaborativa |
| Producto de trabajo | Matriz competitiva verificable en Excel y caso de negocio en Word |
| Proyecto | NOVA Hydrate |
| Equipo de Teams | `LAB-Copilot-Diseno-Desarrollo` |
| Canal de trabajo | `Proyecto-NOVA-Hydrate` |

## 2. Descripción general

En esta práctica transformarás la investigación, la guía de prompts de la Práctica 1 y el concepto visual seleccionado en la Práctica 2 en dos entregables comerciales trazables: una matriz competitiva verificable y un caso de negocio ejecutivo para NOVA Hydrate.

Utilizarás Microsoft Excel con Copilot para estructurar datos competitivos, calcular puntuaciones comparativas, detectar brechas y generar gráficos. Después, utilizarás Word con Copilot para documentar una recomendación comercial que conecte necesidades de usuario, tendencias, propuesta visual, viabilidad y riesgos de lanzamiento.

> **Principio de calidad:** Copilot puede ayudar a estructurar, sintetizar y analizar información, pero no sustituye la verificación humana. Todo dato comercial, precio, especificación o tendencia debe identificarse como **verificado**, **inferido** o **pendiente de validación**.

## 3. Objetivos de aprendizaje

Al finalizar la práctica, podrás:

- [ ] Registrar y normalizar información verificable de al menos cinco competidores relevantes para NOVA Hydrate.
- [ ] Construir una matriz competitiva en Excel con atributos, puntuaciones, fórmulas, filtros y visualizaciones ejecutivas.
- [ ] Distinguir claramente entre hallazgos validados, hipótesis comerciales e inferencias derivadas del análisis.
- [ ] Identificar una oportunidad de posicionamiento para NOVA Hydrate a partir de brechas competitivas documentadas.
- [ ] Redactar un caso de negocio que conecte deseabilidad, factibilidad y viabilidad comercial con el concepto visual seleccionado.

## 4. Requisitos previos

### Conocimientos requeridos

Debes haber completado o tener disponibles los siguientes elementos:

- La guía de prompting corporativo elaborada en la Práctica 1.
- La ficha del concepto visual seleccionado durante la Práctica 2.
- Conocimiento intermedio de tablas estructuradas de Excel, filtros, fórmulas y gráficos.
- Capacidad para distinguir entre una hipótesis y un hallazgo respaldado por evidencia.
- Conocimiento básico de fuentes públicas de productos, tiendas oficiales, distribuidores autorizados y repositorios corporativos.

### Acceso requerido

- Cuenta corporativa del tenant `contoso.onmicrosoft.com`, o cuenta invitada autorizada.
- Acceso de edición a la biblioteca de OneDrive for Business del proyecto.
- Microsoft Excel, Word y Microsoft 365 Copilot habilitados.
- Acceso a Internet para consultar fuentes públicas autorizadas.
- Acceso al equipo de Teams `LAB-Copilot-Diseno-Desarrollo` y al canal `Proyecto-NOVA-Hydrate`.

## 5. Entorno de laboratorio

### Configuración técnica de referencia

| Componente | Requisito o versión de referencia |
|---|---|
| Sistema operativo | Windows 11 Enterprise 24H2 |
| Memoria | 16 GB mínimo; 32 GB recomendados |
| Almacenamiento | 20 GB libres en SSD |
| Red | 25 Mbps de descarga y 5 Mbps de carga como mínimo |
| Microsoft 365 Apps | Versión 2508, Canal actual |
| Excel y Word | Microsoft 365 Apps for enterprise con Copilot |
| Navegador recomendado | Microsoft Edge 139 o posterior |
| Región | Español (España) |
| Zona horaria | Europe/Madrid |
| Fecha | `dd/MM/yyyy` |
| Moneda | EUR (`€`) |
| Separador decimal | Coma |

### Ruta obligatoria del proyecto

Trabaja exclusivamente en la siguiente ubicación de OneDrive for Business:

```text
/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
```

Verifica que exista esta estructura:

```text
/CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
├── 01_Prompts/
├── 02_Moodboard/
├── 03_Caso_Negocio/
├── 04_Expediente_Final/
├── Fuentes_Verificadas/
└── Exportaciones_PDF/
```

### Convención de nombres

Utiliza la siguiente convención para versiones finales:

```text
NN_TipoEntregable_NOVA_Hydrate_vMAJOR.MINOR.ext
```

En esta práctica, los archivos finales serán:

```text
03_Matriz_Competitiva_NOVA_Hydrate_v1.0.xlsx
03_Caso_de_Negocio_NOVA_Hydrate_v1.0.docx
```

Los nombres base solicitados por el proyecto son `03_Matriz_Competitiva_NOVA_Hydrate.xlsx` y `03_Caso_de_Negocio_NOVA_Hydrate.docx`; aplica la versión `v1.0` al guardar el entregable validado.

---

## 6. Procedimiento paso a paso

### Paso 1. Preparar el espacio de trabajo y revisar las entradas

**Objetivo:** Confirmar que dispones de los insumos de las prácticas anteriores y preparar una estructura trazable para la evidencia comercial.

**Instrucciones:**

1. Abre OneDrive for Business y navega a:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/
   ```

2. Comprueba que las carpetas obligatorias están disponibles. Si alguna no existe, créala respetando exactamente el nombre definido.

3. En la carpeta `01_Prompts/`, localiza la guía de prompts creada en la Práctica 1.

4. En la carpeta `02_Moodboard/`, localiza la ficha de concepto visual seleccionado en la Práctica 2.

5. Lee la ficha de concepto y anota, en un documento temporal o nota de trabajo, los siguientes elementos:
   - Nombre o denominación del concepto seleccionado.
   - Público objetivo definido.
   - Problema de uso que busca resolver.
   - Atributos visuales y funcionales destacados.
   - Materiales, formato, paleta, acabados o mensajes visuales relevantes.
   - Restricciones identificadas durante la práctica anterior.

6. En `Fuentes_Verificadas/`, crea un archivo de texto o documento breve denominado:

   ```text
   03_Registro_de_Fuentes_NOVA_Hydrate_v1.0.docx
   ```

7. Crea una tabla inicial con estas columnas:

   | ID fuente | Competidor o tema | URL | Tipo de fuente | Fecha de consulta | Dato verificado | Estado |
   |---|---|---|---|---|---|---|

8. Usa únicamente fuentes autorizadas. Prioriza, en este orden:
   1. Sitio web oficial de la marca.
   2. Ficha oficial del producto.
   3. Tienda oficial o distribuidor autorizado.
   4. Informe corporativo, asociación sectorial o estudio de mercado con autor identificable.
   5. Fuente editorial especializada con fecha y metodología visibles.

9. Evita usar contenido sin autor, publicaciones no verificables en redes sociales o resúmenes generados por IA como evidencia final.

**Salida esperada:**

- Estructura de carpetas validada.
- Guía de prompts y ficha de concepto disponibles.
- Registro inicial de fuentes creado en `Fuentes_Verificadas/`.

**Verificación:**

- La ruta de trabajo no corresponde a Escritorio, Descargas ni una unidad local no administrada.
- Puedes abrir la guía de prompts y la ficha visual desde OneDrive.
- El registro de fuentes contiene al menos una fila preparada para cada competidor que investigarás.

---

### Paso 2. Definir el marco de investigación y las variables competitivas

**Objetivo:** Traducir el concepto visual NOVA Hydrate en preguntas de negocio, hipótesis y variables comparables.

**Instrucciones:**

1. Abre Microsoft 365 Copilot Chat con tu cuenta corporativa.

2. Adjunta o referencia la guía de prompts de la Práctica 1 y la ficha de concepto visual de la Práctica 2, si los permisos lo permiten.

3. Utiliza el siguiente prompt parametrizado. Sustituye los campos entre corchetes con información real de tu concepto:

   ```text
   Actúa como asistente de investigación de diseño y estrategia comercial.

   Contexto:
   - Marca/propuesta: NOVA Hydrate.
   - Categoría de producto: [por ejemplo, botella térmica reutilizable / sistema de hidratación portátil].
   - Concepto visual seleccionado: [nombre o descripción breve].
   - Audiencia principal: [perfil definido en la Práctica 2].
   - Contexto de uso: [movilidad, oficina, deporte, desplazamientos, etc.].
   - Decisión que se debe apoyar: definir una propuesta de posicionamiento y una hipótesis inicial de lanzamiento.

   A partir exclusivamente de la información proporcionada:
   1. Formula cinco hipótesis comerciales que requieran validación.
   2. Propón cinco criterios comparables para analizar competidores directos.
   3. Separa los elementos en: hallazgos confirmados, inferencias y pendientes de validar.
   4. Sugiere preguntas de investigación para comprobar deseabilidad, factibilidad y viabilidad.
   5. No inventes precios, tendencias, cuotas de mercado ni especificaciones.
   6. Entrega el resultado en una tabla.
   ```

4. Revisa críticamente la salida. No copies afirmaciones de Copilot como hechos si no están respaldadas por fuentes.

5. Crea una lista de criterios mínimos para la matriz competitiva. Incluye obligatoriamente:
   - Competidor y producto.
   - Precio en EUR.
   - Capacidad.
   - Material principal.
   - Tiempo de conservación térmica.
   - Canal de venta.
   - Posicionamiento.
   - Atributos de sostenibilidad.
   - Valoración pública.
   - Fortaleza.
   - Debilidad.
   - Fuente y fecha de consulta.
   - Estado de evidencia.

6. Define los criterios de puntuación que utilizarás. Emplea una escala de 1 a 5, donde:
   - `1` = desempeño bajo o ausencia del atributo.
   - `3` = desempeño medio o atributo parcialmente presente.
   - `5` = desempeño alto o atributo claramente diferenciado.

7. Establece estas dimensiones de puntuación para todos los competidores:
   - Desempeño térmico.
   - Relación capacidad/precio.
   - Sostenibilidad comunicada.
   - Disponibilidad de canal.
   - Valoración pública.
   - Diferenciación percibida.

8. Documenta las hipótesis aprobadas en el registro de fuentes o en una sección titulada **Hipótesis de trabajo**.

**Salida esperada:**

- Marco de investigación con hipótesis explícitas.
- Criterios competitivos normalizados.
- Distinción entre evidencia, inferencia e hipótesis.

**Verificación:**

- Cada hipótesis está redactada como una afirmación que puede comprobarse.
- Ninguna hipótesis se presenta como un hallazgo validado.
- Los criterios elegidos se relacionan con decisiones de producto, posicionamiento, canal o precio.

---

### Paso 3. Crear y estructurar la matriz competitiva en Excel

**Objetivo:** Construir un libro de Excel trazable, normalizado y preparado para análisis con Copilot.

**Instrucciones:**

1. Abre Microsoft Excel.

2. Crea un libro nuevo y guárdalo inicialmente en:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/03_Caso_Negocio/
   ```

   Con el nombre:

   ```text
   03_Matriz_Competitiva_NOVA_Hydrate_v1.0.xlsx
   ```

3. Crea las siguientes hojas de cálculo:
   - `Matriz_Competitiva`
   - `Criterios_y_Pesos`
   - `Fuentes`
   - `Hallazgos`
   - `Graficos`

4. En la hoja `Matriz_Competitiva`, crea una tabla con los siguientes encabezados:

   | ID | Competidor | Producto | URL producto | Precio EUR | Capacidad ml | Material | Conservación fría h | Conservación caliente h | Canal principal | Posicionamiento | Sostenibilidad | Valoración pública | Nº reseñas | Fortaleza | Debilidad | Fuente ID | Fecha consulta | Estado evidencia | Térmico 1-5 | Capacidad/Precio 1-5 | Sostenibilidad 1-5 | Canal 1-5 | Valoración 1-5 | Diferenciación 1-5 | Puntuación total |
   |---|---|---|---|---:|---:|---|---:|---:|---|---|---|---:|---:|---|---|---|---|---|---:|---:|---:|---:|---:|---:|---:|

5. Selecciona la tabla y conviértela en una tabla estructurada mediante **Insertar > Tabla**. Marca la opción **La tabla tiene encabezados**.

6. En la pestaña **Diseño de tabla**, asigna el nombre:

   ```text
   tblCompetidores
   ```

7. Aplica formatos:
   - `Precio EUR`: moneda EUR con dos decimales.
   - `Capacidad ml`, horas y número de reseñas: número sin decimales.
   - `Valoración pública`: número con un decimal.
   - `Fecha consulta`: formato `dd/MM/yyyy`.
   - Puntuaciones: número entero entre 1 y 5.

8. En la hoja `Criterios_y_Pesos`, crea esta tabla:

   | Criterio | Peso |
   |---|---:|
   | Desempeño térmico | 0,20 |
   | Relación capacidad/precio | 0,20 |
   | Sostenibilidad comunicada | 0,15 |
   | Disponibilidad de canal | 0,15 |
   | Valoración pública | 0,15 |
   | Diferenciación percibida | 0,15 |

9. Comprueba que la suma de los pesos sea `1,00`. Añade una celda de control con la fórmula:

   ```excel
   =SUMA(B2:B7)
   ```

10. En la columna `Puntuación total` de `tblCompetidores`, utiliza una fórmula ponderada. Si los valores de puntuación están en las columnas correspondientes, usa una fórmula equivalente a la siguiente:

   ```excel
   =[@[Térmico 1-5]]*0,20+[@[Capacidad/Precio 1-5]]*0,20+[@[Sostenibilidad 1-5]]*0,15+[@[Canal 1-5]]*0,15+[@[Valoración 1-5]]*0,15+[@[Diferenciación 1-5]]*0,15
   ```

11. Si deseas consultar los pesos desde la hoja de criterios, emplea referencias absolutas o una búsqueda estructurada. Por ejemplo:

   ```excel
   =[@[Térmico 1-5]]*Criterios_y_Pesos!$B$2+
   [@[Capacidad/Precio 1-5]]*Criterios_y_Pesos!$B$3+
   [@[Sostenibilidad 1-5]]*Criterios_y_Pesos!$B$4+
   [@[Canal 1-5]]*Criterios_y_Pesos!$B$5+
   [@[Valoración 1-5]]*Criterios_y_Pesos!$B$6+
   [@[Diferenciación 1-5]]*Criterios_y_Pesos!$B$7
   ```

12. En la hoja `Fuentes`, crea una tabla denominada `tblFuentes` con estas columnas:

   | Fuente ID | Competidor | URL | Tipo de fuente | Fecha de consulta | Dato o evidencia extraída | Verificado por | Observaciones |
   |---|---|---|---|---|---|---|---|

13. En la hoja `Hallazgos`, reserva secciones para:
   - Hallazgos validados.
   - Hipótesis por validar.
   - Brechas competitivas.
   - Riesgos comerciales.
   - Implicaciones para NOVA Hydrate.

**Salida esperada:**

- Libro de Excel con cinco hojas estructuradas.
- Tabla `tblCompetidores` creada y preparada para el análisis.
- Fórmula de puntuación ponderada funcional.
- Tabla de fuentes independiente y trazable.

**Verificación:**

- La tabla contiene todos los campos obligatorios del alcance de la práctica.
- La suma de pesos es exactamente `1,00`.
- La fórmula de puntuación total se replica automáticamente al añadir filas nuevas.
- El archivo está guardado en OneDrive for Business.

---

### Paso 4. Investigar y registrar al menos cinco competidores verificables

**Objetivo:** Recopilar evidencia comercial comparable sin inventar datos ni mezclar fuentes no verificadas.

**Instrucciones:**

1. Identifica al menos cinco competidores de referencia. Incluye, cuando sea posible:
   - Competidores directos de la misma categoría.
   - Una marca premium.
   - Una alternativa de precio accesible.
   - Una alternativa centrada en sostenibilidad.
   - Una alternativa de canal masivo, deportivo, oficina o movilidad, según la audiencia de NOVA Hydrate.

2. Para cada competidor, consulta como mínimo una fuente oficial. Registra:
   - Nombre de marca y producto.
   - Precio observado.
   - Capacidad.
   - Material.
   - Declaración de conservación térmica, si existe.
   - Canal de compra.
   - Mensaje de posicionamiento.
   - Atributos de sostenibilidad declarados.
   - Valoración pública y número de reseñas, indicando la plataforma.
   - URL y fecha de consulta.

3. Copia la URL exacta en la columna `URL producto` y registra un identificador de fuente, por ejemplo:

   ```text
   F-01
   F-02
   F-03
   ```

4. En la hoja `Fuentes`, crea la entrada correspondiente para cada identificador.

5. Clasifica el valor de `Estado evidencia` con una de estas opciones:
   - `Verificado`: dato localizado en fuente oficial o fuente autorizada.
   - `Parcialmente verificado`: dato disponible, pero requiere contraste adicional.
   - `Pendiente de validar`: afirmación sin evidencia suficiente.
   - `No disponible`: la fuente no publica el dato.

6. No rellenes con valores estimados los campos de precio, conservación térmica, capacidad, valoración o reseñas. Si el dato no se publica, escribe:

   ```text
   No disponible
   ```

   o deja la celda vacía cuando sea necesario para evitar errores de cálculo.

7. Para puntuar un atributo cualitativo, documenta el criterio en una nota o comentario. Por ejemplo:

   ```text
   Sostenibilidad 5: material reciclado certificado, piezas reemplazables y programa de reparación documentado.
   Sostenibilidad 3: botella reutilizable con comunicación ambiental genérica.
   Sostenibilidad 1: no se publica información de sostenibilidad.
   ```

8. Registra una fortaleza y una debilidad por competidor. Redáctalas de forma observable y no promocional.

   Ejemplos correctos:
   - “La ficha oficial declara 24 horas de conservación en frío.”
   - “No se publica información sobre disponibilidad de repuestos.”
   - “El precio observado es superior a la media de la muestra.”

   Ejemplos incorrectos:
   - “Es la mejor botella del mercado.”
   - “Tiene calidad excelente.”
   - “Los clientes la aman.”

9. Añade al menos cinco filas completas a `tblCompetidores`.

**Salida esperada:**

- Cinco o más competidores registrados.
- Todas las filas incluyen fuente, fecha de consulta y estado de evidencia.
- Las puntuaciones se basan en criterios documentados.

**Verificación:**

- Filtra la columna `Estado evidencia` y comprueba que no existen filas sin clasificación.
- Abre aleatoriamente dos URL registradas y confirma que el dato clave corresponde a lo anotado.
- Comprueba que cada competidor tiene al menos una fortaleza, una debilidad y una fuente identificable.

---

### Paso 5. Analizar la matriz con Excel y Copilot

**Objetivo:** Identificar brechas, patrones y oportunidades de posicionamiento para NOVA Hydrate.

**Instrucciones:**

1. Selecciona una celda dentro de `tblCompetidores`.

2. Abre Copilot en Excel.

3. Utiliza el siguiente prompt:

   ```text
   Analiza la tabla tblCompetidores como una matriz competitiva para NOVA Hydrate.

   Requisitos:
   - Distingue datos verificados de datos pendientes de validar.
   - Identifica patrones de precio, capacidad, desempeño térmico, sostenibilidad, canales y valoración pública.
   - Detecta tres brechas de mercado potenciales.
   - No afirmes que una brecha es una oportunidad validada si los datos solo permiten inferirla.
   - Indica qué datos faltan antes de recomendar una decisión de lanzamiento.
   - Devuelve una tabla con: hallazgo, evidencia de la tabla, nivel de confianza, implicación para NOVA Hydrate y acción siguiente.
   ```

4. Revisa el análisis de Copilot. Corrige interpretaciones que no se sostengan con los datos de la tabla.

5. En la hoja `Hallazgos`, copia únicamente conclusiones que puedas justificar con la matriz. Clasifica cada registro con uno de estos estados:
   - `Hallazgo validado por la muestra`.
   - `Inferencia basada en la muestra`.
   - `Hipótesis que requiere validación primaria`.

6. Calcula indicadores de referencia en la hoja `Hallazgos`. Por ejemplo:

   **Precio medio:**

   ```excel
   =PROMEDIO(tblCompetidores[Precio EUR])
   ```

   **Capacidad media:**

   ```excel
   =PROMEDIO(tblCompetidores[Capacidad ml])
   ```

   **Puntuación competitiva máxima:**

   ```excel
   =MAX(tblCompetidores[Puntuación total])
   ```

   **Número de competidores con sostenibilidad alta:**

   ```excel
   =CONTAR.SI(tblCompetidores[Sostenibilidad 1-5];">=4")
   ```

7. Si existen celdas vacías que afectan a los cálculos, utiliza fórmulas de control, por ejemplo:

   ```excel
   =SI.ERROR(PROMEDIO(tblCompetidores[Precio EUR]);"Sin datos suficientes")
   ```

8. Crea dos gráficos aptos para comité ejecutivo:

   **Gráfico 1: Precio frente a capacidad**
   - Selecciona las columnas `Competidor`, `Precio EUR` y `Capacidad ml`.
   - Inserta un gráfico de dispersión o de columnas, según la calidad de los datos.
   - Título recomendado:

     ```text
     Comparativa de precio y capacidad — NOVA Hydrate
     ```

   **Gráfico 2: Puntuación competitiva total**
   - Selecciona `Competidor` y `Puntuación total`.
   - Inserta un gráfico de barras horizontales.
   - Ordena la tabla de mayor a menor puntuación antes de crear el gráfico.
   - Título recomendado:

     ```text
     Posición competitiva ponderada de la muestra
     ```

9. Mueve ambos gráficos a la hoja `Graficos`.

10. Añade debajo de cada gráfico una nota breve con:
    - Fuente de los datos.
    - Fecha de consulta.
    - Limitación principal de la comparación.

    Ejemplo:

    ```text
    Fuente: tblCompetidores y tblFuentes. Consulta realizada el dd/MM/yyyy.
    Limitación: la muestra no representa la cuota de mercado ni incluye datos de coste interno.
    ```

**Salida esperada:**

- Hoja `Hallazgos` con conclusiones trazables.
- Dos gráficos comparativos comprensibles.
- Brechas diferenciadas de hechos validados.

**Verificación:**

- Cada hallazgo puede vincularse a una fila, dato o cálculo de la matriz.
- Los gráficos incluyen títulos, ejes comprensibles y no presentan valores sin fuente.
- El análisis no confunde una correlación o diferencia observada con una validación de demanda.

---

### Paso 6. Elaborar la propuesta comercial y la recomendación de lanzamiento

**Objetivo:** Convertir la evidencia competitiva y visual en una propuesta de valor comercial coherente.

**Instrucciones:**

1. Revisa la ficha de concepto de la Práctica 2 junto con la hoja `Hallazgos`.

2. Redacta una propuesta de valor preliminar utilizando esta estructura:

   ```text
   Para [audiencia específica] que necesita [necesidad o problema],
   NOVA Hydrate ofrece [producto o solución] que permite [beneficio principal]
   mediante [diferenciador funcional, visual o de servicio],
   a diferencia de [alternativas actuales], que [limitación identificada].
   ```

3. No declares como hecho aquello que todavía no está validado. Cuando corresponda, utiliza expresiones como:
   - “Se propone validar si…”
   - “La muestra sugiere que…”
   - “La hipótesis de lanzamiento plantea…”
   - “La evidencia disponible indica…”

4. Utiliza Copilot Chat con el siguiente prompt:

   ```text
   Actúa como estratega de producto.

   Usa exclusivamente los hallazgos verificados y las hipótesis identificadas en esta matriz competitiva de NOVA Hydrate.

   Genera:
   1. Una propuesta de valor de máximo 70 palabras.
   2. Tres diferenciadores defendibles, indicando la evidencia disponible para cada uno.
   3. Tres riesgos comerciales.
   4. Cinco indicadores iniciales para validar un lanzamiento piloto.
   5. Una recomendación: avanzar, avanzar con condiciones o no avanzar todavía.

   Reglas:
   - Separa explícitamente hallazgos, inferencias e hipótesis.
   - No inventes tamaños de mercado, márgenes, costes, intención de compra ni datos de usuarios.
   - Si falta evidencia, indica la validación necesaria.
   ```

5. Revisa la salida y conserva únicamente formulaciones consistentes con los datos recopilados.

6. Define los indicadores iniciales de lanzamiento. Incluye, como mínimo:
   - Tasa de conversión de una página de interés o preventa.
   - Intención de compra declarada en prueba de concepto.
   - Rango de precio aceptado.
   - Tasa de repetición o uso semanal en piloto.
   - Incidencias de uso relacionadas con cierre, limpieza, transporte o conservación térmica.
   - Porcentaje de devoluciones o reclamaciones, si aplica.

7. Registra la recomendación final en la hoja `Hallazgos` con una de estas opciones:
   - `Avanzar a validación piloto`.
   - `Avanzar con condiciones de validación`.
   - `No avanzar hasta completar evidencia crítica`.

**Salida esperada:**

- Propuesta de valor trazable.
- Diferenciadores vinculados al concepto y a la matriz.
- Riesgos e indicadores iniciales definidos.
- Recomendación comercial provisional.

**Verificación:**

- La recomendación menciona condiciones o evidencia necesaria.
- Los diferenciadores no son únicamente adjetivos visuales; describen valor para la audiencia.
- Los indicadores pueden medirse durante una prueba piloto o una fase de validación.

---

### Paso 7. Crear el caso de negocio en Word

**Objetivo:** Documentar una argumentación comercial ejecutiva y trazable para NOVA Hydrate.

**Instrucciones:**

1. Abre Microsoft Word.

2. Crea un documento nuevo y guárdalo en:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/03_Caso_Negocio/
   ```

   Con el nombre:

   ```text
   03_Caso_de_Negocio_NOVA_Hydrate_v1.0.docx
   ```

3. Aplica el idioma de revisión **Español (España)** y revisa que las fechas usen el formato `dd/MM/yyyy`.

4. Inserta una portada con:
   - Título: `Caso de negocio — NOVA Hydrate`.
   - Subtítulo: `Validación comercial del concepto de diseño`.
   - Versión: `v1.0`.
   - Fecha.
   - Autor o equipo.
   - Referencia al proyecto y canal de Teams.

5. Estructura el documento con los siguientes encabezados:

   ```text
   1. Resumen ejecutivo
   2. Problema y necesidad de usuario
   3. Oportunidad de mercado
   4. Audiencia prioritaria
   5. Tendencias y evidencia verificada
   6. Propuesta de valor de NOVA Hydrate
   7. Diferenciadores del diseño seleccionado
   8. Análisis competitivo y brechas
   9. Hipótesis de lanzamiento
   10. Riesgos y medidas de mitigación
   11. Indicadores iniciales de validación
   12. Recomendación ejecutiva
   13. Fuentes y trazabilidad
   ```

6. En la sección **Resumen ejecutivo**, redacta entre 120 y 180 palabras que respondan:
   - Qué problema busca resolver NOVA Hydrate.
   - Para quién.
   - Qué evidencia competitiva respalda la oportunidad.
   - Qué debe validarse antes de un lanzamiento amplio.
   - Qué recomendación se propone.

7. En la sección **Problema y necesidad de usuario**, diferencia claramente:
   - Necesidades confirmadas por evidencia previa.
   - Necesidades inferidas.
   - Preguntas pendientes de investigación primaria.

8. En la sección **Oportunidad de mercado**, incorpora una tabla como la siguiente:

   | Dimensión | Evidencia disponible | Interpretación | Estado |
   |---|---|---|---|
   | Deseabilidad | [evidencia] | [implicación] | Verificado / Inferencia / Pendiente |
   | Factibilidad | [evidencia] | [implicación] | Verificado / Inferencia / Pendiente |
   | Viabilidad | [evidencia] | [implicación] | Verificado / Inferencia / Pendiente |

9. En la sección **Tendencias y evidencia verificada**, incorpora únicamente tendencias con fuente, fecha y relación explícita con NOVA Hydrate. No uses frases generales como “la sostenibilidad está creciendo” sin fuente verificable.

10. En **Análisis competitivo y brechas**, inserta:
    - Una tabla resumida de los cinco competidores.
    - El gráfico de puntuación competitiva desde Excel.
    - El gráfico de precio y capacidad, si resulta legible.
    - Una nota que indique las limitaciones de la muestra.

11. En **Hipótesis de lanzamiento**, redacta de tres a cinco hipótesis. Ejemplo de estructura:

    ```text
    Hipótesis H-01: [audiencia] considerará relevante [beneficio] si NOVA Hydrate demuestra [condición].
    Método de validación: [entrevista, landing page, prueba de uso, preventa, etc.].
    Indicador de confirmación: [métrica o umbral].
    Estado: Pendiente de validación.
    ```

12. En **Riesgos y medidas de mitigación**, incluye al menos tres riesgos de naturaleza diferente:
    - Riesgo de mercado.
    - Riesgo de producto o factibilidad.
    - Riesgo de posicionamiento, precio, canal o comunicación.

13. En **Fuentes y trazabilidad**, cita:
    - El archivo de matriz competitiva.
    - El registro de fuentes.
    - La ficha de concepto visual.
    - La guía de prompts.
    - Las URL principales, fecha de consulta y tipo de evidencia.

14. Usa Copilot en Word para revisar claridad y consistencia, con este prompt:

    ```text
    Revisa este caso de negocio de NOVA Hydrate para un comité ejecutivo.

    Comprueba:
    - coherencia entre problema, audiencia, evidencia, propuesta de valor y recomendación;
    - separación entre hallazgos verificados, inferencias e hipótesis;
    - ausencia de afirmaciones comerciales sin fuente;
    - claridad de riesgos, indicadores y acciones siguientes.

    Devuelve:
    1. inconsistencias detectadas;
    2. afirmaciones que requieren fuente o reformulación;
    3. sugerencias de mejora concretas;
    4. una lista de comprobación final.
    No inventes datos ni reescribas las conclusiones como hechos si son hipótesis.
    ```

15. Aplica solo las correcciones que puedas justificar.

**Salida esperada:**

- Documento Word con estructura ejecutiva completa.
- Gráficos y tabla competitiva integrados.
- Trazabilidad entre evidencia, hipótesis, riesgos e indicadores.

**Verificación:**

- El documento contiene las 13 secciones indicadas.
- Toda cifra, precio, especificación o tendencia tiene fuente o se identifica como hipótesis.
- La recomendación ejecutiva es coherente con las limitaciones de la evidencia.

---

### Paso 8. Revisar, exportar y comunicar los entregables

**Objetivo:** Completar la validación de calidad, generar copias en PDF y comunicar la disponibilidad del material al equipo.

**Instrucciones:**

1. Guarda ambos documentos y confirma que OneDrive muestra el estado de sincronización correcto.

2. En Excel, revisa:
   - Filtros activos.
   - Fórmulas sin errores.
   - Fechas y moneda en formato regional correcto.
   - Gráficos actualizados.
   - Fuentes identificables.

3. En Word, ejecuta:
   - **Revisar > Editor** para comprobar ortografía y claridad.
   - **Archivo > Información** para verificar propiedades básicas del documento.
   - Comprobación visual de títulos, tablas, gráficos y referencias.

4. Exporta el libro Excel a PDF:

   ```text
   03_Matriz_Competitiva_NOVA_Hydrate_v1.0.pdf
   ```

5. Exporta el caso de negocio a PDF:

   ```text
   03_Caso_de_Negocio_NOVA_Hydrate_v1.0.pdf
   ```

6. Guarda ambos PDF en:

   ```text
   /CopilotLabs/Curso_Copilot_Diseno_Desarrollo/NOVA_Hydrate/Exportaciones_PDF/
   ```

7. Publica un mensaje en el canal de Teams `Proyecto-NOVA-Hydrate` con el siguiente formato:

   ```text
   Práctica 3 completada — NOVA Hydrate

   Entregables disponibles:
   - 03_Matriz_Competitiva_NOVA_Hydrate_v1.0.xlsx
   - 03_Caso_de_Negocio_NOVA_Hydrate_v1.0.docx
   - Exportaciones PDF correspondientes

   Estado de recomendación: [Avanzar / Avanzar con condiciones / No avanzar todavía].
   Evidencia crítica pendiente: [resumen breve].
   ```

8. No adjuntes copias locales si los archivos ya están disponibles en OneDrive. Comparte enlaces corporativos a los entregables.

**Salida esperada:**

- Archivos Excel, Word y PDF disponibles en las ubicaciones obligatorias.
- Mensaje de disponibilidad publicado en Teams.
- Recomendación y evidencia pendiente comunicadas al equipo.

**Verificación:**

- Los archivos se abren desde OneDrive.
- Los PDF muestran correctamente las tablas y gráficos.
- El mensaje de Teams contiene enlaces o referencias claras a los entregables.

---

## 7. Validación y pruebas

Completa la siguiente lista antes de considerar terminada la práctica.

### Validación de la matriz competitiva

- [ ] El archivo se llama `03_Matriz_Competitiva_NOVA_Hydrate_v1.0.xlsx`.
- [ ] El archivo está almacenado en `03_Caso_Negocio/` dentro de OneDrive corporativo.
- [ ] La matriz contiene al menos cinco competidores.
- [ ] Cada competidor tiene precio, capacidad, material, canal, posicionamiento, sostenibilidad, valoración, fortaleza, debilidad y fuente, o bien indica explícitamente `No disponible`.
- [ ] La tabla está estructurada y se denomina `tblCompetidores`.
- [ ] Cada registro incluye fecha de consulta y estado de evidencia.
- [ ] Las puntuaciones utilizan criterios definidos y una escala consistente de 1 a 5.
- [ ] La suma de los pesos es `1,00`.
- [ ] La puntuación total se calcula sin errores.
- [ ] Se han creado dos gráficos comparativos aptos para revisión ejecutiva.
- [ ] Las conclusiones no presentan hipótesis como hechos.

### Validación del caso de negocio

- [ ] El archivo se llama `03_Caso_de_Negocio_NOVA_Hydrate_v1.0.docx`.
- [ ] El documento incluye las 13 secciones solicitadas.
- [ ] El resumen ejecutivo explica problema, audiencia, oportunidad, condición de validación y recomendación.
- [ ] La propuesta de valor se relaciona con el concepto visual seleccionado.
- [ ] Los diferenciadores se apoyan en evidencia o se identifican como hipótesis.
- [ ] Los riesgos incluyen medidas de mitigación.
- [ ] Los indicadores iniciales son medibles.
- [ ] El documento identifica las limitaciones de la muestra competitiva.
- [ ] Las fuentes y fechas de consulta están documentadas.
- [ ] Los gráficos de Excel se visualizan correctamente en Word.

### Prueba de trazabilidad

Selecciona al azar un competidor y comprueba esta cadena:

```text
Dato en Word
→ dato o gráfico en Excel
→ fila de tblCompetidores
→ identificador de fuente
→ URL y fecha de consulta en tblFuentes o Registro de fuentes
```

La práctica cumple el requisito de trazabilidad si puedes completar esta cadena sin depender de memoria, mensajes informales o archivos locales.

---

## 8. Resolución de problemas

### Problema 1: Copilot genera conclusiones con cifras o tendencias que no aparecen en la matriz

**Síntomas:**
- Copilot menciona cuotas de mercado, precios medios, preferencias de consumidores o tendencias sin que esos datos existan en el libro.
- El análisis parece convincente, pero no puedes localizar el origen de la afirmación.

**Causa:**
Copilot puede complementar una respuesta con inferencias generales o información no incluida explícitamente en la tabla. Esto no constituye evidencia verificable para el caso de negocio.

**Solución:**
1. Elimina o reformula la afirmación no sustentada.
2. Solicita un nuevo análisis indicando: “Usa exclusivamente las columnas y filas de `tblCompetidores`; no utilices conocimiento externo”.
3. Añade una fuente externa autorizada si necesitas respaldar la afirmación.
4. Clasifica el resultado como `Hipótesis` o `Inferencia` si no existe evidencia suficiente.
5. Actualiza la sección de fuentes antes de incluir la conclusión en Word.

### Problema 2: Las fórmulas muestran errores o los valores de precio no se calculan correctamente

**Síntomas:**
- Aparecen errores como `#¿NOMBRE?`, `#¡VALOR!` o resultados vacíos.
- Los precios se interpretan como texto.
- La fórmula de puntuación total no se replica en todas las filas.

**Causa:**
La configuración regional Español (España) utiliza coma como separador decimal y punto y coma como separador de argumentos. Además, algunos precios pueden haberse pegado con símbolos, espacios o formatos de texto.

**Solución:**
1. Verifica que la configuración regional de Excel sea Español (España).
2. Convierte la columna `Precio EUR` a formato Número o Moneda.
3. Elimina símbolos no numéricos, como texto adicional o espacios, antes de introducir el precio.
4. Revisa que las fórmulas utilicen coma decimal, por ejemplo `0,20`.
5. Si usas funciones con argumentos, utiliza punto y coma:

   ```excel
   =SI.ERROR(PROMEDIO(tblCompetidores[Precio EUR]);"Sin datos suficientes")
   ```

6. Confirma que la fórmula se ha escrito dentro de la tabla estructurada `tblCompetidores`; Excel deberá replicarla automáticamente en las filas existentes y nuevas.

---

## 9. Limpieza

1. Cierra las pestañas de navegación que contengan fuentes ya registradas, excepto aquellas necesarias para una revisión posterior autorizada.
2. Elimina documentos temporales, capturas duplicadas y descargas locales que no formen parte de la evidencia aprobada.
3. Conserva únicamente los archivos de trabajo y las exportaciones PDF en las carpetas obligatorias de OneDrive.
4. Comprueba que no existen versiones finales almacenadas en:
   - Escritorio.
   - Descargas.
   - Unidades USB.
   - Carpetas locales no administradas.
5. Mantén el registro de fuentes, la matriz y el caso de negocio disponibles para la Práctica 4.
6. No elimines los archivos de las prácticas anteriores, ya que serán necesarios para consolidar el expediente técnico final.

---

## 10. Resumen

En esta práctica has construido una cadena de evidencia comercial para NOVA Hydrate: investigación competitiva verificable, puntuación comparativa, identificación de brechas, propuesta de valor, hipótesis de lanzamiento, riesgos e indicadores iniciales.

Los entregables creados serán la base sin modificaciones estructurales de la consolidación documental y de la presentación ejecutiva de la Práctica 4. Antes de avanzar, asegúrate de que todas las conclusiones pueden rastrearse hasta una fuente, un cálculo o una hipótesis claramente identificada.

### Entregables finales

| Entregable | Ubicación |
|---|---|
| `03_Matriz_Competitiva_NOVA_Hydrate_v1.0.xlsx` | `/03_Caso_Negocio/` |
| `03_Caso_de_Negocio_NOVA_Hydrate_v1.0.docx` | `/03_Caso_Negocio/` |
| `03_Registro_de_Fuentes_NOVA_Hydrate_v1.0.docx` | `/Fuentes_Verificadas/` |
| PDF de la matriz competitiva | `/Exportaciones_PDF/` |
| PDF del caso de negocio | `/Exportaciones_PDF/` |

### Recursos de consulta recomendados

- [Nielsen Norman Group: investigación de usuarios](https://www.nngroup.com/topic/user-research/)
- [IDEO Design Kit: métodos de diseño centrado en las personas](https://www.designkit.org/methods)
- [Microsoft: uso responsable de Microsoft Copilot](https://www.microsoft.com/en-us/microsoft-copilot/responsible-ai)
- Fichas oficiales de producto, distribuidores autorizados y repositorios corporativos aprobados por la organización.
