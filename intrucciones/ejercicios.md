# Criterios para desarrollar los ejercicios

Este archivo establece los criterios específicos que deben seguirse al crear,
revisar, ampliar o corregir los archivos `ejercicios.tex` del proyecto de
Física.

Las reglas generales del proyecto se encuentran en `AGENTS.md`.

Las decisiones de arquitectura y configuración LaTeX se encuentran en
`instrucciones/configuracion.md`.

Los criterios de desarrollo conceptual se encuentran en
`instrucciones/teoria.md`.

Los criterios del material de consulta rápida se encuentran en
`instrucciones/formulario.md`.

El estado actual del proyecto y el punto exacto de continuación se encuentran
en `pendientes.md`.

Este archivo no debe utilizarse para registrar progreso ni decisiones
estructurales generales.

Su función exclusiva es establecer **cómo deben diseñarse, redactarse,
organizarse, resolver, verificar y revisar los ejercicios de cada tema**.

---

# 1. Objetivo general de los ejercicios

Los ejercicios tienen como objetivo practicar, consolidar, integrar y comprobar
la comprensión de los conceptos desarrollados en la teoría.

No deben limitarse a sustituir valores en fórmulas.

Deben desarrollar progresivamente:

- comprensión física;
- comprensión del enunciado;
- identificación del sistema físico;
- identificación de datos e incógnitas;
- establecimiento de sistemas de referencia;
- construcción e interpretación de diagramas;
- selección del modelo físico;
- identificación de hipótesis y aproximaciones;
- selección del principio o ley apropiada;
- elección de ecuaciones;
- razonamiento escalar y vectorial;
- manejo de unidades;
- análisis dimensional;
- desarrollo algebraico;
- cálculo;
- interpretación de signos;
- interpretación de resultados;
- verificación física;
- comparación de métodos;
- autonomía para resolver problemas.

El estudiante debe avanzar desde situaciones relativamente guiadas hasta
problemas en los que deba decidir por sí mismo cómo representar, modelar y
resolver la situación.

---

# 2. Relación con la teoría

Los ejercicios deben construirse a partir de los conceptos desarrollados en
`teoria.tex`.

No debe evaluarse como contenido principal algo que no haya sido presentado o
preparado previamente en la teoría, salvo que el objetivo explícito sea razonar
a partir de conocimientos anteriores.

Los ejercicios deben permitir practicar, según corresponda:

- conceptos;
- definiciones;
- magnitudes;
- leyes;
- principios;
- modelos;
- hipótesis;
- aproximaciones;
- procedimientos;
- representaciones;
- diagramas;
- gráficas;
- interpretaciones;
- casos especiales;
- conexiones entre conceptos.

Debe existir coherencia entre `teoria.tex`, `formulario.tex` y
`ejercicios.tex`, especialmente en:

- símbolos;
- notación;
- unidades;
- terminología;
- sistemas de referencia;
- convenciones de signos;
- métodos;
- representación vectorial.

---

# 3. Los ejercicios no son una colección de sustituciones

Evitar que el conjunto de ejercicios siga únicamente el patrón:

    datos
    → elegir fórmula evidente
    → sustituir
    → calcular

La aplicación directa tiene valor pedagógico, especialmente en el nivel básico,
pero no debe constituir toda la práctica.

Los ejercicios deben desarrollar también la capacidad de:

    comprender
    → representar
    → decidir
    → plantear
    → resolver
    → interpretar
    → verificar

La dificultad debe aumentar principalmente mediante razonamiento físico y no
mediante cálculos artificialmente largos.

---

# 4. Organización en tres niveles

Los ejercicios deben organizarse siempre en tres niveles:

    Básico
    Intermedio
    Avanzado

La clasificación depende principalmente del razonamiento requerido.

No depende únicamente de:

- cantidad de operaciones;
- tamaño de los números;
- cantidad de decimales;
- dificultad aritmética;
- número de conversiones.

Un ejercicio largo no es necesariamente avanzado.

Un ejercicio conceptual de pocas líneas puede ser avanzado si exige seleccionar
correctamente un modelo, combinar principios o justificar una conclusión
física.

---

# 5. Nivel básico

El nivel básico debe desarrollar familiaridad con los conceptos y herramientas
fundamentales del tema.

Puede incluir:

- reconocimiento de magnitudes;
- identificación de unidades;
- clasificación entre escalares y vectores;
- interpretación de conceptos;
- aplicación directa de una definición;
- aplicación directa de una ley;
- lectura sencilla de gráficas;
- interpretación de diagramas;
- conversiones necesarias;
- cálculo de una magnitud a partir de datos explícitos;
- despejes sencillos;
- análisis básico de signos;
- identificación de relaciones de proporcionalidad;
- preguntas conceptuales fundamentales.

En este nivel puede resultar evidente qué relación física debe utilizarse.

Sin embargo, incluso los ejercicios básicos deben exigir comprensión de lo que
se está calculando.

No deben reducirse todos a sustitución numérica.

---

# 6. Nivel intermedio

El nivel intermedio debe exigir mayor autonomía.

Puede incluir:

- problemas de varios pasos;
- selección entre varias ecuaciones;
- combinación de dos o más relaciones;
- determinación de datos intermedios;
- uso de sistemas de referencia;
- análisis de signos;
- componentes vectoriales;
- interpretación de gráficas;
- construcción de diagramas;
- conversiones no triviales;
- análisis dimensional;
- comparación de situaciones;
- problemas inversos;
- aplicaciones contextualizadas;
- interpretación del resultado;
- conexión entre dos o más conceptos del tema;
- conexión con conocimientos anteriores.

En este nivel el estudiante no debe recibir siempre de manera evidente la
ecuación que necesita.

Debe comenzar a decidir qué información es relevante y qué estrategia utilizar.

---

# 7. Nivel avanzado

El nivel avanzado debe exigir razonamiento físico autónomo.

Puede incluir:

- elección del modelo físico;
- elección del método de solución;
- combinación de varios principios;
- deducción de relaciones;
- problemas con información indirecta;
- problemas inversos;
- comparación de métodos;
- análisis de casos límite;
- interpretación de parámetros;
- razonamiento vectorial completo;
- análisis gráfico;
- problemas simbólicos;
- justificación de aproximaciones;
- evaluación de hipótesis;
- identificación de información innecesaria;
- situaciones en las que no se indique directamente qué ley utilizar;
- problemas que admitan varios métodos;
- problemas de integración conceptual;
- análisis experimental;
- problemas en los que deba determinarse si una afirmación es físicamente
  posible.

El nivel avanzado **no consiste en utilizar números mayores ni en hacer
cálculos más largos**.

Un ejercicio avanzado debe ser más exigente principalmente por las decisiones
físicas que requiere.

---

# 8. Distribución de ejercicios

La cantidad de ejercicios depende de la extensión y complejidad del tema.

No debe imponerse artificialmente el mismo número a todos los temas.

Cuando el tema lo permita, debe existir una representación suficiente de los
tres niveles.

Si se adopta una cantidad simétrica, puede utilizarse, por ejemplo:

    24 ejercicios
    ├── 8 básicos
    ├── 8 intermedios
    └── 8 avanzados

pero esta distribución no constituye una obligación universal.

Un tema breve puede necesitar menos ejercicios.

Un tema central puede necesitar más.

La cantidad debe responder a la cobertura conceptual y no a una cuota fija.

---

# 9. Cobertura conceptual

