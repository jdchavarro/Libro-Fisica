# Criterios para desarrollar la teoría

Este archivo establece los criterios específicos que deben seguirse al crear,
revisar, ampliar o corregir los archivos:

```text
teoria.tex
```

del proyecto de Física.

Las reglas generales del proyecto se encuentran en:

```text
AGENTS.md
```

Las decisiones de arquitectura y configuración LaTeX se encuentran en:

```text
instrucciones/configuracion.md
```

El estado actual del proyecto y el punto exacto de continuación se encuentran
en:

```text
pendientes.md
```

Este archivo no debe utilizarse para registrar progreso ni decisiones
estructurales generales.

Su función exclusiva es establecer **cómo debe desarrollarse la teoría de cada
tema**.

---

# 1. Objetivo de la teoría

La función principal de:

```text
teoria.tex
```

es **enseñar Física**.

La teoría constituye el material principal para comprender cada tema y debe
poder utilizarse simultáneamente como:

1. material de estudio autónomo para el estudiante;
2. base rigurosa para preparar una clase;
3. guion conceptual para impartir una clase;
4. referencia para construir posteriormente el formulario y los ejercicios.

No debe convertirse en una colección de:

- definiciones aisladas;
- fórmulas;
- propiedades;
- procedimientos;
- reglas de cálculo;
- ejemplos desconectados.

Debe construir comprensión física conectando, cuando corresponda:

- fenómenos;
- observaciones;
- conceptos;
- magnitudes;
- sistemas físicos;
- modelos;
- hipótesis;
- aproximaciones;
- principios;
- leyes;
- ecuaciones;
- matemáticas;
- representaciones escalares;
- representaciones vectoriales;
- diagramas;
- gráficas;
- experimentos;
- aplicaciones;
- ejemplos;
- problemas;
- temas anteriores;
- temas posteriores.

---

# 2. Preguntas que debe responder la teoría

Al terminar un tema, el lector debería poder responder, cuando corresponda:

- ¿qué fenómeno físico se está estudiando?
- ¿qué sistema físico se está analizando?
- ¿qué significa físicamente el concepto?
- ¿qué magnitudes intervienen?
- ¿cuáles son escalares y cuáles vectoriales?
- ¿qué símbolos y unidades se utilizan?
- ¿cómo se relacionan las magnitudes?
- ¿qué modelo físico se está empleando?
- ¿qué idealizaciones se realizan?
- ¿qué hipótesis se están suponiendo?
- ¿qué aproximaciones se utilizan?
- ¿qué principio o ley describe el fenómeno?
- ¿de dónde surge la ecuación?
- ¿qué representa cada término?
- ¿qué información física contiene la ecuación?
- ¿cuándo puede utilizarse?
- ¿cuándo deja de ser válida?
- ¿qué significa el signo?
- ¿qué significa la dirección?
- ¿qué significa el sentido?
- ¿cómo se representa gráficamente?
- ¿cómo se aplica a una situación concreta?
- ¿qué casos especiales existen?
- ¿qué errores de interpretación son frecuentes?
- ¿cómo se relaciona con conocimientos anteriores?
- ¿qué conceptos posteriores prepara?

No debe suponerse que el lector comprende una ecuación simplemente porque esta
ha sido presentada.

---

# 3. Principio pedagógico general

Siempre que sea posible, seguir la progresión:

```text
fenómeno
→ observación
→ pregunta física
→ interpretación intuitiva
→ concepto
→ magnitudes
→ modelo
→ principio o ley
→ relación física
→ ecuación
→ interpretación
→ representación
→ aplicación
→ generalización
```

No comenzar directamente con una fórmula cuando el fenómeno pueda construirse
conceptualmente primero.

Evitar como estructura dominante:

```text
fórmula
→ sustitución de números
→ resultado
```

La Física debe aparecer antes que la manipulación algebraica.

---

# 4. Función como guion de clase

La teoría debe poder utilizarse prácticamente como apoyo directo para impartir
una clase.

El desarrollo debe seguir un recorrido natural.

Cuando resulte apropiado, la secuencia puede ser:

1. presentar un fenómeno, observación o situación física;
2. formular una pregunta;
3. construir una interpretación intuitiva;
4. identificar el sistema que se estudiará;
5. identificar las magnitudes relevantes;
6. establecer el sistema de referencia;
7. introducir la notación;
8. definir los conceptos necesarios;
9. presentar el modelo físico;
10. indicar hipótesis e idealizaciones;
11. formular el principio o ley;
12. construir o deducir las ecuaciones;
13. interpretar físicamente cada término;
14. analizar unidades y dimensiones;
15. analizar signos;
16. analizar dirección y sentido cuando corresponda;
17. estudiar representaciones gráficas;
18. resolver ejemplos;
19. discutir casos especiales;
20. analizar condiciones de validez;
21. señalar errores frecuentes;
22. conectar con conocimientos anteriores;
23. conectar con conceptos posteriores;
24. cerrar con una síntesis.

Esta secuencia es una guía.

No debe convertirse en una plantilla rígida ni deben crearse apartados
artificiales únicamente para cumplirla.

---

# 5. Intuición antes del formalismo

Cuando un concepto sea abstracto, introducir primero una interpretación física
o intuitiva cuando esto facilite la comprensión.

Después presentar la formulación rigurosa.

Este criterio resulta especialmente importante en conceptos como:

- campo;
- flujo;
- potencial;
- energía;
- trabajo;
- cantidad de movimiento;
- impulso;
- momento angular;
- entropía;
- ondas;
- interferencia;
- campos electromagnéticos;
- relatividad;
- conceptos cuánticos.

La intuición debe ayudar a comprender.

No debe sustituir una definición correcta.

