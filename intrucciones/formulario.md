# Criterios para desarrollar el formulario

Este archivo establece los criterios específicos que deben seguirse al crear,
revisar, ampliar o corregir los archivos `formulario.tex` del proyecto de
Física.

Las reglas generales del proyecto se encuentran en `AGENTS.md`.

Las decisiones de arquitectura y configuración LaTeX se encuentran en
`instrucciones/configuracion.md`.

Los criterios de desarrollo conceptual se encuentran en
`instrucciones/teoria.md`.

Los criterios para problemas y soluciones se encuentran en
`instrucciones/ejercicios.md`.

El estado actual del proyecto y el punto exacto de continuación se encuentran
en `pendientes.md`.

Este archivo no debe utilizarse para registrar progreso ni decisiones
estructurales generales.

Su función exclusiva es establecer **cómo debe construirse el material de
consulta rápida de cada tema**.

---

# 1. Objetivo del formulario

El archivo `formulario.tex` debe funcionar como material de consulta rápida.

Su objetivo es permitir localizar con facilidad:

- conceptos esenciales;
- magnitudes;
- símbolos;
- unidades;
- definiciones operativas;
- leyes;
- principios;
- fórmulas;
- relaciones entre magnitudes;
- condiciones de aplicación;
- casos particulares;
- procedimientos breves;
- relaciones gráficas;
- conversiones;
- constantes;
- advertencias importantes.

El formulario debe ser suficientemente completo para resultar útil durante:

- estudio;
- repaso;
- resolución de ejercicios;
- preparación de una clase;
- consulta rápida.

No debe convertirse en una reproducción abreviada de toda la teoría.

---

# 2. Diferencia entre teoría y formulario

`teoria.tex` y `formulario.tex` cumplen funciones diferentes.

La teoría responde principalmente:

    ¿qué significa?
    ¿por qué ocurre?
    ¿cómo se interpreta?
    ¿de dónde surge?
    ¿qué modelo se utiliza?
    ¿cuáles son las hipótesis?
    ¿cómo se deduce?
    ¿cuándo es válido?
    ¿cómo se conecta con otros conceptos?

El formulario responde principalmente:

    ¿cuál es la relación?
    ¿qué significa cada símbolo?
    ¿qué unidad tiene?
    ¿qué condición debe cumplirse?
    ¿qué signo debo considerar?
    ¿qué caso particular existe?
    ¿qué procedimiento breve debo seguir?
    ¿qué relación necesito consultar?

Por tanto:

    teoria.tex
    → desarrolla comprensión

    formulario.tex
    → concentra información para consulta rápida

No convertir `formulario.tex` en una teoría resumida párrafo por párrafo.

---

# 3. El formulario no es una lista de fórmulas

Aunque las ecuaciones constituyen una parte importante, el formulario no debe
reducirse a una colección de expresiones matemáticas.

Una fórmula aislada puede ser peligrosa si el lector no sabe:

- qué representa;
- qué significan sus variables;
- qué unidades utiliza;
- bajo qué condiciones es válida;
- qué convención de signos supone;
- si es escalar o vectorial;
- si corresponde a una relación general o a un caso particular.

Por tanto, toda fórmula importante debe conservar la información mínima
necesaria para utilizarla correctamente.

---

# 4. Principio de consulta rápida

La organización debe permitir encontrar información con rapidez.

El contenido debe ser:

- compacto;
- jerarquizado;
- visualmente claro;
- preciso;
- consistente;
- fácil de recorrer.

Evitar:

- párrafos excesivamente largos;
- deducciones extensas;
- explicaciones históricas;
- introducciones narrativas;
- ejemplos desarrollados completos;
- repeticiones innecesarias.

La brevedad no debe eliminar información indispensable para utilizar
correctamente una relación.

---

# 5. Cobertura

El formulario debe cubrir los elementos esenciales desarrollados en la teoría
del mismo tema.

Antes de escribirlo debe revisarse `teoria.tex`.

Debe comprobarse qué elementos requieren consulta rápida, por ejemplo:

- definiciones fundamentales;
- magnitudes;
- símbolos;
- unidades;
- relaciones generales;
- leyes;
- principios;
- condiciones;
- casos especiales;
- procedimientos;
- gráficas;
- constantes;
- conversiones.

No incluir sistemáticamente contenido que no aparezca ni se prepare en la
teoría.

---

# 6. Jerarquía conceptual

El formulario debe conservar la jerarquía conceptual del tema.

Siempre que sea posible, organizar la información aproximadamente como:

    concepto
    → magnitudes
    → relación general
    → condiciones
    → casos particulares
    → procedimiento
    → advertencias

Esta secuencia puede modificarse cuando otra organización resulte más natural.

No ordenar fórmulas únicamente por apariencia matemática.

---

# 7. Organización según la teoría

El orden del formulario debe corresponder, en términos generales, al desarrollo
conceptual de `teoria.tex`.

Esto permite que el estudiante pueda pasar fácilmente de una explicación
detallada a su resumen operativo.

No es necesario reproducir exactamente todas las secciones de la teoría.

El formulario puede agrupar información que en la teoría se desarrolla por
separado cuando esto mejore la consulta.

---

# 8. Definiciones esenciales

Las definiciones fundamentales pueden aparecer de forma compacta.

Por ejemplo:

    Velocidad media:
    cambio de posición por unidad de tiempo.

seguido de:

    \[
    \bar{v}_x=\frac{\Delta x}{\Delta t}.
    \]

La definición debe conservar el significado físico mínimo necesario.

No incluir explicaciones extensas que correspondan a la teoría.

---

# 9. Magnitudes físicas

Cuando resulte útil, incluir una tabla o estructura compacta con:

- magnitud;
- símbolo;
- tipo;
- unidad SI.

Por ejemplo:

    Magnitud        Símbolo       Tipo        Unidad SI
    Posición        \(x\)         escalar*    m
    Velocidad       \(\vect{v}\)  vectorial   m/s
    Aceleración     \(\vect{a}\)  vectorial   m/s²

La clasificación debe respetar el contexto físico.

No crear tablas innecesarias si solo existen una o dos magnitudes.

---

# 10. Símbolos

Todo símbolo importante utilizado en el formulario debe estar definido.

No asumir que el lector recordará automáticamente qué representa cada letra.

Debe evitarse utilizar el mismo símbolo para magnitudes diferentes dentro del
mismo contexto.

La notación debe coincidir con:

    teoria.tex
    ejercicios.tex

del mismo tema.

---

# 11. Unidades

Las unidades SI deben indicarse cuando correspondan.

Debe prestarse especial atención a:

- magnitudes derivadas;
- unidades compuestas;
- prefijos;
- magnitudes adimensionales;
- unidades equivalentes.

No añadir unidades a funciones matemáticas, razones adimensionales o cantidades
que no las poseen.

---

# 12. Sistema Internacional

Utilizar prioritariamente el Sistema Internacional de Unidades.

Cuando una unidad no SI sea de uso frecuente y pedagógicamente relevante puede
incluirse junto con su conversión.

Por ejemplo:

    \[
    \SI{1}{\kilo\metre\per\hour}
    =
    \frac{1}{3.6}\,\SI{}{\metre\per\second}.
    \]

No llenar el formulario de conversiones que no tengan relación directa con el
tema.

---

# 13. Prefijos SI

Cuando sean especialmente relevantes para el tema, puede incluirse una tabla
compacta de prefijos.

Por ejemplo:

    kilo   \(k\)       \(10^3\)
    mili   \(m\)       \(10^{-3}\)
    micro  \(\mu\)     \(10^{-6}\)
    nano   \(n\)       \(10^{-9}\)

No repetir tablas generales de prefijos en todos los temas si ya existe un
recurso global apropiado.

Incluir únicamente los prefijos cuya consulta sea realmente útil.

---

# 14. Fórmulas

Cada fórmula debe presentarse junto con la información mínima necesaria para
usarla correctamente.

Como mínimo, cuando corresponda, debe quedar claro:

- qué calcula;
- qué representan sus variables;
- qué condiciones requiere;
- qué convención de signos utiliza;
- si es vectorial o escalar.

No presentar una ecuación únicamente porque aparece habitualmente en los
formularios escolares.

Debe tener una función real dentro del tema.

---

# 15. Fórmula general antes que casos particulares

Cuando exista una relación general de la que se obtengan varios casos
particulares, debe darse prioridad a la relación general.

Los casos particulares pueden incluirse después si son útiles para consulta.

Evitar memorizar como fórmulas independientes relaciones que pueden comprenderse
como casos de una misma expresión.

Por ejemplo, debe distinguirse entre:

    ecuación general
    → caso particular
    → condición adicional

---

# 16. Condiciones de aplicación

Toda fórmula que no sea universal debe conservar sus condiciones de aplicación.

Por ejemplo:

    \[
    v=v_0+at
    \]

debe asociarse con:

    aceleración constante.

De forma similar:

    \[
    v^2=v_0^2+2a\Delta x
    \]

debe indicar también:

    aceleración constante.

No confiar en que el estudiante recordará la condición por contexto.

---

# 17. Condiciones junto a la ecuación

Siempre que sea posible, colocar la condición cerca de la fórmula a la que
corresponde.

Evitar una estructura en la que todas las ecuaciones aparezcan primero y las
condiciones varias páginas después.

El formulario debe reducir el riesgo de utilizar una expresión fuera de su
régimen de validez.

---

# 18. Hipótesis e idealizaciones

Cuando una fórmula dependa de una hipótesis importante, indicarla brevemente.

Ejemplos:

    resistencia del aire despreciable;
    resorte ideal;
    masa constante;
    campo uniforme;
    carga puntual;
    pequeñas oscilaciones;
    sistema aislado.

No repetir explicaciones extensas sobre las hipótesis.

Su desarrollo corresponde a `teoria.tex`.

---

# 19. Aproximaciones

Toda aproximación relevante debe identificarse.

Por ejemplo:

    Cerca de la superficie terrestre:
    \[
    g\approx \SI{9.8}{\metre\per\second\squared}.
    \]

o:

    Para ángulos pequeños:
    \[
    \sin\theta\approx\theta,
    \]
    con \(\theta\) expresado en radianes.

No presentar una aproximación como igualdad exacta cuando esto pueda inducir a
error.

---

# 20. Principios y leyes

Los principios y leyes fundamentales deben identificarse por su nombre cuando
esto facilite la consulta.

Por ejemplo:

    Segunda ley de Newton

    \[
    \sum\vect{F}=m\vect{a}.
    \]

Debe incluirse la condición o interpretación mínima necesaria.

No limitarse a escribir una ecuación sin indicar qué ley representa cuando el
nombre tenga valor conceptual.

---

# 21. Relaciones vectoriales

Cuando una ley sea vectorial debe conservarse su forma vectorial.

Por ejemplo:

    \[
    \sum\vect{F}=m\vect{a}.
    \]

No sustituirla sistemáticamente por una expresión escalar que oculte su
naturaleza.

Después pueden incluirse las ecuaciones por componentes:

    \[
    \sum F_x=ma_x,
    \qquad
    \sum F_y=ma_y.
    \]

---

# 22. Escalares y vectores

El formulario debe distinguir claramente entre magnitudes escalares y
vectoriales cuando esto sea relevante.

No utilizar indistintamente:

    \(F\)

y:

    \(\vect{F}\)

si una representa la magnitud y la otra el vector.

La notación debe seguir las convenciones globales del proyecto.

---

# 23. Componentes rectangulares

Cuando el tema utilice vectores en dos dimensiones, incluir las relaciones
fundamentales de componentes cuando sean necesarias para resolver problemas.

Por ejemplo:

    \[
    \vect{A}=A_x\ihat+A_y\jhat.
    \]

Si \(\theta\) se mide desde el eje \(+x\):

    \[
    A_x=A\cos\theta,
    \qquad
    A_y=A\sin\theta.
    \]

Debe indicarse que los signos dependen del cuadrante y de la orientación de los
ejes.

No presentar seno y coseno como reglas de signos.

---

# 24. Suma vectorial mediante componentes

Cuando corresponda:

    \[
    R_x=\sum_i A_{ix},
    \qquad
    R_y=\sum_i A_{iy}.
    \]

Magnitud:

    \[
    R=\sqrt{R_x^2+R_y^2}.
    \]

Dirección:

    \[
    \theta=\operatorname{atan2}(R_y,R_x)
    \]

cuando la notación y herramientas adoptadas permitan expresar de forma clara la
determinación correcta del cuadrante.

Si se utiliza:

    \[
    \tan\theta=\frac{R_y}{R_x},
    \]

debe añadirse una advertencia sobre el cuadrante.

---

# 25. Sistemas de referencia

Cuando los signos dependan del sistema de referencia, el formulario debe
recordarlo brevemente.

Por ejemplo:

    Eje \(y\) positivo hacia arriba:
    \[
    a_y=-g.
    \]

No presentar:

    \[
    a=-g
    \]

como una propiedad absoluta de la gravedad.

El signo depende de la orientación elegida para el eje.

---

# 26. Signos

Incluir advertencias compactas cuando exista un error frecuente relacionado con
los signos.