Antes de redactar los ejercicios debe identificarse qué aspectos de la teoría
deben practicarse.

El conjunto completo debe procurar cubrir, cuando corresponda:

- definiciones;
- interpretación conceptual;
- magnitudes;
- unidades;
- leyes;
- principios;
- ecuaciones;
- condiciones de validez;
- signos;
- vectores;
- componentes;
- gráficas;
- diagramas;
- casos particulares;
- aplicaciones;
- razonamiento;
- relaciones entre conceptos.

No crear veinte ejercicios que practiquen exactamente la misma habilidad
cambiando únicamente los números.

---

# 10. Progresión

Los ejercicios deben organizarse de manera progresiva.

Una progresión posible es:

    reconocimiento
    → comprensión
    → aplicación directa
    → interpretación
    → combinación de relaciones
    → elección del método
    → integración de conceptos
    → razonamiento autónomo

La progresión debe sentirse dentro de cada nivel y también entre niveles.

Evitar saltos abruptos entre un ejercicio elemental y otro que exija
conocimientos o métodos todavía no preparados.

---

# 11. Variedad

El conjunto debe incluir variedad suficiente.

Según el tema, pueden combinarse:

- ejercicios conceptuales;
- ejercicios numéricos;
- ejercicios simbólicos;
- ejercicios gráficos;
- ejercicios vectoriales;
- ejercicios experimentales;
- ejercicios de interpretación;
- problemas inversos;
- problemas de comparación;
- problemas de estimación;
- problemas de deducción;
- problemas de aplicación;
- análisis de errores;
- problemas con varias preguntas;
- problemas que requieran justificar una respuesta.

No es necesario incluir todos estos tipos en cada tema.

La variedad debe estar al servicio del aprendizaje.

---

# 12. Ejercicios conceptuales

Los ejercicios conceptuales deben exigir razonamiento físico.

No deben reducirse únicamente a recordar una definición.

Pueden preguntar, por ejemplo:

- qué ocurriría si cambia una variable;
- cuál de varias situaciones es físicamente posible;
- cómo cambia una magnitud;
- qué signo debe tener una cantidad;
- qué gráfica representa correctamente un fenómeno;
- qué afirmación es correcta y por qué;
- qué modelo resulta apropiado;
- qué hipótesis es necesaria;
- qué resultado puede descartarse sin calcular.

Siempre que sea útil, pedir una justificación.

---

# 13. Ejercicios numéricos

Los ejercicios numéricos deben utilizar valores físicamente razonables.

Evitar datos elegidos únicamente para producir resultados enteros si esto hace
que la situación resulte artificial.

También debe evitarse introducir números incómodos sin propósito pedagógico.

Los datos deben permitir practicar:

- unidades;
- órdenes de magnitud;
- signos;
- precisión;
- interpretación.

Los valores deben revisarse antes de entregar el ejercicio.

---

# 14. Ejercicios simbólicos

Cuando aporten comprensión deben incluirse ejercicios que no proporcionen
valores numéricos.

Estos pueden pedir:

- deducir una expresión;
- despejar una magnitud;
- estudiar la dependencia entre variables;
- comparar dos casos;
- analizar un límite;
- determinar una razón;
- interpretar parámetros.

Los ejercicios simbólicos son especialmente útiles en niveles intermedio y
avanzado.

No convertirlos en manipulaciones algebraicas desconectadas de la Física.

---

# 15. Problemas inversos

Deben utilizarse problemas inversos cuando aporten comprensión.

En lugar de pedir siempre el resultado directo de una ecuación, puede
proporcionarse el resultado y solicitar:

- una condición inicial;
- una distancia;
- un tiempo;
- una velocidad;
- una aceleración;
- una masa;
- una constante;
- una carga;
- una fuerza;
- un parámetro del sistema.

Los problemas inversos ayudan a evitar la memorización mecánica de fórmulas.

---

# 16. Problemas con varias partes

Un ejercicio puede contener apartados:

    a)
    b)
    c)

cuando las preguntas formen una secuencia física coherente.

Los apartados pueden utilizarse para:

- construir progresivamente una solución;
- analizar distintas magnitudes;
- comparar situaciones;
- interpretar el resultado;
- estudiar un caso adicional.

No fragmentar artificialmente una pregunta sencilla en demasiados apartados.

---

# 17. Enunciados

Los enunciados deben ser:

- claros;
- precisos;
- físicamente coherentes;
- suficientes;
- gramaticalmente correctos;
- libres de ambigüedades innecesarias.

Deben proporcionar toda la información necesaria, salvo cuando el objetivo
deliberado sea que el estudiante deduzca una información a partir de los datos.

No ocultar información indispensable.

No proporcionar información redundante sin propósito, excepto cuando el
ejercicio avanzado busque que el estudiante identifique qué datos son
relevantes.

---

# 18. Contextualización

Los ejercicios pueden contextualizarse en situaciones:

- cotidianas;
- experimentales;
- científicas;
- tecnológicas;
- deportivas;
- astronómicas;
- industriales;
- de ingeniería.

El contexto debe ser físicamente razonable y aportar significado.

No añadir historias largas que dificulten identificar la Física.

No utilizar un contexto únicamente para disfrazar una sustitución directa.

---

# 19. Datos realistas

Cuando un ejercicio represente una situación real, utilizar valores
razonablemente realistas.

Si se adopta una simplificación importante debe quedar claro cuando sea
necesario.

Por ejemplo:

    desprecie la resistencia del aire;
    considere la cuerda ideal;
    suponga constante la aceleración;
    modele el objeto como una partícula.

No exigir al estudiante que adivine una hipótesis indispensable para resolver
un ejercicio básico o intermedio.

En problemas avanzados puede pedirse explícitamente que identifique las
hipótesis necesarias.

---

# 20. Datos innecesarios

Los datos innecesarios pueden utilizarse deliberadamente en algunos ejercicios
avanzados para desarrollar la capacidad de identificar información relevante.

No deben utilizarse de manera sistemática en los niveles básico e intermedio.

Si se incluyen, deben tener una finalidad pedagógica clara.

---

# 21. Sistemas de referencia

Cuando el problema involucre movimiento, fuerzas, campos u otras magnitudes
vectoriales, debe establecerse o construirse un sistema de referencia.

En la solución desarrollada debe quedar claro, cuando corresponda:

- origen;
- ejes;
- sentido positivo;
- posición inicial;
- orientación angular.

Los signos deben interpretarse respecto de ese sistema.

No cambiar de convención durante una solución sin indicarlo explícitamente.

---

# 22. Vectores

Los ejercicios vectoriales deben distinguir claramente entre:

- vector;
- magnitud;
- componentes;
- dirección;
- sentido.

No sumar magnitudes vectoriales como si fueran escalares.

La respuesta debe incluir dirección y sentido cuando sean necesarios para
describir completamente la magnitud solicitada.

---

# 23. Componentes rectangulares

En problemas vectoriales de dos o tres dimensiones, el método general preferido
es el uso de componentes rectangulares.

En dos dimensiones puede utilizarse:

    \[
    \vect{A}=A_x\ihat+A_y\jhat.
    \]

Las componentes deben obtenerse respetando el sistema de referencia y el
cuadrante.

La resultante se construye mediante:

    \[
    R_x=\sum A_x,
    \qquad
    R_y=\sum A_y.
    \]

Luego:

    \[
    R=\sqrt{R_x^2+R_y^2}.
    \]