No utilizar analogías o explicaciones intuitivas que conduzcan a una
interpretación físicamente incorrecta.

---

# 6. Definiciones

Una definición debe establecer con precisión qué significa una magnitud o
concepto.

Cuando corresponda debe indicar:

- qué representa;
- cómo se determina;
- si es escalar o vectorial;
- símbolo;
- unidad SI;
- interpretación física.

Puede utilizarse:

```latex
\begin{definicion}[Nombre]
...
\end{definicion}
```

No introducir una definición mediante lenguaje ambiguo.

No presentar como definición algo que en realidad sea una ley, una propiedad,
una aproximación o una consecuencia.

---

# 7. Distinguir categorías físicas

Debe diferenciarse explícitamente, cuando sea relevante, entre:

```text
definición
principio
ley física
modelo
hipótesis
idealización
aproximación
consecuencia
relación matemática
ecuación general
caso particular
procedimiento
```

No llamar “ley” a cualquier ecuación.

No presentar una aproximación como si fuera una relación universal.

No presentar una definición como si hubiera sido deducida de una ley.

Los entornos definidos globalmente deben utilizarse según su significado
pedagógico.

---

# 8. Magnitudes físicas

Cuando se introduzca una magnitud importante debe quedar claro, cuando
corresponda:

- nombre;
- símbolo;
- significado físico;
- carácter escalar o vectorial;
- unidad SI;
- dimensiones;
- signo;
- dirección y sentido;
- forma de medición o determinación.

No introducir símbolos sin definirlos.

La notación debe mantenerse coherente con:

```text
formulario.tex
ejercicios.tex
```

del mismo tema.

---

# 9. Sistema de referencia

Cuando el fenómeno dependa de posiciones, velocidades, aceleraciones, fuerzas,
campos u otras magnitudes vectoriales debe definirse claramente el sistema de
referencia.

Cuando corresponda, establecer:

- origen;
- ejes;
- orientación;
- sentido positivo;
- vectores unitarios;
- posición inicial;
- convención angular.

Los signos deben interpretarse siempre en relación con este sistema.

No utilizar expresiones como:

```text
hacia arriba es positivo
```

sin haber establecido previamente la elección del eje.

La elección del sistema de referencia es una decisión del modelo, no una
propiedad absoluta del movimiento.

---

# 10. Escalares y vectores

Debe distinguirse claramente entre magnitudes escalares y vectoriales.

Cuando una magnitud sea vectorial debe considerarse, según corresponda:

- magnitud;
- dirección;
- sentido;
- componentes.

La notación debe respetar las convenciones globales del proyecto.

No sumar vectores como si fueran escalares.

No confundir la magnitud:

```latex
F
```

con el vector:

```latex
\vect{F}
```

cuando la distinción sea relevante.

---

# 11. Componentes rectangulares

Cuando un problema o desarrollo involucre varios vectores en dos o tres
dimensiones, el método general preferido es trabajar mediante componentes
rectangulares.

En dos dimensiones:

```latex
\vect{A}=A_x\ihat+A_y\jhat
```

con:

```latex
A_x=A\cos\theta,
\qquad
A_y=A\sin\theta
```

cuando el ángulo esté definido respecto del eje correspondiente.

La resultante debe construirse mediante:

```latex
R_x=\sum A_x,
\qquad
R_y=\sum A_y
```

y después:

```latex
R=\sqrt{R_x^2+R_y^2}.
```

La dirección debe obtenerse teniendo en cuenta el cuadrante correcto.

Métodos como:

- ley de senos;
- ley de cosenos;
- construcción geométrica;

pueden explicarse cuando aporten comprensión o resulten especialmente
convenientes, pero no deben sustituir el método vectorial general cuando el
objetivo sea construir un procedimiento reutilizable.

---

# 12. Modelos físicos

Cuando se utilice un modelo debe indicarse qué sistema real está siendo
representado y qué características se conservan o ignoran.

Ejemplos:

- partícula;
- cuerpo rígido;
- resorte ideal;
- gas ideal;
- fluido ideal;
- carga puntual;
- campo uniforme;
- onda armónica;
- sistema aislado;
- superficie gaussiana idealizada.

Debe quedar claro que un modelo es una representación útil del sistema físico,
no necesariamente una descripción exacta de toda su complejidad.

---

# 13. Hipótesis e idealizaciones

Cuando una deducción dependa de hipótesis deben indicarse.

Ejemplos:

```text
resistencia del aire despreciable
masa constante
aceleración constante
campo gravitatorio uniforme
resorte ideal
cuerda inextensible y sin masa
polea ideal
partícula puntual
sistema aislado
temperatura uniforme
```

No ocultar una hipótesis necesaria para obtener una ecuación.

---

# 14. Aproximaciones

Toda aproximación relevante debe identificarse como tal.

Debe explicarse:

- qué se aproxima;
- bajo qué condiciones;
- por qué resulta razonable;
- cuándo puede dejar de ser válida.

Ejemplos:

- \(g\) constante cerca de la superficie terrestre;
- pequeñas oscilaciones;
- ángulos pequeños;
- resistencia del aire despreciable;
- objeto tratado como partícula;
- campo aproximadamente uniforme.

No presentar una aproximación como una verdad universal.

---

# 15. Principios y leyes

Cuando se presente un principio o una ley debe explicarse:

- qué afirma;
- qué magnitudes relaciona;
- qué fenómeno describe;
- cuál es su forma matemática;
- qué representa cada término;
- cuáles son sus condiciones de aplicación;
- si posee carácter vectorial o escalar;
- qué consecuencias importantes se derivan.

Puede utilizarse, según corresponda:

```latex
\begin{principio}[Nombre]
...
\end{principio}
```

o:

```latex
\begin{leyfisica}[Nombre]
...
\end{leyfisica}
```