Por ejemplo:

    \(a<0\) no significa necesariamente que disminuya la rapidez.

En movimiento rectilíneo:

    \(v\) y \(a\) con el mismo signo
    → aumenta la rapidez.

    \(v\) y \(a\) con signos opuestos
    → disminuye la rapidez.

Estas notas deben ser breves.

La explicación completa corresponde a la teoría.

---

# 27. Dirección y sentido

Cuando una magnitud vectorial no quede completamente especificada mediante su
magnitud, el formulario debe recordar que el resultado requiere:

- dirección;
- sentido;

o, alternativamente:

- componentes.

No considerar completa una receta de resolución vectorial que produzca
únicamente un valor positivo.

---

# 28. Procedimientos breves

El formulario puede incluir procedimientos compactos para problemas
recurrentes.

Por ejemplo:

    Suma de vectores:
    1. elegir ejes;
    2. descomponer cada vector;
    3. sumar componentes;
    4. hallar la magnitud;
    5. determinar dirección y sentido.

Estos procedimientos deben ser breves.

No convertirlos en soluciones desarrolladas.

---

# 29. Estrategias de resolución

Cuando un tema requiera una estrategia general que no pueda resumirse mediante
una sola ecuación, incluir una secuencia operativa.

Por ejemplo:

    Dinámica:
    1. aislar el cuerpo;
    2. dibujar el diagrama de cuerpo libre;
    3. elegir ejes;
    4. descomponer fuerzas;
    5. aplicar \(\sum F_x=ma_x\) y \(\sum F_y=ma_y\).

La estrategia debe servir como recordatorio.

La explicación detallada pertenece a la teoría y a las soluciones.

---

# 30. Casos particulares

Los casos particulares importantes pueden incluirse cuando:

- aparecen con frecuencia;
- reducen significativamente el trabajo;
- tienen interpretación física propia;
- son útiles durante la resolución de ejercicios.

Debe quedar claro de qué relación general proceden y qué condición adicional
requieren.

No acumular casos particulares innecesarios.

---

# 31. Casos límite

Los casos límite pueden incluirse cuando funcionen como comprobaciones rápidas.

Por ejemplo:

    si \(a=0\),
    las ecuaciones de movimiento uniformemente acelerado deben reducirse al
    movimiento con velocidad constante.

No es necesario incluir análisis extensos.

---

# 32. Relaciones de proporcionalidad

Cuando una ecuación revele una dependencia física importante puede indicarse de
forma compacta.

Por ejemplo:

    \[
    F\propto\frac{1}{r^2}.
    \]

Esto permite responder rápidamente preguntas del tipo:

    si \(r\) se duplica,
    \(F\) se reduce a la cuarta parte.

No repetir relaciones de proporcionalidad que sean triviales o irrelevantes.

---

# 33. Dependencias funcionales

Cuando resulte útil, señalar si una relación es:

- lineal;
- cuadrática;
- inversa;
- inversa al cuadrado;
- exponencial;
- sinusoidal.

Esto puede ayudar a conectar ecuaciones y gráficas.

La descripción debe mantenerse breve.

---

# 34. Gráficas

Cuando las relaciones gráficas sean fundamentales para el tema, el formulario
debe incluir sus propiedades esenciales.

Por ejemplo, para cinemática:

    gráfica \(x-t\)
    → pendiente = velocidad.

    gráfica \(v-t\)
    → pendiente = aceleración.

    gráfica \(v-t\)
    → área algebraica = desplazamiento.

    gráfica \(a-t\)
    → área algebraica = cambio de velocidad.

No desarrollar una explicación completa de cada gráfica.

---

# 35. Pendientes

Cuando la pendiente posea significado físico, debe indicarse claramente.

Por ejemplo:

    \[
    v_x=\frac{dx}{dt}
    \]

corresponde a la pendiente instantánea de la gráfica \(x-t\).

Cuando sea necesario, distinguir entre pendiente media e instantánea.

---

# 36. Áreas

Cuando el área bajo una gráfica posea significado físico, indicarlo.

Por ejemplo:

    \[
    \Delta x=\int_{t_1}^{t_2}v_x(t)\,dt.
    \]

Debe recordarse que se trata de área algebraica cuando la función puede tomar
valores negativos.

---

# 37. Derivadas

Cuando el tema utilice cálculo, incluir las relaciones diferenciales
fundamentales.

Por ejemplo:

    \[
    v_x=\frac{dx}{dt},
    \qquad
    a_x=\frac{dv_x}{dt}
       =\frac{d^2x}{dt^2}.
    \]

No incluir un curso de derivación.

El formulario debe concentrar las relaciones físicas.

---

# 38. Integrales

Cuando sean necesarias:

    \[
    \Delta x=\int_{t_1}^{t_2}v_x(t)\,dt,
    \]

    \[
    \Delta v_x=\int_{t_1}^{t_2}a_x(t)\,dt.
    \]

Debe indicarse brevemente qué representa cada integral.

No incluir deducciones extensas.

---

# 39. Relaciones equivalentes

Cuando una misma relación pueda escribirse de varias formas útiles, pueden
incluirse formas equivalentes si realmente facilitan la resolución.

Evitar llenar el formulario con múltiples despejes de la misma ecuación.

En general, es preferible presentar:

    ecuación fundamental

y realizar el despeje necesario durante el problema.

Puede incluirse un despeje frecuente si tiene valor práctico evidente.

---

# 40. No crear un catálogo de despejes

Evitar estructuras como:

    \[
    v=v_0+at
    \]

    \[
    v_0=v-at
    \]

    \[
    a=\frac{v-v_0}{t}
    \]

    \[
    t=\frac{v-v_0}{a}
    \]

si todas son simples transformaciones de la misma ecuación.

El formulario debe enseñar relaciones físicas, no sustituir la capacidad de
despejar.

---

# 41. Tablas

Las tablas pueden utilizarse cuando permitan comparar información de manera más
rápida que un texto continuo.

Son especialmente útiles para:

- magnitudes y unidades;
- casos particulares;
- comparación de modelos;
- constantes;
- conversiones;
- signos;
- relaciones gráficas.

No utilizar tablas cuando el contenido sea demasiado extenso o conceptual para
leerse correctamente en celdas.

---

# 42. Cuadros de comparación

Cuando dos conceptos se confundan con frecuencia puede utilizarse una
comparación breve.

Por ejemplo:

    Distancia
    → escalar
    → longitud total recorrida.

    Desplazamiento
    → vectorial
    → cambio de posición.

La comparación debe concentrar diferencias esenciales.

La explicación profunda corresponde a la teoría.

---

# 43. Advertencias

El formulario debe incluir advertencias cuando ayuden a prevenir errores
frecuentes.