La dirección debe determinarse teniendo en cuenta el cuadrante correcto.

No asignar signos a seno o coseno mecánicamente.

Los signos proceden de la orientación de las componentes respecto de los ejes.

---

# 24. Métodos geométricos alternativos

La ley de senos, la ley de cosenos u otros métodos geométricos pueden utilizarse
cuando sean apropiados.

Sin embargo, en problemas generales de suma de varios vectores debe preferirse
el método de componentes rectangulares.

Si se presenta un método alternativo debe explicarse:

- por qué es válido;
- qué ángulo debe utilizarse;
- cómo se interpretan los signos;
- qué limitaciones posee;
- cuándo resulta más conveniente.

No mezclar sin explicación convenciones geométricas y convenciones de
componentes.

---

# 25. Diagramas

Debe incluirse un esquema cuando facilite significativamente la comprensión del
problema.

Puede ser especialmente útil en:

- vectores;
- fuerzas;
- movimiento;
- trayectorias;
- campos;
- superficies gaussianas;
- circuitos;
- óptica;
- ondas;
- termodinámica.

El diagrama debe ser coherente con el enunciado y con la solución.

No incluir figuras decorativas.

---

# 26. Diagramas de cuerpo libre

Cuando un problema de dinámica lo requiera, debe utilizarse un diagrama de
cuerpo libre.

Debe mostrar únicamente las fuerzas externas que actúan sobre el cuerpo
aislado.

No incluir:

- velocidad como si fuera una fuerza;
- aceleración como si fuera una fuerza;
- fuerzas que el cuerpo ejerce sobre otros objetos;
- fuerzas inexistentes destinadas a explicar el movimiento.

El sistema de ejes debe definirse claramente.

---

# 27. Gráficas

Los ejercicios pueden pedir:

- interpretar una gráfica;
- construir una gráfica;
- obtener información de una pendiente;
- obtener información de un área;
- comparar gráficas;
- identificar una gráfica compatible con una situación.

Toda gráfica debe rotular:

- ejes;
- magnitudes;
- unidades cuando correspondan;
- escalas relevantes.

La solución debe interpretar físicamente la información gráfica.

---

# 28. Pendientes y áreas

Cuando se utilicen gráficas debe distinguirse entre significado geométrico y
significado físico.

Ejemplos:

    pendiente de x-t
    → velocidad

    pendiente de v-t
    → aceleración

    área algebraica bajo v-t
    → desplazamiento

    área algebraica bajo a-t
    → cambio de velocidad

No utilizar estas relaciones sin explicar sus condiciones y signos cuando sean
relevantes.

---

# 29. Unidades

Todos los cálculos deben mantener unidades coherentes.

Utilizar prioritariamente el Sistema Internacional.

Cuando sea necesaria una conversión, debe mostrarse explícitamente en la
solución si constituye un paso relevante.

No mezclar unidades incompatibles dentro de una ecuación.

El resultado final debe incluir la unidad correspondiente, salvo en magnitudes
adimensionales.

---

# 30. Análisis dimensional

Cuando resulte útil, la solución puede comprobar la homogeneidad dimensional de
una expresión.

Esto es especialmente recomendable cuando:

- se deduce una ecuación;
- se obtiene una relación no evidente;
- existe riesgo de error algebraico;
- el ejercicio solicita verificar una expresión.

El análisis dimensional no sustituye la justificación física.

---

# 31. Cifras significativas

Los resultados numéricos deben expresarse con una precisión razonable.

No presentar un número excesivo de cifras decimales cuando los datos no lo
justifiquen.

Durante cálculos intermedios pueden conservarse cifras adicionales para evitar
errores de redondeo.

El redondeo principal debe realizarse al presentar el resultado final.

---

# 32. Constantes físicas

Cuando un ejercicio requiera una constante física, debe utilizarse un valor
coherente con el resto del proyecto.

No utilizar diferentes valores de una constante dentro del mismo conjunto de
ejercicios sin una razón explícita.

Cuando la precisión exacta sea relevante, consultar la fuente correspondiente.

Cuando se utilice una aproximación pedagógica, mantenerla consistentemente.

---

# 33. Valores de la aceleración gravitatoria

En problemas próximos a la superficie terrestre debe mantenerse una convención
coherente para \(g\).

Si el ejercicio utiliza:

    \[
    g=\SI{9.8}{\metre\per\second\squared}
    \]

o:

    \[
    g=\SI{9.81}{\metre\per\second\squared},
    \]

la solución debe utilizar el mismo valor.

Puede emplearse:

    \[
    g=\SI{10}{\metre\per\second\squared}
    \]

únicamente cuando se indique explícitamente o cuando exista una decisión
pedagógica deliberada.

---

# 34. Signos

Los signos deben tratarse físicamente.

No utilizar reglas simplistas como:

    aceleración negativa = desaceleración

En movimiento rectilíneo debe analizarse la relación entre velocidad y
aceleración.

En general:

    velocidad y aceleración con el mismo signo
    → aumenta la rapidez

    velocidad y aceleración con signos opuestos
    → disminuye la rapidez

Los signos dependen del sistema de referencia elegido.

---

# 35. Direcciones y sentidos

Cuando el resultado sea vectorial debe indicarse, cuando corresponda:

- magnitud;
- dirección;
- sentido;
- componentes.

No considerar completa una respuesta vectorial si solo se proporciona un número
positivo y el problema requiere orientación.

---

# 36. Ángulos

Los ángulos deben definirse respecto de un eje o dirección claramente
identificada.

No escribir simplemente:

    \[
    \theta=30^\circ
    \]

si no está claro desde qué dirección se mide.

En problemas vectoriales debe verificarse cuidadosamente el cuadrante.

Cuando se utilice una función trigonométrica inversa, no debe confiarse
ciegamente en el valor principal de la calculadora.

---

# 37. Modelos físicos

La solución debe identificar el modelo físico cuando sea relevante.

Ejemplos:

- partícula;
- movimiento con aceleración constante;
- caída libre;
- resorte ideal;
- carga puntual;
- campo uniforme;
- cuerpo rígido;
- sistema aislado.

No utilizar una ecuación sin comprobar que el modelo correspondiente sea
aplicable.

---

# 38. Hipótesis

Las hipótesis necesarias deben indicarse en la solución cuando sean importantes.

Por ejemplo:

- resistencia del aire despreciable;
- aceleración constante;
- cuerda ideal;
- polea ideal;
- masa constante;
- superficie sin rozamiento;
- carga puntual;
- campo uniforme.

En ejercicios avanzados puede pedirse al estudiante que identifique las
hipótesis.

---

# 39. Aproximaciones

Cuando se utilice una aproximación debe quedar claro:

- cuál es;
- por qué puede utilizarse;
- qué efecto se está despreciando;
- bajo qué condiciones es razonable.

No utilizar aproximaciones ocultas que modifiquen significativamente la Física
del problema.

---

# 40. Respuesta breve

Cada ejercicio debe incluir una respuesta breve mediante el entorno:

    \begin{respuesta}
    ...
    \end{respuesta}

La respuesta debe proporcionar el resultado necesario para comprobar el
ejercicio sin reproducir toda la solución.

Puede incluir:

- valor numérico;
- unidad;
- signo;
- dirección;
- sentido;
- relación simbólica;
- conclusión conceptual.

Debe ser suficientemente completa para saber si el resultado es correcto.

---

# 41. Explicación desarrollada