No limitar una ley física a mostrar su ecuación.

---

# 16. Introducción de ecuaciones

Antes de presentar una ecuación importante debe quedar claro qué problema
físico resuelve.

Después de presentarla deben explicarse:

- significado de cada variable;
- unidades;
- carácter escalar o vectorial;
- condiciones de validez;
- interpretación física;
- signos;
- casos particulares cuando aporten valor.

Una fórmula no debe aparecer como un objeto aislado.

---

# 17. Interpretación física de las ecuaciones

Toda ecuación importante debe leerse físicamente.

Por ejemplo:

```latex
\[
v=v_0+at
\]
```

no debe presentarse únicamente como una relación algebraica.

Debe explicarse que, bajo aceleración constante, la velocidad cambia
linealmente con el tiempo.

Puede analizarse:

```text
a > 0
a < 0
a = 0
```

pero siempre en relación con el sistema de referencia y con el signo de la
velocidad.

También debe explicarse qué representa físicamente:

```latex
at
```

y cómo se relaciona la ecuación con una gráfica \(v-t\).

---

# 18. Condiciones de validez

Toda ecuación que no sea universal debe acompañarse de sus condiciones de
aplicación.

Por ejemplo:

```latex
\[
v^2=v_0^2+2a\Delta x
\]
```

requiere aceleración constante.

La relación:

```latex
\[
F=-kx
\]
```

corresponde al régimen en el que el sistema puede modelarse mediante la ley de
Hooke.

Debe indicarse claramente cuándo una relación:

- es exacta dentro del modelo;
- es aproximada;
- es empírica;
- depende de determinadas hipótesis;
- corresponde únicamente a un caso particular.

---

# 19. Deducciones

Las ecuaciones importantes deben deducirse cuando la deducción aporte
comprensión física.

Una deducción debe mostrar:

1. punto de partida;
2. principio físico utilizado;
3. hipótesis;
4. relaciones matemáticas;
5. transformaciones relevantes;
6. resultado;
7. interpretación.

No omitir pasos conceptualmente importantes.

Tampoco extender una deducción mediante pasos algebraicos triviales que
dificulten seguir la Física.

La prioridad es mostrar por qué aparece la ecuación.

---

# 20. Matemáticas como lenguaje de la Física

Las matemáticas deben utilizarse como herramienta para expresar relaciones
físicas.

Cuando se utilicen:

- álgebra;
- geometría;
- trigonometría;
- vectores;
- derivadas;
- integrales;
- ecuaciones diferenciales;

debe explicarse su significado físico cuando esto aporte comprensión.

No convertir innecesariamente la teoría de Física en un curso de Matemáticas.

Cuando una herramienta matemática sea necesaria y no pueda suponerse conocida,
puede recordarse brevemente.

No repetir capítulos completos de Matemáticas dentro de Física.

---

# 21. Cálculo diferencial

Cuando una derivada posea significado físico debe explicarse.

Por ejemplo:

```latex
\[
v_x=\frac{dx}{dt}
\]
```

debe interpretarse como la tasa instantánea de cambio de la posición respecto
del tiempo.

De forma similar:

```latex
\[
a_x=\frac{dv_x}{dt}
\]
```

representa la tasa instantánea de cambio de la velocidad.

No introducir derivadas únicamente como operaciones formales.

---

# 22. Cálculo integral

Cuando una integral posea significado físico debe explicarse.

Por ejemplo:

```latex
\[
\Delta x=\int_{t_1}^{t_2}v_x(t)\,dt
\]
```

debe relacionarse con:

- acumulación;
- desplazamiento;
- área algebraica bajo la gráfica \(v_x-t\).

Cuando corresponda debe distinguirse entre:

```text
área geométrica
```

y:

```text
área algebraica
```

según los signos de la función.

---

# 23. Ecuaciones diferenciales

Cuando aparezca una ecuación diferencial debe explicarse primero qué relación
física expresa.

No comenzar directamente con técnicas de solución.

Debe identificarse:

- variable dependiente;
- variable independiente;
- parámetros físicos;
- condiciones iniciales;
- significado físico de la solución.

La complejidad matemática debe justificarse por el contenido físico.

---

# 24. Análisis dimensional

Cuando aporte comprensión debe comprobarse la homogeneidad dimensional de una
ecuación.

El análisis dimensional puede utilizarse para:

- detectar errores;
- comprobar relaciones;
- interpretar constantes;
- anticipar dependencias;
- verificar resultados.

No utilizarlo como sustituto de una deducción física cuando esta sea necesaria.

---

# 25. Signos

Los signos deben interpretarse físicamente.

No enseñar reglas incorrectas como:

```text
aceleración negativa = desaceleración
```

La interpretación correcta depende del sistema de referencia.

En movimiento rectilíneo:

```text
velocidad y aceleración con el mismo signo
→ aumenta la rapidez

velocidad y aceleración con signos opuestos
→ disminuye la rapidez
```

Esta lógica debe explicarse, no memorizarse como una regla aislada.

---

# 26. Dirección y sentido

Cuando una magnitud sea vectorial debe explicarse cómo determinar:

- dirección;
- sentido;
- componentes;
- signo de las componentes.

No utilizar únicamente una magnitud positiva cuando el problema requiera
información vectorial.

En resultados vectoriales debe indicarse claramente la orientación física.

---

# 27. Unidades

Las unidades deben formar parte del razonamiento.

Cuando se introduzca una ecuación debe comprobarse, cuando sea útil, que las
unidades sean coherentes.

Utilizar prioritariamente el SI.

Las conversiones necesarias deben mostrarse explícitamente cuando aporten valor
pedagógico.

No mezclar unidades incompatibles dentro de una ecuación.

---