Por ejemplo:

    No confundir rapidez con velocidad.

    No utilizar ecuaciones de aceleración constante si \(a\) varía.

    El signo de una componente depende del eje elegido.

    El área bajo \(v-t\) representa desplazamiento, no necesariamente distancia.

Las advertencias deben ser breves y específicas.

---

# 44. Errores frecuentes

No es necesario reproducir todos los errores frecuentes desarrollados en
`teoria.tex`.

Seleccionar únicamente aquellos cuya consulta rápida resulte especialmente
útil durante la resolución de problemas.

No saturar el formulario con cajas de advertencia.

---

# 45. Constantes físicas

Cuando el tema requiera constantes físicas de uso frecuente, puede incluirse
una tabla compacta.

Debe indicarse:

- símbolo;
- valor;
- unidad.

Por ejemplo:

    \[
    g\approx\SI{9.8}{\metre\per\second\squared}.
    \]

Los valores deben ser coherentes con el resto del proyecto.

---

# 46. Precisión de constantes

No utilizar más cifras de las necesarias para el nivel y propósito del
formulario.

Cuando se requiera precisión actualizada, consultar las fuentes oficiales
correspondientes, como BIPM o NIST.

Para ejercicios pedagógicos puede utilizarse un valor aproximado siempre que
sea consistente.

---

# 47. Conversiones

Incluir conversiones cuando sean utilizadas con frecuencia dentro del tema.

Por ejemplo:

    \[
    \SI{1}{\kilo\metre\per\hour}
    =
    \frac{5}{18}\,\SI{}{\metre\per\second}.
    \]

No convertir el formulario de cada tema en una tabla general de unidades.

Las conversiones generales deben centralizarse cuando exista un lugar
apropiado para ellas.

---

# 48. Notación científica

Cuando el tema utilice escalas muy grandes o muy pequeñas, puede incluirse un
recordatorio mínimo de notación científica y prefijos relevantes.

Esto resulta especialmente útil en:

- gravitación;
- electricidad;
- magnetismo;
- física atómica;
- física moderna;
- astronomía.

No repetir explicaciones matemáticas básicas innecesariamente.

---

# 49. Relaciones trigonométricas

Cuando un tema utilice repetidamente descomposición vectorial o geometría,
pueden incluirse las relaciones trigonométricas estrictamente necesarias.

Por ejemplo:

    \[
    \sin\theta=\frac{\text{cateto opuesto}}{\text{hipotenusa}},
    \qquad
    \cos\theta=\frac{\text{cateto adyacente}}{\text{hipotenusa}}.
    \]

No convertir el formulario de Física en un formulario general de
trigonometría.

---

# 50. Ángulos

Cuando se utilicen componentes, debe quedar claro desde qué eje se mide el
ángulo.

Si:

    \[
    A_x=A\cos\theta,
    \qquad
    A_y=A\sin\theta,
    \]

debe indicarse que esta forma supone que \(\theta\) se mide respecto del eje
\(+x\), salvo que el contexto establezca otra cosa.

No memorizar seno y coseno independientemente de la geometría.

---

# 51. Cuadrantes

Cuando sea relevante, incluir un recordatorio breve de que la dirección obtenida
mediante:

    \[
    \tan^{-1}\left(\frac{A_y}{A_x}\right)
    \]

debe corregirse según los signos de \(A_x\) y \(A_y\).

Cuando sea posible, preferir una formulación que determine correctamente el
cuadrante.

---

# 52. Diagramas mínimos

El formulario puede incluir diagramas pequeños cuando permitan comprender una
convención de forma mucho más rápida que el texto.

Por ejemplo:

- sistema de ejes;
- convención angular;
- componentes de un vector;
- signo de una fuerza;
- esquema de una configuración típica.

No incluir figuras complejas que ocupen espacio sin mejorar la consulta.

---

# 53. Diagramas y fórmulas

Cuando una ecuación dependa fuertemente de una geometría, puede resultar útil
colocar un pequeño esquema junto a ella.

Esto es especialmente útil en:

- vectores;
- torque;
- óptica;
- electricidad;
- magnetismo;
- ondas.

El esquema debe coincidir exactamente con la convención utilizada en la
ecuación.

---

# 54. TikZ y PGFPlots

Cuando una figura sencilla pueda construirse mediante TikZ o PGFPlots, puede
preferirse esta solución por:

- calidad vectorial;
- coherencia;
- facilidad de modificación;
- integración con LaTeX.

No utilizar diagramas generados si una explicación textual compacta resulta más
clara.

---

# 55. Ejemplos mínimos

El formulario puede incluir ejemplos mínimos cuando ayuden a recordar cómo se
aplica una relación.

Un ejemplo mínimo debe ser breve.

Por ejemplo:

    Si \(r\) se duplica en una relación \(F\propto1/r^2\),
    entonces:
    \[
    F'=\frac{F}{4}.
    \]

No incluir soluciones completas con datos, desarrollo, sustitución y análisis.

Eso corresponde a `ejercicios.tex`.

---

# 56. Cuándo no incluir ejemplos

No incluir ejemplos únicamente para llenar espacio.

Si una fórmula y su condición son suficientemente claras, el ejemplo puede ser
innecesario.

El formulario debe permanecer compacto.

---

# 57. Relaciones entre conceptos

Cuando varias magnitudes estén conectadas, puede ser útil mostrar una cadena de
relaciones.

Por ejemplo, en cinemática:

    \[
    x(t)
    \xrightarrow{\ d/dt\ }
    v(t)
    \xrightarrow{\ d/dt\ }
    a(t).
    \]

y:

    \[
    a(t)
    \xrightarrow{\ \int dt\ }
    v(t)
    \xrightarrow{\ \int dt\ }
    x(t).
    \]

Este tipo de representación puede condensar una estructura conceptual completa.

---

# 58. Jerarquía entre ecuaciones

Cuando existan muchas ecuaciones, debe distinguirse entre:

- relaciones fundamentales;
- relaciones derivadas;
- casos particulares.

No presentarlas todas con el mismo peso visual si no poseen la misma
importancia conceptual.

La relación fundamental debe resultar fácil de localizar.

---

# 59. Ecuaciones fundamentales

Las ecuaciones fundamentales del tema deben destacarse mediante los mecanismos
ya definidos globalmente.

No crear un estilo local diferente para cada tema.

Debe consultarse `config/entornos.tex` antes de introducir nuevos recursos de
presentación.

---

# 60. Deducciones

El formulario no es el lugar para deducciones largas.

