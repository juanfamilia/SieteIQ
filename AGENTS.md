# SieteIQ — Agent Operating Instructions

## 1. Propósito del proyecto

SieteIQ es un sistema de inteligencia diseñado para transformar evidencia y datos relevantes en entendimiento útil para la toma de decisiones, la acción y el aprendizaje.

Su propósito no es producir más datos, más reportes ni más dashboards.

Su propósito es ayudar a responder, de forma verificable:

* ¿Qué está pasando?
* ¿Qué sabemos realmente?
* ¿Qué relaciones o patrones podemos observar?
* ¿Qué podría explicar lo que estamos viendo?
* ¿Qué no sabemos?
* ¿Qué información necesitamos para reducir la incertidumbre?
* ¿Qué decisiones o acciones podrían considerarse?
* ¿Qué ocurrió después?
* ¿Qué aprendimos?

## 2. Principio rector

La cadena fundamental de SieteIQ es:

**DATOS → INFORMACIÓN → ENTENDIMIENTO → DECISIÓN → ACCIÓN → RESULTADO → APRENDIZAJE**

Esta cadena debe orientar las decisiones de producto, arquitectura, datos, análisis, inteligencia artificial e interfaz.

La tecnología es un **habilitador**.

No es el producto.

## 3. Qué SieteIQ NO es

SieteIQ no debe convertirse en:

* un dashboard por el simple hecho de tener datos;
* una herramienta de Business Intelligence tradicional;
* una base de datos presentada como producto;
* un generador automático de informes;
* un chatbot que responde preguntas sin evidencia;
* una colección de agentes autónomos sin propósito;
* una demostración tecnológica;
* una plataforma que produzca conclusiones para impresionar al usuario;
* una agencia de investigación tradicional disfrazada de tecnología.

Un dashboard puede formar parte de SieteIQ.

Una base de datos puede formar parte de SieteIQ.

Un LLM puede formar parte de SieteIQ.

Pero ninguno de ellos constituye por sí mismo la inteligencia.

## 4. Inteligencia antes que interfaz

Una interfaz no debe ocultar la ausencia de inteligencia.

Antes de construir una visualización, reporte, chatbot o pantalla, debe existir una razón clara:

**¿Qué entendimiento o decisión mejora esta interfaz?**

Si una visualización no mejora el entendimiento, no es prioritaria.

Si una funcionalidad no ayuda a responder una pregunta relevante, reducir incertidumbre, evaluar una hipótesis, tomar una decisión, ejecutar una acción o aprender de un resultado, debe cuestionarse su necesidad.

La apariencia nunca debe sustituir el valor analítico.

## 5. Data ≠ Information ≠ Intelligence

SieteIQ debe mantener una distinción explícita entre:

### Datos

Observaciones, registros, mediciones, documentos o valores provenientes de una fuente.

### Información

Datos organizados y contextualizados de forma que permitan describir qué está ocurriendo.

### Entendimiento

Interpretación fundamentada que relaciona información, contexto, comparación, conocimiento y evidencia.

### Inteligencia

Entendimiento estructurado alrededor de una pregunta o decisión, incluyendo evidencia, hipótesis, incertidumbre, alternativas y posibles implicaciones.

### Acción

Una decisión ejecutada o una intervención concreta derivada del entendimiento.

### Resultado

Lo que ocurrió después de la acción.

### Aprendizaje

La actualización del entendimiento a partir de los resultados observados.

No asumir que una etapa existe simplemente porque existe la anterior.

Tener datos no significa tener información.

Tener información no significa comprender.

Comprender no garantiza una buena decisión.

Una decisión no equivale a una acción.

Una acción no garantiza un resultado.

Y un resultado sin aprendizaje no completa el ciclo.

## 6. La inteligencia debe ser verificable

Toda afirmación producida por SieteIQ debe poder clasificarse.

Como mínimo, distinguir:

* **OBSERVADO** — directamente presente en una fuente.
* **CALCULADO** — obtenido mediante una operación reproducible.
* **ESTIMADO** — aproximación basada en supuestos explícitos.
* **INFERIDO** — interpretación derivada de evidencia disponible.
* **HIPÓTESIS** — explicación posible que todavía necesita validación.
* **PROPUESTA** — posible acción o decisión.
* **RESULTADO** — consecuencia observada posteriormente.
* **DESCONOCIDO** — información que no está disponible o no puede establecerse.
* **CONFLICTIVO** — fuentes o evidencias que no coinciden.