Cada ejercicio debe incluir una solución desarrollada mediante:

    \begin{explicacion}
    ...
    \end{explicacion}

La explicación debe mostrar el razonamiento físico necesario para llegar al
resultado.

No debe limitarse a repetir la respuesta.

No debe reducirse a sustituir números en una fórmula sin explicar por qué se
utiliza.

---

# 42. Estructura general de una solución

Cuando corresponda, la explicación debe incluir:

1. datos;
2. incógnitas;
3. esquema;
4. sistema de referencia;
5. conversiones;
6. modelo físico;
7. hipótesis;
8. principio o ley;
9. ecuaciones;
10. despeje;
11. sustitución;
12. cálculo;
13. unidades;
14. cifras significativas;
15. signo;
16. dirección y sentido;
17. resultado final;
18. interpretación física;
19. verificación.

No todos los ejercicios necesitan mostrar formalmente los diecinueve pasos.

La estructura debe adaptarse al problema.

No convertir una solución sencilla en un procedimiento burocrático.

---

# 43. Datos

Cuando facilite la comprensión, comenzar la solución identificando los datos.

Por ejemplo:

    \[
    v_0=\SI{12}{\metre\per\second},
    \qquad
    a=-\SI{9.8}{\metre\per\second\squared}.
    \]

No repetir innecesariamente todos los datos si el ejercicio es conceptual o
muy sencillo.

---

# 44. Incógnita

Debe quedar claro qué se busca.

Cuando existan varias preguntas, identificar las incógnitas relevantes.

Esto ayuda a seleccionar las relaciones físicas apropiadas.

---

# 45. Principio físico antes de la fórmula

Antes de utilizar una ecuación importante debe identificarse, cuando sea
relevante, el principio o modelo que la justifica.

Por ejemplo:

    Como el movimiento tiene aceleración constante, puede utilizarse...

o:

    Aplicamos conservación de la energía mecánica porque...

o:

    Por la segunda ley de Newton...

El estudiante debe aprender a seleccionar principios, no únicamente fórmulas.

---

# 46. Despeje antes de sustituir

Cuando sea pedagógicamente útil, realizar primero el despeje simbólico y después
sustituir los valores.

Preferir:

    \[
    t=\frac{v-v_0}{a}
    \]

y luego sustituir.

Esto permite:

- observar la estructura de la relación;
- reducir errores;
- verificar dimensiones;
- reutilizar el resultado.

No es necesario forzar un despeje separado en operaciones triviales.

---

# 47. Sustitución

La sustitución debe mostrar con claridad qué valor corresponde a cada variable.

No escribir largas cadenas numéricas sin conexión visible con la ecuación
física.

Mantener las unidades durante el cálculo cuando esto ayude a verificar la
coherencia.

---

# 48. Cálculo

Todos los resultados deben verificarse antes de entregar el archivo.

No confiar únicamente en cálculos mentales.

Cuando existan varias operaciones, comprobar independientemente:

- signos;
- potencias;
- raíces;
- funciones trigonométricas;
- conversiones;
- notación científica.

Los ejercicios creados para el proyecto deben tener soluciones correctas.

---

# 49. Interpretación del resultado

Cuando aporte valor, después del resultado debe explicarse qué significa
físicamente.

Por ejemplo:

- por qué el signo es negativo;
- qué indica la dirección;
- si el objeto está ascendiendo o descendiendo;
- si la rapidez aumenta o disminuye;
- por qué una fuerza apunta en determinado sentido;
- si el valor obtenido es razonable;
- qué implica el resultado respecto del sistema.

No terminar todos los ejercicios automáticamente con una frase genérica.

La interpretación debe aportar información real.

---

# 50. Verificación física

Cuando corresponda, comprobar:

- unidades;
- dimensiones;
- signo;
- dirección;
- orden de magnitud;
- caso límite;
- consistencia con el enunciado;
- coherencia con el modelo.

Preguntas útiles:

    ¿el resultado tiene las unidades correctas?
    ¿el signo concuerda con el sistema de referencia?
    ¿la magnitud es físicamente razonable?
    ¿el resultado satisface las condiciones iniciales?
    ¿recupera un caso conocido?

---

# 51. Soluciones conceptuales

Un ejercicio conceptual también debe incluir explicación.

No basta con responder:

    Sí.

o:

    No.

La explicación debe justificar la conclusión mediante principios físicos.

Puede ser breve si el razonamiento es sencillo.

---

# 52. Soluciones de gráficas

Cuando el ejercicio utilice una gráfica, la solución debe interpretar la
información física de la gráfica.

No limitarse a leer coordenadas.

Debe explicarse, según corresponda:

- pendiente;
- área;
- interceptos;
- máximos;
- mínimos;
- signos;
- cambios de comportamiento.

---

# 53. Soluciones vectoriales

En problemas vectoriales la explicación debe mostrar las componentes necesarias.

Una estructura típica es:

    \[
    \vect{A}=A_x\ihat+A_y\jhat,
    \]

    \[
    \vect{B}=B_x\ihat+B_y\jhat,
    \]

    \[
    \vect{R}=\vect{A}+\vect{B},
    \]

    \[
    R_x=A_x+B_x,
    \qquad
    R_y=A_y+B_y.
    \]

Luego:

    \[
    R=\sqrt{R_x^2+R_y^2}.
    \]

La dirección debe determinarse respetando el cuadrante.

No ocultar los signos de las componentes.

---

# 54. Fuerzas eléctricas y campos eléctricos

En problemas de electricidad con varias cargas, debe prestarse especial
atención a:

- signo de cada carga;
- posición de cada carga;
- vector de separación;
- distancia;
- dirección de la fuerza o del campo;
- sentido determinado por atracción o repulsión;
- componentes rectangulares;
- superposición.

No asignar el signo de la carga directamente a una magnitud escalar de fuerza.

La dirección y el sentido deben surgir del análisis vectorial.

---

# 55. Posiciones dadas mediante coordenadas

Cuando las posiciones se proporcionen mediante coordenadas, debe preferirse una
formulación vectorial clara.

Por ejemplo, si una fuente está en \((x_q,y_q)\) y el punto de observación en
\((x_P,y_P)\), construir:

    \[
    \vect{r}=(x_P-x_q)\ihat+(y_P-y_q)\jhat.
    \]

Luego:

    \[
    r=\norm{\vect{r}}.
    \]

y el vector unitario:

    \[
    \hat{r}=\frac{\vect{r}}{r}.
    \]

Este procedimiento reduce ambigüedades de dirección y debe preferirse cuando
las coordenadas formen parte natural del problema.

---

# 56. Conservación

Cuando se utilice un principio de conservación debe identificarse:

- el sistema;
- la magnitud conservada;
- las condiciones que permiten aplicar la conservación;
- estados inicial y final.

No utilizar automáticamente una ecuación de conservación sin comprobar las
condiciones físicas.

---

# 57. Energía

En problemas de energía debe distinguirse entre:

- trabajo;
- energía cinética;
- energía potencial;
- energía mecánica;
- transferencia de energía;
- fuerzas conservativas;
- fuerzas no conservativas.

No utilizar conservación de energía mecánica si existen transferencias o fuerzas
no conservativas relevantes sin incorporarlas correctamente.

---

# 58. Dinámica

En problemas de dinámica debe:

1. identificar el cuerpo o sistema;
2. construir el diagrama de cuerpo libre;
3. elegir ejes;
4. descomponer fuerzas cuando corresponda;
5. aplicar la segunda ley de Newton por componentes.