# 28. Cifras significativas

En ejemplos numéricos debe evitarse presentar una precisión injustificada.

El número de cifras significativas debe ser razonable respecto de los datos.

No llenar la teoría de discusiones metrológicas cuando no sean relevantes, pero
tampoco presentar resultados con una precisión artificial.

---

# 29. Casos especiales

Los casos especiales deben presentarse como consecuencias del modelo general
cuando sea posible.

Ejemplos:

- velocidad inicial nula;
- aceleración nula;
- equilibrio;
- movimiento en sentido negativo;
- fuerza resultante nula;
- carga positiva;
- carga negativa;
- ángulo nulo;
- pequeñas oscilaciones;
- ausencia de rozamiento;
- campo uniforme.

Evitar enseñar cada caso como una fórmula independiente si puede comprenderse a
partir de una relación general.

---

# 30. Casos límite

Cuando un caso límite aporte comprensión, debe analizarse.

Preguntas útiles pueden ser:

```text
¿qué ocurre cuando una magnitud tiende a cero?
¿qué ocurre cuando una distancia se hace muy grande?
¿qué ocurre si desaparece una fuerza?
¿qué ocurre si el ángulo es cero?
¿el resultado recupera un caso conocido?
```

Los casos límite permiten comprobar la coherencia física de una expresión.

---

# 31. Representaciones gráficas

Cuando una gráfica aporte comprensión debe incluirse o explicarse.

Toda gráfica física debe identificar:

- variable del eje horizontal;
- variable del eje vertical;
- unidades;
- escala cuando sea relevante;
- signo;
- pendiente;
- interceptos;
- áreas cuando tengan significado físico;
- regiones importantes.

No utilizar una gráfica únicamente como decoración.

---

# 32. Interpretación de pendientes

Cuando la pendiente posea significado físico debe explicarse.

Por ejemplo:

```text
gráfica x-t
→ pendiente = velocidad

gráfica v-t
→ pendiente = aceleración
```

Debe aclararse cuándo se habla de:

- pendiente media;
- pendiente instantánea.

La interpretación geométrica debe conectarse con la definición física.

---

# 33. Interpretación de áreas

Cuando el área bajo una curva posea significado físico debe explicarse.

Por ejemplo:

```text
área algebraica bajo v-t
→ desplazamiento

área algebraica bajo a-t
→ cambio de velocidad
```

Debe indicarse claramente cuándo el signo del área tiene significado físico.

---

# 34. Diagramas

Los diagramas deben utilizarse cuando reduzcan la dificultad conceptual.

Pueden incluir:

- sistemas de referencia;
- vectores;
- trayectorias;
- diagramas de cuerpo libre;
- superficies gaussianas;
- campos;
- circuitos;
- rayos;
- ondas;
- procesos termodinámicos.

Los diagramas deben ser:

- claros;
- rotulados;
- físicamente correctos;
- consistentes con la notación del texto.

---

# 35. Diagramas de cuerpo libre

Cuando se utilice un diagrama de cuerpo libre debe quedar claro:

1. qué cuerpo se aísla;
2. qué fuerzas externas actúan sobre él;
3. qué sistema de referencia se utiliza;
4. qué componentes se tomarán.

No incluir en el diagrama fuerzas ejercidas por el cuerpo sobre otros objetos.

No inventar fuerzas para representar movimiento.

---

# 36. Ejemplos dentro de la teoría

Los ejemplos de `teoria.tex` tienen función pedagógica.

Deben enseñar cómo utilizar los conceptos que acaban de desarrollarse.

No deben convertirse simplemente en una colección adicional de ejercicios.

Los ejemplos deben seleccionarse para:

- aclarar un concepto;
- mostrar una aplicación;
- introducir un método;
- interpretar una ecuación;
- comparar casos;
- mostrar un error frecuente;
- conectar varias ideas.

Puede utilizarse:

```latex
\begin{ejemplo}
...
\end{ejemplo}
```

---

# 37. Progresión de los ejemplos

Cuando un tema lo justifique, los ejemplos deben avanzar progresivamente.

Una secuencia posible es:

```text
ejemplo conceptual
→ aplicación directa
→ ejemplo con representación
→ ejemplo con varios pasos
→ ejemplo que exige elegir el método
```

No es necesario incluir todos estos tipos en cada tema.

La cantidad de ejemplos debe responder a las necesidades pedagógicas del
contenido.

---

# 38. Estructura de un ejemplo numérico

Cuando corresponda, un ejemplo puede mostrar:

1. situación física;
2. datos;
3. incógnita;
4. sistema de referencia;
5. esquema;
6. principio físico;
7. ecuaciones;
8. despeje;
9. sustitución;
10. cálculo;
11. unidades;
12. resultado;
13. interpretación.

No todos los ejemplos necesitan mostrar formalmente cada apartado.

Debe evitarse una estructura burocrática cuando el razonamiento sea sencillo.

---

# 39. Interpretación del resultado

Un ejemplo no debe terminar necesariamente al obtener un número.

Cuando aporte valor debe explicarse:

- qué significa el resultado;
- si el signo tiene sentido;
- si la dirección es razonable;
- si la magnitud es plausible;
- qué ocurriría al modificar un parámetro;
- qué relación física evidencia.

---

# 40. Métodos alternativos

Cuando existan varios métodos físicamente relevantes puede explicarse más de
uno.

Debe indicarse cuándo un método resulta especialmente conveniente.

No es necesario mostrar varias soluciones si una alternativa no aporta
aprendizaje adicional.

El objetivo no es acumular procedimientos.

El objetivo es que el estudiante pueda elegir una estrategia.

---

# 41. Comparación de métodos

Cuando dos métodos sean importantes puede compararse:

- qué información requieren;
- qué principios utilizan;
- cuál es más general;
- cuál es más directo;
- cuál permite mayor interpretación física;
- qué limitaciones posee cada uno.

Ejemplos posibles:

```text
cinemática vs. energía
componentes vectoriales vs. construcción geométrica
dinámica vs. conservación de energía
integración directa vs. ecuación conocida
```

No presentar los métodos como recetas desconectadas.

---

# 42. Aplicaciones

Incluir aplicaciones cuando ayuden a comprender la importancia del concepto.

Pueden relacionarse con:

- ingeniería;
- tecnología;
- transporte;
- construcción;
- electricidad;
- electrónica;
- medicina;
- astronomía;
- deportes;
- instrumentos;
- fenómenos naturales;
- situaciones cotidianas.

La aplicación debe estar conectada realmente con la Física estudiada.

No incluir ejemplos decorativos que no aporten comprensión.

---

# 43. Relación con experimentos

Cuando corresponda, explicar cómo una ley o relación puede observarse o medirse
experimentalmente.

Puede discutirse:

- qué magnitudes se medirían;
- qué instrumentos podrían utilizarse;
- qué variables se controlarían;
- qué gráfica se construiría;
- qué representa la pendiente;
- qué comportamiento apoyaría el modelo;
- qué desviaciones indicarían limitaciones del modelo.

No es necesario convertir cada tema en una práctica de laboratorio.

---

# 44. Interpretación microscópica y macroscópica

Cuando aporte valor, conectar la descripción macroscópica con una interpretación
microscópica.

Ejemplos:

```text
expansión térmica
↔ estructura atómica

presión
↔ choques moleculares

corriente eléctrica
↔ movimiento de portadores

elasticidad
↔ interacción entre partículas
```

No introducir una explicación microscópica demasiado avanzada si distrae del
objetivo principal.

---

# 45. Errores frecuentes

Los errores conceptuales importantes deben señalarse explícitamente.

Puede utilizarse:

```latex
\begin{errorfrecuente}
...
\end{errorfrecuente}
```

o:

```latex
\begin{advertencia}
...
\end{advertencia}
```

Debe explicarse:

1. cuál es el error;
2. por qué es incorrecto;
3. cuál es la interpretación correcta.

Ejemplos:

- confundir distancia con desplazamiento;
- confundir velocidad con rapidez;
- creer que aceleración negativa implica siempre disminuir rapidez;
- confundir masa con peso;
- creer que acción y reacción se cancelan;
- ignorar el signo de una carga;
- utilizar una ecuación fuera de sus condiciones de validez;
- sumar vectores como si fueran escalares.

No llenar la teoría de advertencias innecesarias.

---

# 46. Conocimientos previos

Cuando un concepto dependa de contenidos anteriores, recordarlos brevemente si
esto facilita la continuidad.

Por ejemplo:

- antes de componentes, recordar descomposición vectorial;
- antes de trabajo, recordar producto escalar;
- antes de potencial eléctrico, conectar con energía potencial;
- antes de ondas, recordar movimiento armónico.

No repetir capítulos completos.

El recordatorio debe contener únicamente lo necesario para continuar.

---

# 47. Conexiones con temas posteriores

Cuando un concepto sea fundamental para capítulos futuros puede indicarse
brevemente.

Por ejemplo:

```text
campo eléctrico
→ potencial eléctrico

movimiento armónico
→ ondas

trabajo y energía
→ termodinámica y electromagnetismo

momento angular
→ sistemas orbitales y Física moderna
```

No desarrollar anticipadamente toda la teoría posterior.

---

# 48. Continuidad conceptual

Cada tema debe sentirse como parte de una obra progresiva.

Siempre que sea posible debe quedar claro:

```text
qué sabemos
→ qué problema aparece
→ qué nuevo concepto necesitamos
→ qué permite explicar
→ hacia qué tema conduce
```

Las transiciones deben evitar la sensación de capítulos desconectados.

---

# 49. Nivel de profundidad

La teoría no debe escribirse exclusivamente para un grado escolar determinado
salvo petición expresa.

Debe buscar un equilibrio entre:

- claridad;
- profundidad;
- rigor;
- extensión;
- utilidad pedagógica.

Debe ser suficientemente accesible para aprender el tema y suficientemente
completa para que un docente pueda utilizarla como base de clase.

No reducir un tema a una colección de fórmulas.

Tampoco extender innecesariamente la explicación mediante repeticiones.

---

# 50. Desarrollo progresivo del formalismo

Cuando el tema lo permita, introducir primero una descripción accesible y
aumentar gradualmente el formalismo.

Una progresión posible es:

```text
interpretación cualitativa
→ representación gráfica
→ relación algebraica
→ formulación vectorial
→ formulación mediante cálculo
```

No introducir inmediatamente el nivel matemático más avanzado cuando una
construcción gradual facilite la comprensión.

No evitar el cálculo cuando este aporte una comprensión más profunda y sea
adecuado al desarrollo del tema.

---

# 51. Rigor físico

Toda afirmación física debe ser correcta.

Verificar especialmente:

- condiciones de aplicación;
- signos;
- dirección;
- sentido;
- unidades;
- sistemas de referencia;
- carácter escalar o vectorial;
- conservación;
- causalidad cuando corresponda;
- aproximaciones;
- límites de los modelos.

No utilizar una explicación intuitiva si conduce a una interpretación
físicamente incorrecta.

---

# 52. Rigor matemático

Verificar cuidadosamente:

- álgebra;
- geometría;
- trigonometría;
- derivadas;
- integrales;
- signos;
- exponentes;
- vectores;
- unidades;
- dimensiones;
- resultados numéricos.

Las deducciones matemáticas deben ser coherentes con las hipótesis físicas
utilizadas.