No presentar una inferencia como un hecho.

No presentar una hipótesis como una conclusión.

No presentar una estimación como un dato observado.

No ocultar la ausencia de información.

## 7. Evidencia y procedencia

Toda fuente relevante debe conservar su procedencia.

Cuando sea posible, registrar:

* fuente;
* fecha;
* período de referencia;
* ubicación o URL;
* metodología conocida;
* unidad de medida;
* población o universo;
* versión;
* fecha de acceso;
* transformaciones realizadas;
* supuestos relevantes.

Los datos externos deben distinguirse de los datos generados internamente.

Nunca eliminar el origen de un dato durante una transformación si conservarlo es técnicamente posible.

La trazabilidad debe permitir responder:

**¿De dónde salió esta afirmación?**

## 8. No confundir correlación con causalidad

SieteIQ debe ser especialmente cuidadoso con explicaciones causales.

Una coincidencia temporal, correlación estadística o relación aparente no demuestra causalidad.

Cuando la evidencia no permita establecer causalidad, utilizar lenguaje apropiado:

* asociado con;
* coincide con;
* podría estar relacionado con;
* es consistente con;
* constituye una hipótesis;
* requiere investigación adicional.

No convertir una correlación en una explicación causal mediante lenguaje generado por IA.

## 9. Comparabilidad

Antes de comparar datos, comprobar si realmente son comparables.

Considerar, cuando corresponda:

* período;
* población;
* universo;
* definición;
* unidad;
* metodología;
* cobertura;
* geografía;
* fuente;
* cambios regulatorios;
* cambios metodológicos.

Una diferencia numérica no necesariamente representa una diferencia real del fenómeno.

## 10. Contexto antes de interpretación

Los números deben interpretarse dentro de su contexto.

SieteIQ debe buscar, cuando sea relevante:

* histórico;
* geográfico;
* económico;
* demográfico;
* institucional;
* regulatorio;
* competitivo;
* operativo;
* temporal.

No utilizar una cifra aislada para construir una conclusión amplia cuando el contexto disponible pueda cambiar su interpretación.

## 11. Preguntas antes que respuestas

SieteIQ debe privilegiar la formulación correcta del problema.

Una buena respuesta a una mala pregunta puede producir una mala decisión.

Ante una pregunta ambigua:

1. identificar la ambigüedad;
2. explicitar los supuestos;
3. determinar qué información está disponible;
4. determinar qué información falta;
5. reformular la pregunta cuando sea necesario.

El sistema debe poder decir:

**“No sabemos todavía.”**

Eso es un resultado válido.

## 12. Hipótesis

Cuando exista una explicación posible, estructurarla como hipótesis.

Una hipótesis debe poder relacionarse con:

* evidencia que la respalda;
* evidencia que la contradice;
* información faltante;
* explicaciones alternativas;
* nivel de incertidumbre;
* método posible de validación.

No construir una única narrativa cuando existen explicaciones plausibles alternativas.

## 13. Challenge Engine

SieteIQ debe intentar debilitar sus propias conclusiones.

Cuando una hipótesis o interpretación sea relevante, el sistema debe preguntarse:

* ¿Qué evidencia contradice esta hipótesis?
* ¿Qué otra explicación podría producir el mismo patrón?
* ¿Qué supuesto estamos dando por cierto?
* ¿Qué dato podría cambiar la conclusión?
* ¿Estamos confundiendo correlación con causalidad?
* ¿La fuente es suficiente para esta afirmación?
* ¿Estamos extrapolando más allá de la población observada?

El objetivo no es generar duda artificial.

El objetivo es reducir conclusiones frágiles.

## 14. Lentes de decisión

SieteIQ puede examinar un problema desde diferentes perspectivas cuando estas sean relevantes.

Ejemplos:

* dirección;
* finanzas;
* operaciones;
* comercial;
* investigación;
* gestión pública;
* docente;
* dirección escolar;
* estudiante;
* familia;
* territorio;
* planificación.

Estas perspectivas no son “personas artificiales” que deben actuar como personajes.

Son **lentes analíticos**.

Dos lentes pueden producir interpretaciones diferentes.

SieteIQ no debe ocultar automáticamente esa discrepancia.

Debe mostrar la evidencia, los supuestos y las diferencias de perspectiva.

## 15. El papel de la inteligencia artificial

Los LLM son herramientas de razonamiento lingüístico y asistencia analítica.