Cuando resulte útil recordar el origen de una ecuación puede incluirse una
cadena muy breve, por ejemplo:

    \[
    a=\frac{dv}{dt}
    \quad\Longrightarrow\quad
    dv=a\,dt
    \quad\Longrightarrow\quad
    v=v_0+at,
    \]

para \(a\) constante.

Solo debe hacerse cuando la cadena aporte valor de consulta.

La deducción completa pertenece a la teoría.

---

# 61. Condiciones matemáticas

Cuando una ecuación requiera una condición matemática además de una física,
debe indicarse.

Por ejemplo:

    aproximación de ángulo pequeño:
    \[
    \sin\theta\approx\theta,
    \qquad
    |\theta|\ll1,
    \]
    con \(\theta\) en radianes.

No omitir restricciones que puedan producir un uso incorrecto.

---

# 62. Convenciones

Las convenciones utilizadas en el tema deben resumirse cuando sean necesarias.

Pueden incluir:

- sentido positivo;
- dirección angular positiva;
- notación vectorial;
- signos de cargas;
- orientación de campos;
- convención de potencial;
- sentido de corriente;
- convención de signos termodinámicos.

Las convenciones deben coincidir con la teoría y los ejercicios.

---

# 63. Convenciones que pueden variar

Cuando existan varias convenciones válidas, no presentar una como universal.

Debe indicarse cuál adopta el proyecto.

Por ejemplo, en un problema vertical puede elegirse positivo hacia arriba o
hacia abajo.

El formulario puede mostrar la convención preferida o recordar que el signo
depende de la elección del eje.

---

# 64. Procedimientos vectoriales

Cuando el tema involucre varias magnitudes vectoriales, debe incluirse un
procedimiento general.

Por ejemplo:

    1. dibujar o identificar la geometría;
    2. elegir ejes;
    3. determinar dirección y sentido de cada vector;
    4. obtener componentes;
    5. sumar componentes;
    6. reconstruir la resultante;
    7. interpretar dirección y sentido.

Este procedimiento debe mantenerse coherente con `ejercicios.md`.

---

# 65. Procedimientos de problemas con coordenadas

Cuando las posiciones estén dadas mediante coordenadas, puede incluirse:

    \[
    \Delta\vect{r}
    =
    (x_2-x_1)\ihat
    +
    (y_2-y_1)\jhat.
    \]

Magnitud:

    \[
    r=\sqrt{(\Delta x)^2+(\Delta y)^2}.
    \]

Vector unitario:

    \[
    \hat{r}
    =
    \frac{\Delta\vect{r}}{r}.
    \]

Este procedimiento es especialmente útil en gravitación, electricidad y otros
problemas de campos.

---

# 66. Superposición

Cuando un tema utilice el principio de superposición, debe incluirse su forma
operativa.

Por ejemplo:

    \[
    \vect{E}_{\text{neto}}
    =
    \sum_i \vect{E}_i.
    \]

Debe recordarse que la suma es vectorial.

No reducir una superposición vectorial a suma de magnitudes salvo en
configuraciones donde esto sea válido.

---

# 67. Conservación

Cuando el tema utilice una ley de conservación, el formulario debe indicar:

- qué magnitud se conserva;
- bajo qué condición;
- relación entre estado inicial y final.

Por ejemplo:

    Sistema aislado:
    \[
    \vect{p}_i=\vect{p}_f.
    \]

La condición debe permanecer junto a la ecuación.

---

# 68. Energía

Cuando corresponda, distinguir claramente:

- energía cinética;
- energía potencial;
- energía mecánica;
- trabajo;
- potencia.

No agrupar ecuaciones de energía sin indicar qué representa cada una.

Las condiciones para conservar energía mecánica deben quedar visibles.

---

# 69. Dinámica

Cuando el tema sea de dinámica, el formulario debe conservar como relación
central:

    \[
    \sum\vect{F}=m\vect{a}.
    \]

y, cuando corresponda:

    \[
    \sum F_x=ma_x,
    \qquad
    \sum F_y=ma_y.
    \]

Debe acompañarse de un procedimiento breve basado en diagrama de cuerpo libre.

No convertir la dinámica en una lista de fórmulas para cada configuración
particular.

---

# 70. Cinemática

Cuando el tema sea de cinemática, debe distinguirse claramente entre:

- posición;
- desplazamiento;
- distancia;
- velocidad;
- rapidez;
- aceleración.

Las ecuaciones de movimiento con aceleración constante deben agruparse bajo una
condición explícita:

    \(a=\text{constante}\).

No presentarlas como ecuaciones generales de cualquier movimiento.

---

# 71. Movimiento vertical

En caída libre y movimiento vertical debe indicarse claramente:

    si \(+y\) apunta hacia arriba:
    \[
    a_y=-g.
    \]

La aceleración no cambia de signo cuando el objeto pasa del ascenso al descenso
si se conserva el mismo sistema de referencia.

Esta advertencia debe aparecer de forma compacta.

---

# 72. Electricidad

En temas eléctricos debe distinguirse cuidadosamente entre:

- carga;
- fuerza eléctrica;
- campo eléctrico;
- energía potencial eléctrica;
- potencial eléctrico.

No utilizar indistintamente magnitudes relacionadas pero físicamente distintas.

Las unidades deben quedar especialmente claras.

---

# 73. Signo de las cargas

Cuando intervengan cargas positivas y negativas, el formulario debe distinguir
entre:

- magnitud de una cantidad;
- signo de la carga;
- dirección del vector.

No insertar automáticamente el signo de una carga en una magnitud escalar de
fuerza para decidir la dirección.

La orientación debe determinarse mediante el análisis físico y vectorial.

---

# 74. Campos

Cuando una magnitud de campo sea vectorial, conservar su formulación vectorial.

En configuraciones con varias fuentes:

    \[
    \vect{F}_{\text{net}}
    =
    \sum_i\vect{F}_i,
    \]

o:

    \[
    \vect{E}_{\text{net}}
    =
    \sum_i\vect{E}_i.
    \]

El formulario debe recordar el principio de superposición cuando corresponda.

---

# 75. Magnitudes escalares en campos

Cuando una magnitud asociada al campo sea escalar, debe aprovecharse esta
diferencia.

Por ejemplo, el potencial eléctrico se suma algebraicamente:

    \[
    V=\sum_i V_i.
    \]

Esto debe diferenciarse claramente de la suma vectorial del campo eléctrico.

---

# 76. Diferencias conceptuales importantes

Cuando dos relaciones similares puedan confundirse, el formulario debe
distinguirlas explícitamente.

Por ejemplo:

    Campo eléctrico:
    vectorial.

    Potencial eléctrico:
    escalar.

o:

    Distancia:
    escalar.

    Desplazamiento:
    vectorial.

Estas comparaciones son especialmente valiosas en un formulario.