---

# 53. Estilo de redacción

Todo el contenido debe escribirse en español claro, académico y natural.

Preferir explicaciones completas pero directas.

Evitar:

- frases innecesariamente rebuscadas;
- lenguaje excesivamente coloquial;
- repeticiones;
- definiciones circulares;
- párrafos sin función pedagógica;
- afirmaciones vagas;
- listas excesivas cuando un párrafo explique mejor la idea.

La precisión no debe sacrificarse por brevedad.

La claridad no debe sacrificarse por formalismo.

---

# 54. Terminología

Utilizar terminología física consistente.

No alternar arbitrariamente entre términos equivalentes si esto puede confundir.

Cuando existan varias denominaciones habituales puede mencionarse la alternativa
la primera vez.

Después debe mantenerse preferentemente una denominación principal.

La terminología debe permanecer coherente entre:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

---

# 55. Notación

La notación debe ser consistente con el resto de la colección.

Antes de introducir una notación diferente debe comprobarse si el proyecto ya
posee una convención establecida.

No cambiar arbitrariamente símbolos entre:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

Cuando un cambio sea realmente necesario debe revisarse su impacto sobre el
tema completo.

---

# 56. Código LaTeX

El contenido definitivo debe entregarse como LaTeX limpio y listo para integrarse
en el proyecto.

Los archivos internos:

```text
teoria.tex
```

no deben contener normalmente:

```latex
\documentclass
\begin{document}
\end{document}
```

porque son incluidos desde documentos maestros.

Deben utilizar los comandos y entornos ya definidos globalmente.

No redefinir localmente:

- colores;
- comandos;
- estilos;
- entornos;

sin una razón justificada.

---

# 57. Estructura LaTeX

Utilizar según corresponda:

```latex
\section{}
\subsection{}
\subsubsection{}
```

de acuerdo con la jerarquía establecida por el documento maestro.

No introducir:

```latex
\chapter{}
```

si el capítulo ya es creado desde el documento maestro.

No crear niveles de sección innecesarios.

---

# 58. Entornos pedagógicos

Utilizar los entornos definidos globalmente cuando ayuden a distinguir la
función del contenido.

Entre ellos pueden encontrarse:

```latex
\begin{definicion}
\end{definicion}

\begin{principio}
\end{principio}

\begin{leyfisica}
\end{leyfisica}

\begin{modelo}
\end{modelo}

\begin{hipotesis}
\end{hipotesis}

\begin{aproximacion}
\end{aproximacion}

\begin{idea}
\end{idea}

\begin{interpretacion}
\end{interpretacion}

\begin{formula}
\end{formula}

\begin{condicion}
\end{condicion}

\begin{ejemplo}
\end{ejemplo}

\begin{aplicacion}
\end{aplicacion}

\begin{consejo}
\end{consejo}

\begin{estrategia}
\end{estrategia}

\begin{advertencia}
\end{advertencia}

\begin{errorfrecuente}
\end{errorfrecuente}

\begin{observacion}
\end{observacion}

\begin{recordatorio}
\end{recordatorio}

\begin{nota}
\end{nota}

\begin{notapedagogica}
\end{notapedagogica}

\begin{resumen}
\end{resumen}
```

No utilizar cajas únicamente para decorar.

Cada entorno debe corresponder con la función conceptual del contenido.

---

# 59. Expresiones matemáticas en LaTeX

Las expresiones cortas deben mantenerse compactas cuando esto mejore la
legibilidad.

Por ejemplo:

```latex
\[
v=v_0+at.
\]
```

No dividir artificialmente ecuaciones breves en múltiples líneas.

Para desarrollos largos pueden utilizarse entornos apropiados como:

```latex
align
aligned
```

cuando mejoren la lectura.

No introducir saltos de línea únicamente por estética del código fuente.

---

# 60. Figuras e imágenes específicas

Las imágenes propias de un tema deben almacenarse en:

```text
tema/imagenes/
```

Las figuras deben incluirse solamente cuando aporten comprensión.

Cuando una figura pueda construirse claramente mediante:

- TikZ;
- PGFPlots;
- Circuitikz;

puede preferirse este método por:

- consistencia;
- calidad vectorial;
- facilidad de modificación;
- coherencia con la notación.

No crear diagramas excesivamente complejos si una figura sencilla comunica
mejor la idea.

---

# 61. Fuentes bibliográficas

Antes de desarrollar la teoría deben consultarse realmente las fuentes
bibliográficas pertinentes disponibles en:

```text
libros/
```

No basta con conocer el tema de memoria.

La consulta debe permitir comparar, cuando resulte útil:

- organización;
- secuencia conceptual;
- profundidad;
- definiciones;
- principios;
- leyes;
- modelos;
- hipótesis;
- notación;
- deducciones;
- representaciones;
- ejemplos;
- aplicaciones;
- métodos;
- progresión pedagógica.

No es necesario utilizar todos los libros para cada tema.

Deben seleccionarse las fuentes relevantes para el contenido concreto.

---

# 62. Uso de las fuentes principales

Las fuentes principales deben tener prioridad para establecer:

- rigor físico;
- profundidad;
- formulación matemática;
- relaciones entre conceptos;
- deducciones;
- condiciones de validez;
- estructura general del contenido.

Entre las fuentes principales del proyecto se encuentran:

```text
Sears–Zemansky / Young–Freedman
Serway–Jewett
Schaum / Bueche–Hecht
Bauer–Westfall
```

Schaum puede resultar especialmente útil para:

- granularidad;
- estructura de temas;
- procedimientos;
- problemas.

Sears, Serway y Bauer pueden utilizarse para complementar:

- profundidad conceptual;
- formalismo;
- deducciones;
- interpretación;
- aplicaciones.