Por ejemplo:

    \[
    \sum F_x=ma_x,
    \qquad
    \sum F_y=ma_y.
    \]

No comenzar directamente con ecuaciones sin identificar las fuerzas.

---

# 59. Cinemática

En problemas de cinemática debe identificarse primero:

- tipo de movimiento;
- sistema de referencia;
- posición inicial;
- velocidad inicial;
- aceleración;
- intervalo temporal.

No utilizar ecuaciones de aceleración constante cuando la aceleración no pueda
considerarse constante.

Debe diferenciarse entre:

- posición;
- desplazamiento;
- distancia;
- velocidad;
- rapidez;
- aceleración.

---

# 60. Caída libre y movimiento vertical

En problemas de caída libre debe definirse explícitamente el eje vertical.

Si se elige hacia arriba como positivo:

    \[
    a_y=-g.
    \]

Si se elige hacia abajo como positivo:

    \[
    a_y=+g.
    \]

Ambas elecciones son válidas si se mantienen consistentemente.

No memorizar reglas independientes de signos para subida y bajada.

La aceleración gravitatoria mantiene su dirección mientras se conserve el mismo
modelo y sistema de referencia.

---

# 61. Pistas

Las pistas pueden utilizarse cuando tengan valor pedagógico.

Deben ayudar a iniciar el razonamiento sin revelar la solución.

Una pista adecuada puede:

- sugerir qué principio considerar;
- recordar una representación útil;
- señalar que debe elegirse un sistema de referencia;
- sugerir que se construya un diagrama;
- indicar que deben utilizarse componentes.

No debe proporcionar directamente:

- la ecuación final ya despejada;
- el resultado;
- todos los pasos de solución.

---

# 62. Uso de pistas según dificultad

Las pistas son especialmente útiles en ejercicios básicos e intermedios.

En ejercicios avanzados deben reducirse o eliminarse para exigir mayor
autonomía.

No debe aplicarse una regla mecánica.

Un ejercicio avanzado puede incluir una pista si el objetivo principal se
encuentra después de un obstáculo secundario que no se desea evaluar.

---

# 63. Respuesta y explicación para todos los ejercicios

Todo ejercicio definitivo debe tener:

    ejercicio
    respuesta
    explicacion

salvo que exista una razón pedagógica o técnica expresamente documentada.

No dejar ejercicios sin solución desarrollada en el archivo fuente únicamente
porque la versión del estudiante no la mostrará.

La ocultación se controla mediante el sistema de versiones.

---

# 64. Sistema de versiones

Debe utilizarse un único `ejercicios.tex`.

El sistema de versiones controla qué contenido aparece en cada salida.

Conceptualmente:

    estudiante
    → ejercicio
    → pista cuando corresponda

    respuestas
    → ejercicio
    → pista cuando corresponda
    → respuesta

    docente
    → ejercicio
    → pista cuando corresponda
    → respuesta
    → explicación

No crear tres copias diferentes del conjunto de ejercicios.

---

# 65. Numeración común

El mismo ejercicio debe conservar el mismo número en:

- estudiante;
- respuestas;
- docente.

La ocultación de respuestas y explicaciones no debe modificar la numeración.

No duplicar enunciados para resolver problemas de versiones.

---

# 66. Código fuente habitual

La estructura conceptual de cada ejercicio debe ser:

    \begin{ejercicio}
    Enunciado.
    \end{ejercicio}

    \begin{respuesta}
    Respuesta breve.
    \end{respuesta}

    \begin{explicacion}
    Solución desarrollada.
    \end{explicacion}

Si el sistema dispone de un mecanismo específico para pistas, debe utilizarse
de acuerdo con la configuración vigente.

No inventar nuevos entornos sin comprobar primero `config/entornos.tex` y
`config/versiones.tex`.

---

# 67. No duplicar enunciados

El enunciado debe aparecer una sola vez en el código fuente.

No crear:

    ejercicio_estudiante
    ejercicio_respuestas
    ejercicio_docente

con el mismo enunciado repetido.

La arquitectura debe permitir corregir un ejercicio una sola vez.

---

# 68. Código LaTeX

`ejercicios.tex` es un fragmento de contenido.

No debe contener normalmente:

    \documentclass
    \begin{document}
    \end{document}

Debe utilizar los comandos, colores, estilos y entornos globales.

No redefinir localmente la configuración general.

---

# 69. Secciones por nivel

Cuando la estructura vigente lo permita, los niveles deben quedar claramente
identificados.

Puede utilizarse la convención existente del proyecto mediante comandos como:

    \nivelbasico
    \nivelintermedio
    \nivelavanzado

si estos se encuentran definidos en la configuración.

No inventar una nueva convención si ya existe una solución global.

---

# 70. Imágenes en ejercicios

Una imagen necesaria para comprender el enunciado debe formar parte del
contenido visible en todas las versiones.

Una imagen que pertenezca exclusivamente a la solución puede colocarse dentro
de la explicación correspondiente.

Las imágenes específicas del tema deben almacenarse normalmente en:

    imagenes/

dentro de la carpeta correspondiente.

---

# 71. TikZ y diagramas generados

Cuando un esquema pueda construirse claramente mediante TikZ puede utilizarse
esta herramienta.

Los diagramas deben ser:

- simples;
- legibles;
- físicamente correctos;
- coherentes con el texto;
- compatibles con la compilación del proyecto.

No utilizar diagramas excesivamente elaborados si una figura sencilla comunica
mejor la situación.

---

# 72. No dar pistas involuntarias mediante figuras

Una figura incluida en el enunciado no debe revelar accidentalmente la
respuesta.

Por ejemplo, si se pregunta por la dirección de una fuerza resultante, no debe
dibujarse ya la resultante con su dirección exacta salvo que esa información
forme parte del problema.

Las figuras deben proporcionar la información necesaria, no resolver el
ejercicio.

---

# 73. Originalidad

Los ejercicios finales del proyecto deben redactarse de forma original.

Las fuentes bibliográficas pueden utilizarse para estudiar:

- tipos de problemas;
- progresión;
- nivel de dificultad;
- aplicaciones;
- estrategias;
- cobertura conceptual.

No copiar mecánicamente grandes conjuntos de ejercicios de una fuente.

Puede conservarse una situación física clásica cuando sea pedagógicamente útil,
pero el enunciado y el desarrollo deben integrarse coherentemente en la obra.

---

# 74. Uso de las fuentes bibliográficas

Antes de crear una colección importante de ejercicios debe revisarse el
tratamiento del tema en las fuentes pertinentes de `libros/`.

La consulta puede utilizarse para comparar:

- tipos de ejercicios;
- secuencia de dificultad;
- problemas conceptuales;
- aplicaciones;
- métodos;
- profundidad;
- nivel matemático;
- cobertura.

No es necesario utilizar todos los libros para cada tema.

Debe seleccionarse material relevante.

---

# 75. Fuentes principales

Las fuentes principales pueden utilizarse especialmente para estudiar:

- rigor de los problemas;
- variedad;
- progresión;
- integración conceptual;
- aplicaciones;
- métodos de solución.

Entre las fuentes principales del proyecto se encuentran:

    Sears–Zemansky / Young–Freedman
    Serway–Jewett
    Schaum / Bueche–Hecht
    Bauer–Westfall