---

# 77. Estructura visual

El formulario debe poder recorrerse visualmente con facilidad.

Debe utilizarse de forma coherente:

- títulos;
- subtítulos;
- tablas;
- ecuaciones;
- cajas existentes;
- listas breves;
- espacios.

No debe convertirse en una pared continua de ecuaciones.

Tampoco debe fragmentarse en una cantidad excesiva de cajas pequeñas.

---

# 78. Densidad de información

El formulario debe ser compacto, pero no ilegible.

No reducir excesivamente:

- tamaño de fuente;
- espacios;
- explicaciones;
- etiquetas;

solo para introducir más contenido en una página.

La prioridad es que la información pueda localizarse y utilizarse rápidamente.

---

# 79. Orden de lectura

Aunque el formulario sea de consulta, debe poder leerse de principio a fin de
manera coherente.

No debe parecer una colección aleatoria de ecuaciones.

Debe conservar una estructura conceptual reconocible.

---

# 80. Redundancia útil

Una pequeña redundancia puede justificarse cuando evita errores.

Por ejemplo, repetir:

    \(a=\text{constante}\)

junto a varias ecuaciones de cinemática puede ser preferible a indicarlo una
sola vez de forma poco visible.

La redundancia debe utilizarse para seguridad conceptual, no para llenar
espacio.

---

# 81. Redundancia innecesaria

Evitar repetir exactamente la misma:

- definición;
- ecuación;
- advertencia;
- tabla;

en varios lugares del formulario sin una razón clara.

El formulario debe ser eficiente.

---

# 82. Contenido que no debe incluirse normalmente

No incluir normalmente:

- historia extensa;
- biografías;
- motivaciones largas;
- demostraciones completas;
- soluciones desarrolladas;
- grandes bloques narrativos;
- problemas completos;
- discusiones pedagógicas para el docente;
- referencias bibliográficas extensas.

Estos contenidos pertenecen a otros componentes.

---

# 83. Relación con los ejercicios

El formulario debe contener las relaciones y recordatorios necesarios para
resolver los ejercicios del tema sin convertirse en un solucionario.

Antes de considerarlo terminado debe revisarse `ejercicios.tex`.

Debe comprobarse:

- que las fórmulas utilizadas aparezcan cuando sea razonable;
- que las condiciones importantes estén disponibles;
- que la notación coincida;
- que los procedimientos generales sean coherentes.

No debe incluir la solución específica de ningún ejercicio.

---

# 84. Relación con las soluciones

Las soluciones desarrolladas pueden utilizar el formulario como referencia
operativa.

Por ello, las ecuaciones y convenciones deben coincidir exactamente.

Si durante la creación de los ejercicios aparece una relación importante que no
estaba contemplada, debe evaluarse si pertenece al formulario.

No añadir automáticamente toda ecuación utilizada en una solución.

---

# 85. Relación con la teoría

El formulario debe derivarse de la teoría, no desarrollarse de manera
independiente.

Antes de crearlo debe leerse `teoria.tex` completo.

Si se detecta una inconsistencia entre teoría y formulario, no debe resolverse
silenciosamente.

Debe determinarse cuál formulación es correcta y mantener coherencia en todo el
tema.

---

# 86. Fuentes bibliográficas

Antes de desarrollar un formulario nuevo deben consultarse las fuentes
pertinentes disponibles en `libros/`, especialmente cuando exista duda sobre:

- notación;
- formulación de una ley;
- condiciones de validez;
- unidades;
- casos particulares;
- convenciones;
- constantes;
- relaciones derivadas.

No basta con recopilar fórmulas de memoria.

---

# 87. Uso de las fuentes

Las fuentes deben utilizarse para comparar:

- ecuaciones fundamentales;
- notación;
- condiciones;
- organización;
- casos especiales;
- procedimientos;
- advertencias;
- tablas útiles.

El formulario final debe integrarse en la estructura propia del proyecto.

No copiar mecánicamente el formulario de un libro.

---

# 88. Fuentes principales

Entre las fuentes principales del proyecto se encuentran:

    Sears–Zemansky / Young–Freedman
    Serway–Jewett
    Schaum / Bueche–Hecht
    Bauer–Westfall

Estas fuentes pueden utilizarse para comprobar:

- rigor;
- formulaciones generales;
- condiciones;
- notación;
- relaciones fundamentales.

Schaum puede resultar especialmente útil para identificar relaciones operativas
y casos utilizados con frecuencia en problemas.

---

# 89. Fuentes complementarias

También pueden consultarse:

    Serway–Vuille
    Walter Pérez Terrel
    Juan A. Cuéllar
    Hipertexto Física
    Investiguemos Física

Estas fuentes pueden resultar útiles para:

- presentación introductoria;
- tablas;
- conversiones;
- relaciones operativas;
- nivel escolar;
- organización de consulta.

Toda información debe comprobarse con criterio físico y matemático.

---

# 90. Discrepancias entre fuentes

Si las fuentes utilizan diferentes:

- símbolos;
- signos;
- convenciones;
- valores aproximados;
- formulaciones;

debe elegirse la opción que resulte:

1. físicamente correcta;
2. matemáticamente consistente;
3. coherente con la teoría;
4. coherente con los ejercicios;
5. coherente con el resto del proyecto.

No mezclar convenciones diferentes dentro del mismo formulario.

---

# 91. Originalidad

El formulario final debe ser una síntesis propia del proyecto.

No debe reproducir de manera mecánica:

- tablas;
- formularios;
- resúmenes;
- cuadros;

de una fuente concreta.

La organización debe responder a las necesidades de esta colección.

---

# 92. Código LaTeX

`formulario.tex` es un fragmento de contenido.

No debe contener normalmente:

    \documentclass
    \begin{document}
    \end{document}

Debe integrarse en los documentos maestros existentes.

No redefinir localmente:

- comandos;
- colores;
- estilos;
- entornos;

si estos ya existen globalmente.

---

# 93. Jerarquía LaTeX

Utilizar según corresponda:

    \section{}
    \subsection{}
    \subsubsection{}

de acuerdo con la jerarquía establecida por el documento maestro.

No introducir `\chapter{}` si el capítulo ya es creado externamente.

No crear subdivisiones innecesarias para cantidades mínimas de contenido.

---

# 94. Entornos existentes

Antes de crear una caja o estructura nueva debe consultarse
`config/entornos.tex`.

Utilizar los entornos existentes cuando sean adecuados.

Pueden existir, entre otros:

    definicion
    principio
    leyfisica
    formula
    condicion
    advertencia
    recordatorio
    resumen

No asumir que todos deben utilizarse.

El formulario debe mantener una presentación compacta.

