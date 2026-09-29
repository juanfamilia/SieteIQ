# Siete IQ — Agent Instructions

## 1. Propósito del proyecto

Siete IQ es el motor de inteligencia de **Siete Inteligencia Creativa**.

No es un dashboard, un chatbot, una agencia tradicional de investigación de mercado ni una colección de agentes de IA.

Su propósito es construir un sistema replicable que permita transformar:

**fuentes → datos → contexto → relaciones → señales → hipótesis → evidencia → inteligencia → acción → aprendizaje**

El objetivo es ayudar a una persona u organización a entender mejor qué está ocurriendo, qué podría explicarlo, qué no sabemos todavía, qué preguntas deben hacerse y qué acciones pueden probarse.

El sistema debe ser capaz de:

* observar;
* comparar;
* detectar cambios y patrones;
* relacionar información de diferentes fuentes;
* formular preguntas;
* generar hipótesis;
* cuestionar sus propias hipótesis;
* identificar incertidumbre;
* explicar sus razonamientos;
* proponer acciones;
* definir cómo medir esas acciones;
* aprender de nuevos resultados.

---

# 2. Principio fundamental

## REALIDAD ANTES QUE IMPRESIÓN

Siete IQ debe preferir una respuesta incompleta pero sustentada antes que una respuesta espectacular pero inventada.

Nunca fabricar:

* datos;
* fuentes;
* citas;
* estadísticas;
* relaciones;
* causalidades;
* resultados;
* conclusiones;
* capacidades del sistema;
* capacidades de una herramienta;
* información sobre una organización;
* información sobre una persona;
* resultados de una consulta que no se haya ejecutado.

Si una información no está disponible, el sistema debe decir:

> "No tenemos evidencia suficiente para determinarlo."

Cuando corresponda, debe explicar qué información adicional permitiría avanzar.

---

# 3. Mejor caso, pero real

El proyecto debe buscar un **best case realista**.

"Best case" significa:

* arquitectura sólida;
* automatización progresiva;
* buena experiencia de usuario;
* capacidad de escalar;
* procesos reproducibles;
* uso inteligente de LLM;
* capacidad de trabajar con múltiples fuentes;
* resultados útiles para decisiones;
* bajo costo inicial;
* independencia razonable de proveedores.

No significa:

* asumir capacidades que todavía no existen;
* construir sistemas innecesariamente complejos;
* utilizar tecnologías solamente porque son populares;
* crear agentes autónomos sin necesidad;
* pretender que el LLM razona correctamente por defecto;
* afirmar causalidad sin diseño/evidencia apropiada;
* prometer automatización total;
* construir infraestructura empresarial antes de validar el problema.

La implementación debe ser **la más sencilla que permita alcanzar el resultado requerido con calidad suficiente**.

---

# 4. Rol del agente de programación

El coding agent es un ejecutor técnico.

No es el propietario del producto.

No debe cambiar por iniciativa propia:

* la visión de Siete IQ;
* la metodología de inteligencia;
* la arquitectura conceptual;
* los criterios de evidencia;
* las definiciones de inteligencia;
* las prioridades del producto;
* los criterios comerciales.

Si una decisión de producto o arquitectura importante no está especificada, el agente debe:

1. identificar la incertidumbre;
2. explicar las alternativas;
3. recomendar una opción si tiene evidencia suficiente;
4. solicitar confirmación cuando la decisión pueda afectar significativamente el proyecto.

No debe ocultar incertidumbre detrás de código.

---

# 5. Principios de ingeniería

## 5.1 Simplicidad

Preferir:

* Python;
* PostgreSQL;
* DuckDB;
* Polars/Pandas cuando sean apropiados;
* SQL;
* Git;
* APIs simples;
* estructuras de datos claras.

Evitar inicialmente:

* Kubernetes;
* microservicios innecesarios;
* Spark;
* Databricks;
* arquitecturas distribuidas;
* data lakes complejos;
* entrenamiento de modelos propios;
* sistemas de agentes múltiples sin necesidad;
* infraestructura costosa.

La complejidad debe justificarse por una necesidad real.

---

# 6. Independencia de proveedores

Siete IQ no debe depender conceptualmente de un único proveedor de IA.

El código debe separar:

**inteligencia de negocio**

de

**proveedor/modelo de IA**.

Cuando se utilice un LLM, crear una interfaz que permita cambiar posteriormente de proveedor.

Ejemplo conceptual:

```text
IQ
 │
 └── LLM Interface
       ├── Provider A
       ├── Provider B
       ├── Provider C
       └── Local model
```

No implementar integraciones múltiples solamente por anticipación.

Primero debe existir una necesidad real.

---

# 7. LLM: qué puede hacer y qué no

El LLM puede utilizarse para tareas como:

* interpretación de lenguaje;
* clasificación;
* extracción de entidades;
* generación de preguntas;
* generación de hipótesis;
* resumen;
* comparación semántica;
* explicación;
* búsqueda asistida;
* identificación de posibles relaciones;
* generación de alternativas;
* cuestionamiento de una hipótesis;
* traducción entre lenguaje técnico y ejecutivo.

El LLM NO debe ser la autoridad para:

* cálculos financieros;
* cálculos estadísticos;
* agregaciones;
* porcentajes;
* conteos;
* fechas;
* identificadores;
* reglas determinísticas;
* resultados matemáticos;
* datos oficiales;
* causalidad científica;
* hechos que puedan verificarse directamente.

Cuando una operación pueda ejecutarse determinísticamente con código o SQL, debe preferirse código o SQL.

---

# 8. Evidencia

Toda afirmación relevante producida por Siete IQ debe poder clasificarse.

Tipos mínimos:

* `OBSERVATION`
* `CALCULATION`
* `ESTIMATE`
* `INFERENCE`
* `HYPOTHESIS`
* `ACTION`
* `OUTCOME`
* `UNKNOWN`

El sistema debe evitar presentar una inferencia como si fuera un dato observado.

Siempre que sea posible registrar:

* fuente;
* dataset;
* variable;
* período;
* población;
* unidad;
* método;
* transformación;
* fecha de procesamiento;
* evidencia utilizada;
* nivel de confianza;
* limitaciones.

---

# 9. Causalidad

Siete IQ no debe convertir automáticamente una relación estadística en causalidad.

Ejemplo:

Incorrecto:

> "La inversión provocó el aumento del rendimiento."

Si los datos solamente muestran una asociación:

> "La inversión y el rendimiento aumentaron conjuntamente."

La conclusión causal requiere evidencia y diseño adecuados.

Cuando exista una posible relación causal, utilizar lenguaje como:

* "podría estar relacionado";
* "es consistente con";
* "sugiere";
* "merece investigación";
* "no podemos determinar causalidad con estos datos".

---

# 10. Comparabilidad

Antes de comparar dos datos, verificar cuando sea relevante:

* definición;
* población;
* unidad;
* período;
* metodología;
* cobertura;
* escala;
* composición;
* fuente;
* cambios metodológicos;
* datos faltantes;
* incertidumbre.

No asumir que dos números son comparables simplemente porque tienen el mismo nombre.

---

# 11. El modelo de inteligencia

El sistema debe aspirar a producir la siguiente cadena:

```text
DATA
  ↓
CONTEXT
  ↓
COMPARISON
  ↓
RELATIONSHIP
  ↓
SIGNAL
  ↓
QUESTION
  ↓
HYPOTHESIS
  ↓
CHALLENGE
  ↓
EVIDENCE
  ↓
INTELLIGENCE
  ↓
IMPLICATION
  ↓
ACTION
  ↓
OUTCOME
  ↓
LEARNING
```

La cadena no debe ejecutarse artificialmente si una etapa no tiene evidencia suficiente.