Pueden utilizarse para:

* interpretar lenguaje;
* clasificar información;
* extraer entidades;
* estructurar documentos;
* generar preguntas;
* formular hipótesis;
* identificar posibles relaciones;
* comparar textos o contextos;
* proponer explicaciones alternativas;
* desafiar hipótesis;
* sintetizar evidencia;
* explicar resultados;
* ayudar a construir consultas.

No deben ser la autoridad final para:

* cálculos determinísticos;
* agregaciones;
* identificadores;
* fechas verificables;
* valores que pueden calcularse directamente;
* hechos oficiales cuando exista una fuente verificable;
* conclusiones causales sin evidencia adecuada.

Cuando una máquina pueda calcular algo de manera determinística, debe hacerlo mediante código o una herramienta determinística, no mediante una estimación lingüística del LLM.

## 16. La arquitectura debe preservar la independencia del proveedor

SieteIQ no debe depender estructuralmente de un único proveedor de IA.

La arquitectura debe permitir, cuando sea razonable:

* cambiar de modelo;
* cambiar de proveedor;
* utilizar modelos locales;
* utilizar APIs externas;
* funcionar parcialmente sin LLM.

El conocimiento, los datos, las reglas y la lógica del sistema pertenecen al proyecto.

No deben quedar encerrados innecesariamente dentro de un proveedor.

## 17. Arquitectura conceptual

La arquitectura inicial debe seguir esta lógica:

**FUENTES**
↓
**INGESTIÓN**
↓
**DATOS RAW**
↓
**VALIDACIÓN**
↓
**NORMALIZACIÓN**
↓
**MODELO DE DATOS**
↓
**MOTOR ANALÍTICO**
↓
**MODELO DE EVIDENCIA**
↓
**MOTOR DE INTELIGENCIA**
↓
**CAPA LLM / RAZONAMIENTO**
↓
**CHALLENGE**
↓
**LENTES**
↓
**DECISIÓN / ACCIÓN**
↓
**RESULTADO**
↓
**APRENDIZAJE**

La implementación concreta puede cambiar.

La cadena lógica no debe perderse.

## 18. Simplicidad primero

Construir la solución más sencilla que permita demostrar la hipótesis del producto.

No introducir tecnología por prestigio, moda o anticipación.

Evitar inicialmente, salvo necesidad demostrada:

* Kubernetes;
* microservicios;
* Spark;
* Databricks;
* arquitecturas distribuidas;
* data lakes complejos;
* entrenamiento de modelos propios;
* sistemas multiagente complejos;
* infraestructura innecesaria;
* múltiples bases de datos sin justificación.

La complejidad debe ser consecuencia de una necesidad real.

## 19. Stack inicial preferido

Cuando sea apropiado, el proyecto puede comenzar con:

* Python;
* PostgreSQL;
* DuckDB;
* Polars o Pandas;
* Git/GitHub;
* una capa de aplicación sencilla;
* un proveedor LLM intercambiable.

Supabase puede utilizarse como infraestructura inicial cuando simplifique el desarrollo.

Estas tecnologías no son dogmas.

Si una alternativa resulta técnicamente más apropiada, documentar la razón.

## 20. Separación de datos

Mantener conceptualmente separados:

* datos originales;
* datos procesados;
* datos derivados;
* datos externos;
* resultados analíticos;
* hipótesis;
* conclusiones;
* acciones;
* resultados posteriores.

No sobrescribir información original innecesariamente.

Las transformaciones importantes deben ser reproducibles.

## 21. Reproducibilidad

Un resultado importante debe poder reproducirse.

Siempre que sea razonable, conservar:

* código;
* versión;
* parámetros;
* fuentes;
* fechas;
* supuestos;
* transformaciones;
* consultas;
* modelo utilizado;
* instrucciones relevantes para el LLM.

Una respuesta que no puede reconstruirse debe tratarse con mayor cautela.

## 22. Acción

La inteligencia no termina en una explicación.

Cuando corresponda, una salida puede especificar:

* decisión que debe considerarse;
* acción propuesta;
* responsable;
* horizonte temporal;
* indicador de seguimiento;
* condición de éxito;
* riesgos;
* información que debe revisarse posteriormente.

SieteIQ no debe ejecutar automáticamente acciones de alto impacto sin autorización humana explícita.

## 23. Resultados y aprendizaje

Cuando una acción sea ejecutada y exista información posterior, SieteIQ debe poder registrar:

* qué se decidió;
* qué se hizo;
* cuándo;
* qué se esperaba;
* qué ocurrió;
* qué evidencia apareció;
* qué hipótesis se fortalecieron;
* qué hipótesis se debilitaron;
* qué cambió en el entendimiento.

El objetivo final es cerrar el ciclo:

**Entender → Decidir → Actuar → Medir → Aprender.**

## 24. Seguridad y control humano

No ejecutar acciones destructivas, irreversibles o de alto impacto sin autorización explícita.

No exponer secretos, credenciales, tokens o información privada.

No incorporar credenciales directamente al código.

Las operaciones que puedan modificar datos, infraestructura o repositorios deben ser explícitas y revisables.

El agente técnico ejecuta instrucciones.

No sustituye al responsable del producto.

## 25. Rol del agente

El agente es un **ejecutor técnico y asistente de ingeniería**.

Debe:

* inspeccionar antes de modificar;
* explicar decisiones importantes;
* respetar este documento;
* evitar inventar;
* identificar incertidumbres;
* mantener cambios pequeños y revisables;
* escribir código mantenible;
* probar lo que construye;
* documentar decisiones relevantes.

No debe asumir decisiones de producto que correspondan al responsable humano.

## 26. Regla de realidad

Antes de afirmar que una funcionalidad existe, comprobar que existe.

Antes de afirmar que un dato es correcto, verificar su fuente.

Antes de afirmar que un sistema funciona, probarlo.

Antes de agregar una dependencia, demostrar que es necesaria.

Antes de crear una arquitectura compleja, demostrar que la simplicidad no es suficiente.

Si algo no puede verificarse, decirlo explícitamente.

## 27. Criterio de calidad

Una implementación de SieteIQ debe aspirar a ser:

**REAL**
Existe y funciona.

**VERIFICABLE**
Sus afirmaciones y resultados pueden comprobarse.

**REPRODUCIBLE**
Puede reconstruirse el resultado.

**EXPLICABLE**
Puede entenderse cómo se llegó a él.

**SUSTENTADA**
Las conclusiones tienen evidencia suficiente.

**ÚTIL**
Mejora el entendimiento de un problema real.

**ACCIONABLE**
Puede contribuir a una decisión o acción.

**MANTENIBLE**
Puede modificarse sin reconstruir todo el sistema.

**ECONÓMICA**
La complejidad y el costo son proporcionales al valor obtenido.

## 28. Anti-overengineering

No construir infraestructura para problemas que todavía no existen.

No crear abstracciones prematuras.

No crear agentes porque “podrían ser útiles”.

No incorporar una tecnología porque sea técnicamente interesante.

Primero demostrar valor.

Después escalar la arquitectura según la evidencia.

## 29. Aprendizaje a partir de errores

Los errores son información.

Cuando una implementación falle:

1. identificar la causa;
2. documentarla cuando sea relevante;
3. corregirla;
4. determinar si una regla, prueba o procedimiento puede evitar su repetición.

No ocultar errores para mantener una apariencia de progreso.

## 30. Gold Rule

Cuando exista conflicto entre:

* velocidad y calidad;
* apariencia y realidad;
* complejidad y simplicidad;
* automatización y control;
* una respuesta convincente y una respuesta verificable;

priorizar:

**REALIDAD > APARIENCIA**

**VERIFICABILIDAD > CONVICCIÓN**

**SIMPLICIDAD > COMPLEJIDAD**

**CALIDAD > VELOCIDAD**

**EVIDENCIA > SUPOSICIÓN**

**UTILIDAD > DEMOSTRACIÓN TECNOLÓGICA**

**APRENDIZAJE > PERFECCIÓN INICIAL**

## 31. Definición operativa de éxito

SieteIQ está avanzando cuando puede demostrar, con un caso real:

**que una fuente de datos relevante puede transformarse de manera reproducible en información;**

**que esa información puede contextualizarse y analizarse;**

**que el sistema puede distinguir hechos, cálculos, inferencias e hipótesis;**

**que puede producir entendimiento útil;**

**que ese entendimiento puede informar una decisión o acción;**

**y que el resultado posterior puede alimentar nuevamente el sistema.**

El objetivo no es construir primero una gran plataforma.

El objetivo es demostrar que esta cadena funciona.

**Datos → Información → Entendimiento → Decisión → Acción → Resultado → Aprendizaje.**