---

# 95. Uso de cajas

Las cajas deben utilizarse para establecer jerarquía y facilitar la consulta.

No encerrar cada ecuación en una caja independiente.

Demasiadas cajas destruyen la jerarquía visual.

Reservarlas para información realmente importante.

---

# 96. Expresiones matemáticas

Las expresiones cortas deben mantenerse compactas.

Por ejemplo:

    \[
    v=v_0+at.
    \]

No dividir artificialmente ecuaciones sencillas en varias líneas.

Para conjuntos relacionados puede utilizarse `aligned`, `align` u otra
estructura ya compatible con el proyecto cuando mejore la lectura.

---

# 97. Alineación de ecuaciones

Cuando varias ecuaciones pertenezcan al mismo conjunto, puede ser conveniente
alinearlas.

Por ejemplo:

    \[
    \begin{aligned}
    v &= v_0+at,\\
    x &= x_0+v_0t+\frac12at^2,\\
    v^2 &= v_0^2+2a(x-x_0).
    \end{aligned}
    \]

Debe quedar visible la condición común:

    \(a=\text{constante}\).

---

# 98. Unidades con `siunitx`

Cuando la configuración del proyecto utilice `siunitx`, deben escribirse las
unidades mediante sus comandos correspondientes.

Por ejemplo:

    \[
    g=\SI{9.8}{\metre\per\second\squared}.
    \]

No mezclar arbitrariamente diferentes estilos de escritura de unidades.

---

# 99. Notación vectorial LaTeX

Utilizar los comandos globales establecidos para vectores y vectores unitarios.

Por ejemplo, si el proyecto define:

    \vect{A}
    \ihat
    \jhat
    \khat

deben preferirse esos comandos frente a introducir notaciones locales
diferentes.

---

# 100. Imágenes

Las imágenes específicas del formulario deben almacenarse según la estructura
definida para el tema.

No duplicar una imagen de la teoría únicamente para decorar.

Puede reutilizarse o adaptarse una figura cuando tenga verdadera función de
consulta.

---

# 101. Tablas extensas

Si una tabla se vuelve demasiado grande, debe evaluarse si realmente pertenece
al formulario.

Una tabla extensa puede ser más difícil de consultar que varias estructuras
pequeñas bien organizadas.

No sacrificar legibilidad por compactación.

---

# 102. Longitud

No existe un número fijo de páginas para `formulario.tex`.

Su extensión depende de:

- cantidad de conceptos;
- cantidad de ecuaciones;
- número de condiciones;
- necesidad de tablas;
- procedimientos;
- complejidad del tema.

Debe ser más breve que la teoría, pero suficientemente completo para cumplir su
función.

---

# 103. No imponer una página

No debe intentarse forzar cada formulario a una sola página.

Algunos temas simples pueden ocupar una página.

Otros temas pueden necesitar varias.

La prioridad es la calidad de consulta, no una restricción artificial de
espacio.

---

# 104. Formularios acumulativos

Si en el futuro existen formularios globales o acumulativos, el formulario de
cada tema debe seguir siendo autoconsistente dentro de su alcance.

No eliminar información esencial de un tema únicamente porque aparece en un
formulario general, salvo que la arquitectura del proyecto establezca
explícitamente otra política.

---

# 105. Procedimiento antes de crear un formulario nuevo

Antes de escribir un nuevo `formulario.tex` debe realizarse, como mínimo, el
siguiente proceso:

1. consultar `AGENTS.md`;
2. consultar `pendientes.md`;
3. consultar `instrucciones/formulario.md`;
4. consultar `instrucciones/teoria.md`;
5. consultar `instrucciones/ejercicios.md` cuando ya existan ejercicios;
6. leer completamente `teoria.tex`;
7. identificar los conceptos esenciales;
8. identificar las magnitudes y símbolos;
9. identificar las unidades;
10. identificar las ecuaciones fundamentales;
11. identificar las condiciones de validez;
12. identificar los casos particulares útiles;
13. identificar procedimientos recurrentes;
14. identificar advertencias necesarias;
15. consultar las fuentes bibliográficas pertinentes;
16. comprobar notación y convenciones;
17. redactar una síntesis compacta;
18. verificar todas las ecuaciones;
19. verificar dimensiones y unidades;
20. comprobar coherencia con teoría y ejercicios;
21. comprobar LaTeX;
22. compilar cuando sea posible.

No comenzar simplemente recopilando todas las fórmulas que aparezcan en la
teoría.

---

# 106. Selección de contenido

Para cada elemento de la teoría debe preguntarse:

    ¿necesita el estudiante consultar esto rápidamente mientras estudia o
    resuelve problemas?

Si la respuesta es sí, puede pertenecer al formulario.

Si la respuesta es no, probablemente debe permanecer únicamente en la teoría.

Esta pregunta debe utilizarse para controlar la extensión.

---

# 107. Procedimiento para revisar un formulario existente

Cuando se solicite revisar un `formulario.tex` existente, no debe reescribirse
automáticamente desde cero.

Primero:

1. leer el formulario completo;
2. leer la teoría correspondiente;
3. revisar los ejercicios correspondientes cuando existan;
4. consultar las instrucciones vigentes;
5. identificar ecuaciones faltantes;
6. identificar ecuaciones innecesarias;
7. verificar condiciones;
8. verificar símbolos;
9. verificar unidades;
10. verificar signos;
11. verificar vectores;
12. verificar casos particulares;
13. verificar procedimientos;
14. verificar coherencia visual;
15. verificar LaTeX;
16. conservar el contenido correcto;
17. modificar únicamente lo necesario.

No reemplazar una estructura que funciona únicamente por preferencia
estilística.

---

# 108. Revisión de ecuaciones

Toda ecuación debe verificarse antes de considerar terminado el formulario.

Comprobar:

- signos;
- exponentes;
- factores numéricos;
- raíces;
- funciones trigonométricas;
- productos escalares;
- productos vectoriales;
- derivadas;
- integrales.

No asumir que una fórmula es correcta porque sea conocida.

---

# 109. Revisión dimensional

Comprobar la homogeneidad dimensional de las relaciones cuando corresponda.

Esto resulta especialmente importante en:

- fórmulas derivadas;
- expresiones modificadas;
- casos particulares;
- ecuaciones transcritas desde fuentes.

Una inconsistencia dimensional debe corregirse antes de continuar.

---

# 110. Revisión de unidades

Comprobar:

- unidad SI;
- símbolo correcto;
- prefijos;
- potencias;
- unidades compuestas;
- equivalencias.

No confundir símbolo de magnitud con símbolo de unidad.

---

# 111. Revisión de condiciones