Es válido detenerse.

Por ejemplo:

```text
DATA
  ↓
COMPARISON
  ↓
SIGNAL
  ↓
UNKNOWN
```

Esto puede ser un resultado correcto.

---

# 12. Challenge Engine

Una conclusión no debe considerarse madura simplemente porque un LLM la generó.

Cuando sea apropiado, el sistema debe intentar debilitarla.

Debe preguntar:

* ¿qué evidencia contradice esta hipótesis?
* ¿qué explicación alternativa existe?
* ¿hay una variable omitida?
* ¿cambió la metodología?
* ¿cambió la composición de la población?
* ¿hay selección de casos?
* ¿la relación podría ser espuria?
* ¿el período analizado es suficiente?
* ¿qué información todavía falta?
* ¿qué tendría que observarse para considerar incorrecta esta explicación?

El objetivo no es destruir toda conclusión.

El objetivo es evitar conclusiones débiles presentadas como certezas.

---

# 13. Incertidumbre

La incertidumbre es un resultado válido del sistema.

Siete IQ debe distinguir entre:

* sabemos;
* calculamos;
* estimamos;
* inferimos;
* sospechamos;
* proponemos como hipótesis;
* no sabemos.

Nunca utilizar un porcentaje de "confidence" simplemente porque el modelo lo generó.

Un nivel de confianza debe tener una definición y metodología documentada.

---

# 14. Lentes

Siete IQ puede analizar un problema desde diferentes perspectivas.

Inicialmente pueden incluir:

* docente;
* director de centro;
* técnico distrital;
* familia/APMAE;
* estudiante;
* gestión central;
* planificación/finanzas;
* investigador;
* Siete IQ.

Los lentes no son personajes ficticios.

Cada lente representa:

* objetivos;
* decisiones;
* información disponible;
* restricciones;
* preguntas;
* intereses;
* horizonte temporal.

Los lentes pueden discrepar.

El sistema no debe elegir automáticamente quién tiene razón.

Debe mostrar:

**qué observa cada lente + qué evidencia lo respalda + dónde existe discrepancia.**

---

# 15. Acciones

Una acción propuesta debe ser concreta.

Cuando sea posible debe especificar:

* qué;
* quién;
* dónde;
* cuándo;
* para qué;
* recursos necesarios;
* indicador de seguimiento;
* resultado esperado;
* cómo determinar si funcionó.

Una recomendación genérica como:

> "Hay que mejorar la educación."

no constituye una acción útil.

---

# 16. Datos

Nunca modificar los datos originales.

Utilizar una separación conceptual:

```text
data/raw/
data/processed/
data/external/
```

Los archivos originales deben permanecer preservados.

Toda transformación debe ser reproducible.

Cuando sea posible:

```text
RAW
 ↓
EXTRACT
 ↓
VALIDATE
 ↓
NORMALIZE
 ↓
TRANSFORM
 ↓
ANALYZE
```

Debe ser posible volver a ejecutar el proceso.

---

# 17. Fuentes

Las fuentes deben conservar su procedencia.

Registrar cuando sea posible:

* nombre de la fuente;
* organización;
* URL o referencia;
* fecha de acceso;
* período de los datos;
* archivo original;
* versión;
* metodología;
* limitaciones.

Preferir fuentes primarias y oficiales cuando existan.

Las fuentes secundarias pueden utilizarse cuando aporten información relevante, pero deben identificarse como tales.

---

# 18. Proyecto inicial: PISA

El primer laboratorio de Siete IQ será educación utilizando PISA como una de las fuentes.

PISA NO es el producto.

PISA NO debe utilizarse para crear rankings de centros educativos que los datos no permitan sostener.

El objetivo inicial es demostrar que Siete IQ puede pasar de:

> "República Dominicana obtuvo X puntos."

a:

> "¿Qué cambió, dónde, en qué población, en qué contexto, qué relaciones aparecen, qué explicaciones son compatibles con los datos, cuáles no podemos sostener y qué debería investigarse o probarse?"

El sistema debe reconocer las limitaciones de la muestra y del diseño de PISA.

No extrapolar resultados a niveles que el diseño de la fuente no permita.

---

# 19. Arquitectura inicial

La arquitectura conceptual es:

```text
SOURCES
   ↓
INGESTION
   ↓
RAW DATA
   ↓
VALIDATION
   ↓
NORMALIZATION
   ↓
DATA MODEL
   ↓
ANALYTICAL ENGINE
   ↓
EVIDENCE MODEL
   ↓
INTELLIGENCE ENGINE
   ↓
LLM / REASONING LAYER
   ↓
CHALLENGE
   ↓
LENSES
   ↓
ACTION
   ↓
USER INTERFACE
```

No construir todos los componentes simultáneamente.

Cada capa debe demostrar utilidad antes de aumentar la complejidad.

---

# 20. Base tecnológica inicial

Preferencias iniciales:

* Python 3.12;
* PostgreSQL;
* Supabase como infraestructura inicial si resulta conveniente;
* DuckDB para análisis local;
* Polars/Pandas según necesidad;
* Git/GitHub;
* Next.js para interfaz cuando sea necesario;
* APIs de LLM mediante una capa de abstracción;
* Docker solamente cuando aporte valor real.

Estas son preferencias, no dogmas.

Una tecnología puede cambiar si existe una razón técnica documentada.

---

# 21. Seguridad

Nunca colocar en Git:

* API keys;
* passwords;
* tokens;
* secrets;
* credenciales;
* archivos `.env` reales.

Utilizar:

```text
.env
.env.example
```

`.env` debe estar incluido en `.gitignore`.

Nunca imprimir secretos en logs.

---

# 22. Código

El código debe priorizar:

* claridad;
* funciones pequeñas;
* nombres descriptivos;
* tipos cuando aporten valor;
* manejo explícito de errores;
* validación de inputs;
* tests;
* documentación;
* reproducibilidad.

No escribir código innecesariamente sofisticado.

No crear abstracciones "por si acaso".

No duplicar lógica si una abstracción sencilla resuelve el problema.

---

# 23. Tests

Toda funcionalidad importante debe tener una forma objetiva de comprobarse.

Priorizar:

* unit tests;
* tests de integración cuando sean necesarios;
* validación de schemas;
* tests de datos;
* tests de reproducibilidad.

Un módulo no está terminado simplemente porque "corre".

Debe poder verificarse.

---

# 24. Evaluación de inteligencia

Siete IQ necesita evaluar no solamente si el software funciona, sino si sus resultados son buenos.

Las evaluaciones pueden clasificar resultados como:

* `CORRECT`
* `INCORRECT`
* `INCOMPLETE`
* `UNSUPPORTED`
* `INTERESTING`
* `REDUNDANT`
* `INVALID_ACTION`
* `GOOD_QUESTION`

La evaluación humana inicial es parte del desarrollo del sistema.

No asumir que una respuesta generada por un LLM es correcta porque suena convincente.

---

# 25. Documentación

Cada módulo importante debe documentar:

1. qué hace;
2. qué problema resuelve;
3. inputs;
4. outputs;
5. dependencias;
6. cómo ejecutarlo;
7. cómo verificarlo;
8. limitaciones;
9. decisiones relevantes.

La documentación debe describir el sistema real, no el sistema imaginado.

---

# 26. Workflow obligatorio del coding agent

Antes de modificar código:

1. inspeccionar el repositorio;
2. identificar archivos relevantes;
3. comprender las convenciones existentes;
4. determinar dependencias;
5. describir brevemente el cambio propuesto;
6. implementar la modificación más pequeña que resuelva el problema;
7. ejecutar tests/validaciones;
8. corregir errores;
9. revisar efectos secundarios;
10. documentar lo necesario;
11. resumir qué cambió y cómo verificarlo.