No copiar la estructura de un único libro mecánicamente.

---

# 63. Uso de fuentes complementarias

Las fuentes complementarias pueden utilizarse para enriquecer:

- explicaciones;
- ejemplos;
- secuencias pedagógicas;
- aplicaciones;
- tratamiento introductorio;
- conexiones con enseñanza escolar.

Entre ellas pueden encontrarse:

```text
Serway–Vuille
Walter Pérez Terrel
Juan A. Cuéllar
Hipertexto Física
Investiguemos Física
```

Su contenido debe evaluarse con el mismo criterio de exactitud física y
matemática.

---

# 64. Síntesis de las fuentes

El contenido final debe ser original.

No debe reproducir mecánicamente un libro.

El procedimiento deseable es:

```text
consultar
→ comparar
→ identificar coincidencias y diferencias
→ seleccionar el enfoque más sólido
→ organizar pedagógicamente
→ redactar de forma original
→ verificar
```

La teoría final debe sentirse como parte de esta colección, no como un resumen
de una fuente concreta.

---

# 65. Discrepancias entre fuentes

Cuando distintas fuentes presenten:

- notaciones diferentes;
- convenciones distintas;
- enfoques pedagógicos diferentes;
- simplificaciones diferentes;
- grados de profundidad diferentes;

debe adoptarse la formulación que resulte:

1. físicamente correcta;
2. matemáticamente sólida;
3. pedagógicamente clara;
4. coherente con el resto de la colección.

Cuando la discrepancia sea relevante para la comprensión puede mencionarse.

No es necesario documentar diferencias menores que no afecten el aprendizaje.

---

# 66. Constantes y datos oficiales

Cuando se utilicen constantes físicas o datos cuyo valor requiera precisión
actualizada, verificar fuentes oficiales cuando sea necesario.

Pueden utilizarse:

```text
BIPM
NIST
```

para información metrológica y constantes.

No es necesario realizar una consulta externa para cada valor aproximado
pedagógico ampliamente establecido cuando la precisión exacta no sea relevante.

---

# 67. Preguntas de comprensión

Cuando aporten valor pueden incluirse preguntas conceptuales breves destinadas a
comprobar comprensión.

Ejemplos:

```text
¿puede un objeto tener velocidad cero y aceleración distinta de cero?

¿una aceleración negativa implica siempre que disminuye la rapidez?

¿qué diferencia existe entre distancia y desplazamiento?

¿por qué el campo eléctrico es una magnitud vectorial?

¿qué representa físicamente el área bajo una gráfica velocidad-tiempo?
```

Estas preguntas deben centrarse en razonamiento conceptual.

No sustituyen los ejercicios formales de:

```text
ejercicios.tex
```

---

# 68. Secuencia pedagógica para el docente

Cuando aporte utilidad puede incluirse al final del tema una breve orientación
para impartirlo.

Puede indicar, por ejemplo:

1. fenómeno inicial;
2. pregunta motivadora;
3. concepto principal;
4. demostración o ejemplo;
5. representación gráfica;
6. segundo ejemplo;
7. error frecuente;
8. preguntas de comprobación;
9. conexión con el siguiente tema.

No debe convertirse en un plan de clase burocrático.

Su función es facilitar el uso directo de la teoría.

---

# 69. Resumen final

Cuando el tema lo justifique puede incluirse:

```latex
\begin{resumen}
...
\end{resumen}
```

El resumen debe concentrar:

- ideas físicas esenciales;
- relaciones conceptuales;
- condiciones importantes;
- interpretaciones principales;
- conexiones.

No debe convertirse en un segundo formulario.

El formulario ya cumple la función de consulta rápida de ecuaciones.

---

# 70. Relación con `formulario.tex`

`teoria.tex` y `formulario.tex` tienen funciones distintas.

La teoría responde principalmente:

```text
¿qué significa?
¿por qué ocurre?
¿cómo se interpreta?
¿de dónde surge?
¿cómo se utiliza?
¿qué modelo se está empleando?
¿cuándo es válido?
¿qué representa físicamente?
```

El formulario responde principalmente:

```text
¿cuál es la ecuación?
¿qué significa cada símbolo?
¿qué unidad tiene?
¿qué condición debo cumplir?
¿qué caso especial debo recordar?
¿qué procedimiento breve debo utilizar?
```

Por tanto:

```text
teoria.tex
→ enseña y explica

formulario.tex
→ permite consultar rápidamente
```

No convertir `teoria.tex` en un formulario extendido.

No convertir `formulario.tex` en una teoría abreviada.

---

# 71. Relación con `ejercicios.tex`

Los ejemplos de:

```text
teoria.tex
```

enseñan cómo utilizar los conceptos.

Los problemas de:

```text
ejercicios.tex
```

permiten practicar y comprobar que el estudiante puede utilizarlos.

La teoría debe preparar suficientemente al estudiante para resolver los
ejercicios.

No debe exigirse sistemáticamente en los ejercicios un concepto que nunca haya
sido presentado o preparado en la teoría.

Los ejercicios tampoco deben ser simples copias numéricas de los ejemplos.

---

# 72. Evitar repetición innecesaria

La teoría debe ser completa, pero no repetitiva.

No explicar varias veces exactamente la misma idea con palabras diferentes si
esto no añade comprensión.

Una repetición puede justificarse cuando:

- conecta con otro concepto;
- presenta otra representación;
- corrige una idea intuitiva incorrecta;
- muestra una aplicación;
- introduce un nivel más profundo de formalismo.

La extensión debe responder a la complejidad física del tema.

---

# 73. No simplificar incorrectamente

Nunca sacrificar exactitud física para producir una explicación aparentemente
más sencilla.

Si una afirmación solo es válida bajo determinadas condiciones, indicarlas.