Schaum puede ser especialmente útil para observar granularidad y variedad de
problemas.

Las fuentes universitarias pueden aportar problemas de integración conceptual y
métodos más profundos.

---

# 76. Fuentes complementarias

Las fuentes complementarias pueden ser especialmente útiles para:

- problemas introductorios;
- progresión escolar;
- aplicaciones sencillas;
- contextualización;
- ejercicios básicos e intermedios.

Entre ellas pueden encontrarse:

    Serway–Vuille
    Walter Pérez Terrel
    Juan A. Cuéllar
    Hipertexto Física
    Investiguemos Física

Los problemas seleccionados como inspiración deben evaluarse con el mismo
criterio de exactitud física y matemática.

---

# 77. No copiar errores de las fuentes

Las fuentes son referencias, no autoridades infalibles.

Todo ejercicio utilizado como inspiración debe comprobarse.

Si una fuente presenta:

- error numérico;
- signo incorrecto;
- ambigüedad;
- unidad incorrecta;
- notación inconsistente;
- solución incompleta;

el proyecto debe corregirlo.

No conservar un error por fidelidad a la fuente.

---

# 78. Creación de nuevos ejercicios

Al crear un ejercicio nuevo debe comprobarse antes de incorporarlo:

1. que el enunciado sea resoluble;
2. que contenga la información necesaria;
3. que no tenga contradicciones;
4. que el modelo físico sea coherente;
5. que los valores sean razonables;
6. que exista una solución clara;
7. que el resultado sea físicamente posible;
8. que el nivel asignado sea adecuado;
9. que aporte algo distinto al conjunto;
10. que pueda resolverse con los conocimientos desarrollados.

No generar grandes cantidades de ejercicios sin verificarlos individualmente.

---

# 79. Verificación numérica

Todo ejercicio numérico debe calcularse y comprobarse antes de considerarse
terminado.

La verificación debe incluir:

- operaciones;
- signos;
- unidades;
- conversiones;
- cifras significativas;
- funciones trigonométricas;
- potencias;
- raíces;
- notación científica.

Cuando el problema sea suficientemente complejo, realizar una comprobación
independiente del resultado.

---

# 80. Verificación simbólica

Las deducciones y resultados simbólicos deben comprobarse mediante:

- sustitución;
- dimensiones;
- casos particulares;
- casos límite;
- comparación con relaciones conocidas;

cuando corresponda.

No considerar correcta una expresión únicamente porque el álgebra parezca
plausible.

---

# 81. Verificación de vectores

En resultados vectoriales comprobar:

- signos de componentes;
- cuadrante;
- magnitud;
- dirección;
- sentido;
- unidad.

Cuando sea posible, verificar que la resultante tenga una orientación coherente
con la geometría del problema.

---

# 82. Verificación de gráficas

En ejercicios gráficos comprobar:

- variables;
- unidades;
- escalas;
- pendientes;
- áreas;
- signos;
- puntos característicos;
- coherencia con las ecuaciones.

Una gráfica incorrecta invalida pedagógicamente el ejercicio aunque el cálculo
numérico sea correcto.

---

# 83. Verificación de diagramas

Comprobar que los diagramas:

- correspondan al enunciado;
- utilicen el mismo sistema de referencia;
- muestren correctamente los vectores;
- no incluyan información contradictoria;
- tengan etiquetas legibles;
- no revelen accidentalmente la solución.

---

# 84. Dificultad real

Antes de asignar un nivel debe preguntarse:

    ¿qué decisión física debe tomar el estudiante?

Un ejercicio es básico si la relación principal está prácticamente determinada.

Es intermedio si debe combinar información o seleccionar entre varias
relaciones.

Es avanzado si debe modelar, elegir principios, integrar conceptos o justificar
decisiones de forma autónoma.

No clasificar por apariencia.

---

# 85. Evitar dificultad artificial

No aumentar la dificultad mediante:

- números excesivamente incómodos;
- cantidades innecesarias de conversiones;
- textos deliberadamente confusos;
- datos ocultos sin razón;
- álgebra larga sin contenido físico;
- geometría complicada irrelevante.

La dificultad debe provenir principalmente de la Física.

---

# 86. Evitar ejercicios repetitivos

Dos ejercicios son demasiado similares si únicamente cambian:

- nombres;
- números;
- unidades;
- objetos;

pero exigen exactamente el mismo razonamiento.

Puede haber cierta repetición deliberada en el nivel básico para consolidar una
habilidad, pero el conjunto completo debe avanzar.

---

# 87. Preguntas de interpretación

Los problemas numéricos pueden incluir preguntas adicionales como:

- ¿qué significa el signo obtenido?
- ¿en qué dirección ocurre el movimiento?
- ¿aumenta o disminuye la rapidez?
- ¿qué variable influye más?
- ¿es razonable el resultado?
- ¿qué ocurriría si se duplica una magnitud?
- ¿qué hipótesis se utilizó?

Estas preguntas ayudan a conectar cálculo y comprensión.

No añadirlas mecánicamente a todos los ejercicios.

---

# 88. Comparación de situaciones

Los ejercicios comparativos son útiles para evitar aprendizaje mecánico.

Pueden pedir comparar:

- dos masas;
- dos velocidades;
- dos trayectorias;
- dos campos;
- dos configuraciones de cargas;
- dos resortes;
- dos sistemas térmicos;
- dos circuitos.

La comparación debe fundamentarse en una relación física.

---

# 89. Variación de parámetros

Cuando sea útil, pedir cómo cambia un resultado si se modifica una variable.

Por ejemplo:

    si la distancia se duplica,
    ¿cómo cambia la fuerza?

Este tipo de ejercicio desarrolla comprensión funcional y proporcional.

No exigir siempre un nuevo cálculo numérico si la relación puede analizarse
conceptualmente.

---

# 90. Casos límite

En niveles intermedio y avanzado pueden utilizarse preguntas de casos límite.

Por ejemplo:

- ¿qué ocurre si una masa tiende a cero?
- ¿qué ocurre si una distancia aumenta mucho?
- ¿qué ocurre si desaparece el rozamiento?
- ¿qué ocurre si el ángulo es cero?
- ¿qué ocurre si dos cargas tienen igual magnitud?

Los casos límite deben utilizarse para comprobar comprensión, no como
formalismo vacío.

---

# 91. Estimaciones

Cuando el tema lo permita pueden incluirse ejercicios de estimación.

Estos desarrollan:

- órdenes de magnitud;
- modelado;
- selección de datos razonables;
- análisis crítico.

La solución debe explicar las hipótesis utilizadas.

No exigir una precisión incompatible con el carácter estimativo del problema.

---

# 92. Análisis experimental

En niveles intermedio o avanzado pueden incluirse problemas basados en datos
experimentales.

Pueden pedir:

- construir una gráfica;
- identificar una relación;
- calcular una pendiente;
- determinar una constante;
- comparar teoría y experimento;
- interpretar desviaciones;
- estimar incertidumbres cuando corresponda al nivel.

El ejercicio debe mantener el foco en la Física.

---

# 93. Errores experimentales e incertidumbre

Cuando el tema y el nivel lo justifiquen, pueden incluirse ejercicios sobre:

- incertidumbre;
- precisión;
- exactitud;
- propagación sencilla;
- comparación de resultados.

No introducir formalismo estadístico innecesario si no forma parte del
desarrollo previsto.

---

# 94. Problemas abiertos