No reescribir archivos completos si un cambio localizado es suficiente.

No crear archivos innecesarios.

No cambiar tecnologías sin justificación.

---

# 27. Regla contra la alucinación técnica

Si el agente no sabe:

* una API;
* una versión;
* una función;
* un comportamiento de una librería;
* una estructura de datos;
* una capacidad de una herramienta;

debe verificarlo mediante documentación disponible o inspección del entorno.

Nunca inventar una API para que el código parezca completo.

Si no puede verificarlo:

> indicar la incertidumbre antes de implementarlo.

---

# 28. Regla contra el sobreingeniería

Antes de agregar una tecnología, servicio, agente o dependencia, preguntar:

> ¿Qué problema real resuelve ahora?

Si la respuesta es "lo necesitaremos cuando escalemos", no incorporarlo todavía salvo que el costo de introducirlo posteriormente sea materialmente mayor.

---

# 29. Agentes

No construir un sistema multiagente simplemente porque es posible.

Inicialmente preferir:

1. workflow determinístico;
2. funciones especializadas;
3. un LLM cuando aporte valor;
4. evaluación;
5. automatización;
6. agentes solamente cuando exista una tarea que realmente se beneficie de autonomía.

La autonomía debe ganarse mediante evidencia de confiabilidad.

---

# 30. Principio de reproducibilidad

El conocimiento de Juan debe convertirse progresivamente en:

* reglas;
* schemas;
* procesos;
* código;
* prompts versionados;
* evaluaciones;
* documentación;
* datasets de prueba.

El objetivo es que Siete IQ no dependa permanentemente de la memoria o criterio tácito de una sola persona.

La automatización debe capturar el proceso, no reemplazar ciegamente el juicio.

---

# 31. Principio de aprendizaje

Cada error importante debe convertirse, cuando sea apropiado, en:

* un test;
* una regla;
* una validación;
* una mejora de documentación;
* una mejora del prompt;
* una mejora del modelo;
* o una decisión explícita de no automatizar.

No corregir repetidamente el mismo problema de forma manual.

---

# 32. Regla de oro

Siete IQ no debe intentar impresionar con información.

Debe conseguir que el usuario pueda decir:

> **"Ahora entiendo mejor qué está pasando, sé qué no sabemos y sé cuál es la siguiente pregunta o acción que tiene sentido."**

Si además puede demostrar:

> **qué evidencia sustenta esa inteligencia,**

y posteriormente:

> **qué ocurrió después de actuar,**

entonces estamos construyendo un sistema de inteligencia y no simplemente un sistema de generación de respuestas.

---

# 33. Criterio final de calidad

Antes de considerar terminada una funcionalidad, evaluar:

### REAL

¿Funciona realmente?

### VERIFICABLE

¿Podemos comprobarlo?

### REPRODUCIBLE

¿Podemos ejecutarlo nuevamente?

### EXPLICABLE

¿Podemos entender cómo llegó al resultado?

### SUSTENTADO

¿La evidencia respalda la afirmación?

### ÚTIL

¿Ayuda a responder una pregunta real?

### ACCIONABLE

¿Puede conducir a una acción razonable?

### MANTENIBLE

¿Otra persona podría entender y modificar el sistema?

### ECONÓMICO

¿La complejidad y el costo están justificados?

Si no cumple alguno de estos criterios, no asumir que está terminado.

---

# 34. Prioridad absoluta

Durante la construcción inicial:

**CALIDAD > VELOCIDAD**

pero:

**SIMPLICIDAD > COMPLEJIDAD**

y:

**REALIDAD > APARIENCIA**

El sistema debe evolucionar mediante pequeños incrementos verificables.

No construir una gran plataforma hipotética.

Construir una capacidad real, comprobarla y después ampliarla.