Si una explicación introductoria es una aproximación, identificarla.

Si existe una excepción importante, mencionarla cuando sea pedagógicamente
relevante.

La simplificación debe reducir dificultad, no introducir errores.

---

# 74. Revisión conceptual

Antes de considerar terminada la teoría debe comprobarse:

- que los conceptos estén correctamente definidos;
- que las leyes estén correctamente formuladas;
- que los modelos estén identificados;
- que las hipótesis estén claras;
- que las aproximaciones estén señaladas;
- que las ecuaciones tengan condiciones de validez;
- que los signos estén interpretados;
- que los vectores estén tratados correctamente;
- que las unidades sean coherentes;
- que las gráficas sean correctas;
- que los ejemplos sean físicamente válidos;
- que las conexiones conceptuales sean correctas.

---

# 75. Revisión matemática

Antes de considerar terminada la teoría debe comprobarse:

- álgebra;
- despejes;
- signos;
- trigonometría;
- derivadas;
- integrales;
- productos vectoriales;
- componentes;
- dimensiones;
- unidades;
- resultados numéricos.

No entregar una deducción sin comprobarla.

---

# 76. Revisión de ejemplos

Cada ejemplo numérico debe verificarse independientemente.

Comprobar:

```text
datos
→ conversiones
→ ecuaciones
→ despeje
→ sustitución
→ operaciones
→ unidades
→ cifras significativas
→ signo
→ dirección
→ resultado
→ interpretación
```

No asumir que un resultado es correcto porque el procedimiento parece familiar.

---

# 77. Revisión de figuras

Antes de considerar terminada una figura comprobar:

- orientación de ejes;
- signos;
- dirección de vectores;
- sentido de flechas;
- etiquetas;
- unidades;
- posición de objetos;
- correspondencia con el texto;
- coherencia con las ecuaciones.

Una figura físicamente incorrecta puede producir más confusión que la ausencia
de figura.

---

# 78. Revisión de continuidad

Antes de terminar un tema comprobar:

```text
¿qué conceptos anteriores necesita?
¿se recordaron cuando era necesario?
¿introduce símbolos nuevos correctamente?
¿mantiene la notación establecida?
¿prepara los ejercicios?
¿prepara el formulario?
¿conecta con el siguiente tema?
```

El tema debe integrarse en la obra completa.

---

# 79. Procedimiento antes de crear una teoría nueva

Antes de escribir un nuevo:

```text
teoria.tex
```

debe realizarse, como mínimo, el siguiente proceso:

1. consultar `AGENTS.md`;
2. consultar `pendientes.md`;
3. consultar `instrucciones/teoria.md`;
4. consultar `instrucciones/configuracion.md` cuando sea necesario;
5. localizar el tema dentro del índice maestro;
6. revisar los temas inmediatamente anteriores relacionados;
7. identificar las fuentes bibliográficas pertinentes;
8. consultar realmente esas fuentes;
9. comparar sus enfoques;
10. determinar la estructura conceptual del tema;
11. comprobar la notación ya establecida;
12. identificar diagramas o gráficas necesarios;
13. desarrollar el contenido;
14. verificar Física y Matemáticas;
15. comprobar coherencia LaTeX.

No comenzar a escribir directamente desde conocimiento general si las fuentes
del proyecto están disponibles.

---

# 80. Procedimiento para revisar una teoría existente

Cuando se solicite revisar un:

```text
teoria.tex
```

existente, no debe reescribirse automáticamente desde cero.

Primero:

1. leer el archivo completo;
2. identificar su posición en el índice;
3. consultar las instrucciones vigentes;
4. consultar las fuentes pertinentes;
5. identificar errores físicos;
6. identificar errores matemáticos;
7. identificar omisiones importantes;
8. identificar problemas pedagógicos;
9. identificar inconsistencias de notación;
10. identificar problemas LaTeX;
11. conservar el contenido correcto que ya funcione;
12. modificar únicamente lo necesario para llevarlo al estándar actual.

No destruir una estructura correcta únicamente por preferencia estilística.

---

# 81. Criterio para considerar completa la teoría

La teoría de un tema puede considerarse completa cuando:

- enseña suficientemente el fenómeno;
- define los conceptos necesarios;
- establece las magnitudes;
- presenta los modelos;
- identifica hipótesis y aproximaciones;
- desarrolla las leyes y principios;
- explica las ecuaciones;
- establece condiciones de validez;
- interpreta signos y vectores;
- utiliza las matemáticas con significado físico;
- incluye las representaciones necesarias;
- contiene ejemplos suficientes;
- analiza los casos importantes;
- señala errores frecuentes relevantes;
- conecta con conocimientos anteriores;
- prepara los temas posteriores cuando corresponda;
- mantiene coherencia con el resto de la colección;
- ha sido contrastada con las fuentes pertinentes;
- ha sido revisada física y matemáticamente;
- utiliza correctamente la configuración LaTeX del proyecto.

Solo después de cumplir estos criterios puede marcarse el componente:

```text
teoría
```

como completo en:

```text
pendientes.md
```

---

# 82. Principio final

La teoría debe construir comprensión.

Ante cualquier decisión de redacción debe priorizarse:

```text
exactitud física
→ exactitud matemática
→ comprensión conceptual
→ claridad pedagógica
→ progresión
→ interpretación física
→ coherencia con la colección
→ utilidad para aprender
→ utilidad para enseñar
```

El lector no debe terminar un tema sabiendo únicamente qué fórmula utilizar.

Debe comprender:

```text
qué fenómeno describe,
por qué aparece la relación,
qué significa físicamente,
bajo qué condiciones funciona,
cómo se representa,
cómo se utiliza
y cómo se conecta con el resto de la Física.
```