Algunos ejercicios avanzados pueden admitir más de una estrategia o más de una
respuesta razonable bajo diferentes hipótesis.

En esos casos el enunciado debe permitir justificar las decisiones.

La solución debe explicar:

- qué hipótesis se adoptan;
- por qué son razonables;
- cómo afectan el resultado.

No forzar una única respuesta si la Física del problema admite varias bajo
modelos diferentes.

---

# 95. Problemas imposibles o insuficientes

Puede ser pedagógicamente útil incluir algún ejercicio en el que el estudiante
deba determinar que:

- faltan datos;
- el modelo no es aplicable;
- la información es contradictoria;
- la situación propuesta es físicamente imposible.

Este tipo de ejercicio debe utilizarse principalmente en niveles superiores y
con intención clara.

La solución debe explicar por qué no puede obtenerse el resultado solicitado.

---

# 96. Métodos alternativos

Cuando un problema admita dos métodos relevantes, la explicación puede mostrar
ambos si esto aporta comprensión.

Por ejemplo:

    dinámica vs. energía
    cinemática vs. energía
    componentes vs. geometría
    integración vs. ecuación conocida

No mostrar soluciones alternativas únicamente para aumentar la extensión.

Debe quedar claro qué método resulta más general, directo o ilustrativo.

---

# 97. Selección del método

En ejercicios avanzados debe desarrollarse la capacidad de elegir el método.

No indicar siempre:

    use conservación de energía

o:

    aplique la segunda ley de Newton

si precisamente la selección del principio forma parte del aprendizaje.

En ejercicios básicos e intermedios puede proporcionarse mayor orientación.

---

# 98. No ocultar pasos conceptualmente importantes

La explicación desarrollada no debe saltar desde los datos hasta el resultado
mediante una fórmula sin justificar.

Debe mostrarse especialmente:

- elección del sistema;
- selección del modelo;
- principio físico;
- signos;
- descomposición vectorial;
- hipótesis;
- ecuaciones relevantes.

Los pasos puramente aritméticos triviales pueden compactarse.

---

# 99. No sobreexplicar operaciones elementales

Una solución desarrollada no significa describir verbalmente cada operación
aritmética.

Evitar frases como:

    ahora multiplicamos por 2;
    luego dividimos entre 3;

si estas operaciones son evidentes y no aportan comprensión física.

La explicación debe concentrarse en los pasos conceptualmente importantes.

---

# 100. Claridad de la solución

La solución debe poder seguirse sin necesidad de adivinar pasos.

Las ecuaciones deben aparecer en un orden lógico.

No introducir símbolos nuevos sin definirlos.

No cambiar de notación durante el procedimiento.

No mezclar diferentes convenciones de signos.

---

# 101. Resultado final

El resultado principal debe quedar claramente identificable.

Debe incluir, según corresponda:

- valor;
- unidad;
- signo;
- dirección;
- sentido.

Puede destacarse utilizando los mecanismos ya existentes en el proyecto si
corresponde.

No introducir un estilo local nuevo únicamente para resaltar resultados.

---

# 102. Interpretación y respuesta breve

La `respuesta` y la conclusión de la `explicacion` deben ser coherentes.

Si durante la revisión cambia un resultado, deben actualizarse ambas.

Este punto debe comprobarse especialmente después de corregir cálculos.

No permitir que la respuesta breve conserve un valor antiguo mientras la
explicación contiene otro.

---

# 103. Coherencia entre apartados

En ejercicios con apartados:

    a)
    b)
    c)

debe comprobarse que los resultados intermedios utilizados posteriormente sean
correctos.

Si un apartado depende del anterior, la explicación debe dejar clara esa
dependencia.

Cuando sea posible, evitar que un pequeño error numérico inicial haga
imposibles todos los apartados posteriores.

---

# 104. Independencia pedagógica

Un ejercicio puede utilizar resultados obtenidos anteriormente dentro del mismo
problema, pero el conjunto completo no debe depender excesivamente de haber
resuelto ejercicios anteriores.

Cada ejercicio debe ser suficientemente independiente para utilizarse de forma
selectiva en una clase o tarea, salvo que se haya diseñado deliberadamente una
secuencia.

---

# 105. Uso en clase

Los ejercicios deben ser útiles tanto para estudio individual como para
enseñanza.

Dentro del conjunto deben existir problemas adecuados para:

- explicación guiada;
- práctica en clase;
- trabajo individual;
- tarea;
- discusión conceptual;
- profundización.

No es necesario etiquetar cada ejercicio con estos usos salvo que se adopte
posteriormente una convención específica.

---

# 106. Uso de calculadora

Los ejercicios pueden requerir calculadora cuando la Física lo justifique.

No diseñar la dificultad alrededor de operaciones numéricas tediosas.

Cuando el razonamiento pueda realizarse simbólicamente antes de calcular,
preferir esa estrategia.

---

# 107. Notación científica

Utilizar notación científica cuando resulte apropiada, especialmente en:

- electricidad;
- física atómica;
- astronomía;
- constantes físicas;
- escalas microscópicas;
- escalas muy grandes.

Las soluciones deben manejar correctamente potencias de diez y prefijos SI.

---

# 108. Prefijos SI

Debe comprobarse especialmente la conversión de prefijos como:

    kilo
    mega
    giga
    centi
    mili
    micro
    nano
    pico

Errores de prefijos pueden cambiar un resultado por varios órdenes de magnitud.

Las soluciones deben mostrar conversiones cuando sean pedagógicamente
relevantes.

---

# 109. Homogeneidad de notación

Antes de finalizar un conjunto comprobar que no se alternen arbitrariamente
símbolos para una misma magnitud.

Por ejemplo, evitar utilizar en ejercicios consecutivos:

    x_i
    x_0
    x_{\mathrm{inicial}}

sin una razón pedagógica.

La notación debe seguir preferentemente la teoría del tema.

---

# 110. Terminología

Los enunciados y soluciones deben utilizar la terminología correcta.

Distinguir, por ejemplo:

- distancia y desplazamiento;
- rapidez y velocidad;
- masa y peso;
- fuerza y energía;
- campo y fuerza;
- potencial y energía potencial;
- calor y temperatura.

No utilizar términos coloquiales si introducen ambigüedad física.

---

# 111. Revisión lingüística

Antes de terminar deben revisarse:

- ortografía;
- puntuación;
- concordancia;
- claridad;
- símbolos;
- nombres de unidades.

Un enunciado ambiguo puede convertir un ejercicio físicamente correcto en un
mal problema.

---

# 112. Revisión de LaTeX

Antes de considerar terminado `ejercicios.tex`, comprobar:

- apertura y cierre de entornos;
- delimitadores matemáticos;
- comandos;
- unidades;
- caracteres especiales;
- rutas de imágenes;
- TikZ;
- referencias;
- listas;
- tablas;
- numeración.

No asumir que un archivo compila porque una parte de él parece correcta.

---

# 113. Comprobación de las tres versiones

Después de modificaciones importantes debe comprobarse, cuando el entorno lo
permita:

    estudiante
    respuestas
    docente

Verificar que:

- el estudiante no vea respuestas;
- el estudiante no vea explicaciones;
- la versión de respuestas muestre las respuestas previstas;
- la versión de respuestas no muestre explicaciones docentes;
- la versión docente muestre todo;
- la numeración sea idéntica;
- los diagramas necesarios permanezcan visibles;
- no aparezcan espacios o encabezados extraños por contenido oculto.

---