Por cada fórmula debe preguntarse:

    ¿es siempre válida?

Si la respuesta es no, debe identificarse su condición.

Este control es obligatorio.

Una fórmula correcta utilizada fuera de sus condiciones puede producir una
solución físicamente incorrecta.

---

# 112. Revisión de notación

Antes de terminar comprobar que los símbolos coincidan con:

    teoria.tex
    ejercicios.tex

y con las convenciones generales del proyecto.

No introducir cambios de notación únicamente porque una fuente utilice símbolos
diferentes.

---

# 113. Revisión vectorial

Cuando existan vectores comprobar:

- notación;
- componentes;
- signos;
- ejes;
- ángulos;
- cuadrantes;
- magnitudes;
- unidades.

Debe quedar clara la diferencia entre vector y magnitud.

---

# 114. Revisión de constantes

Comprobar que:

- el valor sea correcto;
- la unidad sea correcta;
- la precisión sea apropiada;
- coincida con el valor utilizado en los ejercicios.

No permitir que teoría, formulario y ejercicios utilicen valores incompatibles
sin explicación.

---

# 115. Revisión visual

Después de compilar, cuando sea posible, revisar:

- jerarquía;
- legibilidad;
- densidad;
- alineación;
- tablas;
- cajas;
- ecuaciones;
- saltos de página;
- figuras;
- espacios.

Un formulario puede ser matemáticamente correcto y resultar difícil de
consultar por una mala organización visual.

---

# 116. Compilación

Cuando el entorno lo permita, compilar el documento maestro correspondiente.

Comprobar:

- errores;
- warnings relevantes;
- overfull boxes;
- tablas demasiado anchas;
- ecuaciones fuera del margen;
- imágenes;
- entornos;
- símbolos;
- unidades.

No modificar arbitrariamente la configuración global para solucionar un
problema local sin evaluar primero la causa.

---

# 117. Coherencia entre los tres componentes

Antes de marcar el formulario como completo debe comprobarse la coherencia:

    teoria.tex
    ↕
    formulario.tex
    ↕
    ejercicios.tex

Las tres piezas deben utilizar:

- la misma Física;
- la misma notación;
- las mismas convenciones;
- las mismas unidades;
- las mismas condiciones de validez.

El formulario debe actuar como puente operativo entre teoría y ejercicios.

---

# 118. Corrección de inconsistencias

Si durante la creación del formulario se descubre un error en la teoría o en los
ejercicios, no debe ocultarse adaptando silenciosamente el formulario.

Debe corregirse la fuente del problema y revisar los componentes afectados.

La coherencia debe lograrse mediante corrección física, no mediante
inconsistencias coordinadas.

---

# 119. Criterio para incluir una fórmula

Una fórmula debe incluirse cuando cumpla al menos una función importante, por
ejemplo:

- expresa una definición;
- representa una ley fundamental;
- se utiliza con frecuencia;
- resume una relación importante;
- permite resolver una familia de problemas;
- constituye un caso particular de uso frecuente;
- conecta dos representaciones relevantes.

No incluir ecuaciones únicamente porque aparezcan en una fuente.

---

# 120. Criterio para excluir una fórmula

Una fórmula puede omitirse si:

- se obtiene mediante un despeje trivial;
- es demasiado específica;
- rara vez se utiliza;
- pertenece a un desarrollo secundario;
- solo apareció en un ejemplo particular;
- añade más confusión que utilidad;
- duplica una relación ya presentada.

El formulario debe seleccionar, no acumular.

---

# 121. Criterio para incluir una advertencia

Una advertencia debe incluirse cuando exista un error:

- frecuente;
- conceptualmente importante;
- capaz de producir resultados incorrectos;
- fácil de cometer durante la resolución de problemas.

No incluir advertencias sobre errores demasiado particulares.

---

# 122. Criterio para incluir un procedimiento

Un procedimiento debe incluirse cuando:

- se repite en muchos ejercicios;
- exige varios pasos;
- el orden de los pasos es importante;
- ayuda a evitar errores;
- no puede reducirse a una sola ecuación.

Debe escribirse de manera breve y operativa.

---

# 123. Criterio para considerar completo un apartado

Un apartado del formulario puede considerarse completo cuando:

- contiene las relaciones esenciales;
- define sus símbolos;
- conserva las condiciones;
- indica las unidades necesarias;
- distingue vectores y escalares;
- incluye las advertencias relevantes;
- permite una consulta rápida;
- coincide con la teoría.

No debe considerarse completo únicamente porque contenga todas las fórmulas.

---

# 124. Criterio para considerar completo `formulario.tex`

El componente `formulario.tex` puede considerarse completo cuando:

- sintetiza los conceptos esenciales;
- incluye las magnitudes relevantes;
- utiliza símbolos consistentes;
- presenta las unidades SI necesarias;
- contiene las ecuaciones fundamentales;
- conserva las condiciones de aplicación;
- identifica hipótesis importantes;
- distingue relaciones generales y casos particulares;
- incluye procedimientos breves cuando son útiles;
- incluye advertencias relevantes;
- mantiene correctamente la naturaleza vectorial o escalar;
- es coherente con la teoría;
- es coherente con los ejercicios;
- las ecuaciones han sido verificadas;
- las dimensiones han sido verificadas;
- las unidades han sido verificadas;
- la notación ha sido revisada;
- el código LaTeX es correcto;
- la presentación permite consulta rápida;
- la compilación ha sido comprobada cuando sea posible.

Solo después de cumplir estos criterios puede registrarse el componente
`formulario` como completo en `pendientes.md`.

---

# 125. Pregunta de control final

Antes de terminar el formulario debe hacerse la siguiente comprobación:

    Si un estudiante comprende la teoría y está resolviendo un ejercicio,
    ¿puede encontrar aquí rápidamente la relación, condición, unidad o
    procedimiento que necesita sin tener que releer toda la teoría?

Si la respuesta es no porque falta información esencial, el formulario está
incompleto.

Si la respuesta es no porque existe demasiada información y resulta difícil
encontrarla, el formulario necesita simplificación y reorganización.

---

# 126. Principio final

El formulario debe concentrar la Física sin despojarla de sus condiciones de
validez.

Ante cualquier decisión debe priorizarse:

    exactitud física
    → exactitud matemática
    → condiciones de aplicación
    → claridad
    → rapidez de consulta
    → coherencia con la teoría
    → coherencia con los ejercicios
    → utilidad práctica
    → organización visual
    → concisión

El objetivo no es que el estudiante disponga de la mayor cantidad posible de
fórmulas.

El objetivo es que pueda consultar rápidamente **las relaciones correctas,
comprender qué representan y saber bajo qué condiciones puede utilizarlas**.