# 114. Compilación

Cuando sea posible debe comprobarse la compilación desde los documentos
maestros correspondientes.

No es necesario convertir `ejercicios.tex` en un documento independiente.

Debe comprobarse especialmente:

- errores;
- warnings relevantes;
- overfull boxes;
- figuras;
- ecuaciones;
- saltos de página;
- cajas;
- listas;
- visibilidad de versiones.

---

# 115. Revisión visual

Cuando se genere una salida de prueba debe revisarse visualmente.

Comprobar:

- legibilidad;
- separación entre ejercicios;
- ubicación de figuras;
- ecuaciones demasiado largas;
- cajas cortadas;
- saltos de página poco adecuados;
- títulos de nivel;
- consistencia tipográfica.

La compilación sin errores no garantiza una buena presentación.

---

# 116. Procedimiento antes de crear ejercicios nuevos

Antes de escribir un nuevo `ejercicios.tex` debe realizarse, como mínimo, el
siguiente proceso:

1. consultar `AGENTS.md`;
2. consultar `pendientes.md`;
3. consultar `instrucciones/ejercicios.md`;
4. consultar `instrucciones/teoria.md`;
5. consultar `instrucciones/formulario.md` cuando exista;
6. leer la teoría completa del tema;
7. revisar el formulario si ya existe;
8. identificar conceptos y habilidades que deben practicarse;
9. consultar las fuentes bibliográficas pertinentes;
10. observar tipos y progresión de problemas en las fuentes;
11. diseñar la distribución por niveles;
12. redactar ejercicios originales;
13. resolver todos los ejercicios;
14. comprobar resultados;
15. redactar respuestas breves;
16. redactar explicaciones desarrolladas;
17. revisar coherencia de notación;
18. revisar unidades;
19. revisar signos;
20. revisar diagramas y gráficas;
21. comprobar las versiones;
22. comprobar compilación cuando sea posible.

No generar primero una gran cantidad de enunciados para intentar resolverlos
después sin haber comprobado que todos sean válidos.

---

# 117. Diseño previo del conjunto

Antes de redactar puede elaborarse mentalmente o de forma temporal una matriz de
cobertura.

Por ejemplo:

    concepto                  básico   intermedio   avanzado
    definición                  ✓
    aplicación directa          ✓
    interpretación gráfica      ✓          ✓
    problema inverso                       ✓
    componentes                            ✓            ✓
    integración conceptual                              ✓
    deducción                                            ✓

Esta matriz no necesita aparecer en el archivo final.

Su función es evitar conjuntos desequilibrados.

---

# 118. Procedimiento para revisar ejercicios existentes

Cuando se solicite revisar un `ejercicios.tex` existente, no debe reescribirse
automáticamente desde cero.

Primero:

1. leer el archivo completo;
2. consultar la teoría correspondiente;
3. consultar el formulario correspondiente;
4. consultar las instrucciones vigentes;
5. identificar la estructura de niveles;
6. verificar cada enunciado;
7. verificar cada respuesta;
8. verificar cada explicación;
9. recalcular resultados;
10. comprobar unidades;
11. comprobar signos;
12. comprobar vectores;
13. comprobar diagramas;
14. comprobar dificultad;
15. comprobar cobertura;
16. comprobar originalidad y variedad;
17. comprobar las tres versiones;
18. conservar el contenido correcto;
19. corregir únicamente lo necesario.

No sustituir ejercicios correctos únicamente por preferencia estilística.

---

# 119. Corrección de un ejercicio

Si se detecta un error debe corregirse de manera completa.

Revisar conjuntamente:

    enunciado
    respuesta
    explicación
    figura
    referencias posteriores

No corregir únicamente el número final si el error proviene del planteamiento.

Después de una corrección debe recalcularse el ejercicio completo.

---

# 120. Cambio de datos

Si se modifica un dato del enunciado deben recalcularse todos los resultados que
dependan de él.

No asumir que una pequeña modificación numérica afecta únicamente la respuesta
final.

Revisar:

- apartados;
- gráficas;
- diagramas;
- resultados intermedios;
- cifras significativas;
- interpretación.

---

# 121. Cambio de convención de signos

Si se cambia un sistema de referencia o una convención de signos debe revisarse
todo el ejercicio.

Comprobar:

- datos;
- componentes;
- ecuaciones;
- resultados;
- interpretación.

Dos soluciones con sistemas de referencia diferentes pueden ser igualmente
válidas si son internamente consistentes.

---

# 122. Criterio para considerar completo un ejercicio

Un ejercicio puede considerarse completo cuando:

- el enunciado es claro;
- es físicamente coherente;
- posee los datos necesarios;
- su nivel está bien asignado;
- aporta valor pedagógico;
- tiene respuesta;
- tiene explicación;
- los cálculos están comprobados;
- las unidades son correctas;
- los signos son correctos;
- las direcciones son correctas;
- las figuras son correctas;
- el resultado es razonable;
- la solución explica el razonamiento físico;
- es coherente con la teoría.

---

# 123. Criterio para considerar completo `ejercicios.tex`

El componente `ejercicios.tex` puede considerarse completo cuando:

- existe una progresión adecuada;
- los tres niveles están representados cuando corresponda;
- existe variedad;
- la cobertura conceptual es suficiente;
- todos los ejercicios tienen respuesta;
- todos los ejercicios tienen explicación;
- los resultados han sido verificados;
- las unidades han sido verificadas;
- los signos han sido verificados;
- los vectores han sido verificados;
- las gráficas y diagramas han sido revisados;
- la notación coincide con la teoría;
- el conjunto es coherente con el formulario;
- las tres versiones funcionan correctamente;
- la compilación ha sido comprobada cuando sea posible.

Solo después de cumplir estos criterios puede registrarse el componente como
completo en `pendientes.md`.

---

# 124. Relación entre dificultad y ayuda

La cantidad de ayuda debe disminuir progresivamente.

De forma general:

    básico
    → mayor orientación

    intermedio
    → orientación moderada

    avanzado
    → mayor autonomía

Esto puede reflejarse en:

- información proporcionada;
- pistas;
- subdivisión en apartados;
- indicación del método;
- cantidad de decisiones que debe tomar el estudiante.

No convertir esta progresión en una regla rígida.

---

# 125. Qué debe aprender el estudiante de una solución

La solución docente debe enseñar un método de razonamiento transferible.

El estudiante debería poder reconocer:

    qué sistema estudiar
    → qué datos son relevantes
    → qué modelo utilizar
    → qué principio aplicar
    → cómo representar la situación
    → cómo construir las ecuaciones
    → cómo resolverlas
    → cómo interpretar el resultado
    → cómo comprobarlo

La solución no debe enseñar únicamente a reproducir una secuencia de
operaciones.

---

# 126. Principio final

Los ejercicios deben enseñar a **hacer Física**, no únicamente a calcular.

Ante cualquier decisión de diseño debe priorizarse:

    exactitud física
    → exactitud matemática
    → comprensión conceptual
    → calidad del razonamiento
    → progresión de dificultad
    → claridad pedagógica
    → interpretación física
    → coherencia con la teoría
    → variedad
    → autonomía del estudiante

El objetivo final es que el estudiante avance desde:

    sé qué fórmula parece corresponder

hasta:

    comprendo el sistema,
    identifico el modelo,
    selecciono el principio físico,
    construyo la solución,
    verifico el resultado
    y puedo explicar qué significa físicamente.