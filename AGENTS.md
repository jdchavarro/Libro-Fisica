# AGENTS.md

# Proyecto Física

Este archivo contiene las instrucciones generales que deben seguir los agentes,
asistentes de programación y herramientas de IA que trabajen dentro de este
repositorio.

Estas reglas se aplican a todo el proyecto.

Los criterios específicos para desarrollar teoría, formularios, ejercicios y
otros componentes se encuentran en la carpeta:

```text
instrucciones/
```

Este archivo no sustituye esos documentos. Su función es establecer las reglas
globales del proyecto, indicar qué documentación debe consultarse y definir el
procedimiento general de trabajo.

---

# 1. Objetivo del proyecto

El proyecto tiene como objetivo construir una colección completa, progresiva,
rigurosa y pedagógica de Física que pueda utilizarse tanto para:

- aprender Física;
- estudiar de manera autónoma;
- preparar clases;
- impartir clases;
- consultar fórmulas y relaciones;
- practicar mediante ejercicios;
- disponer de soluciones desarrolladas para uso docente.

La colección no debe convertirse en una acumulación de fórmulas, definiciones
o ejercicios independientes.

Debe constituir una obra coherente en la que se conecten:

- fenómenos;
- conceptos;
- magnitudes físicas;
- modelos;
- hipótesis;
- aproximaciones;
- leyes;
- principios;
- matemáticas;
- representaciones vectoriales;
- diagramas;
- gráficas;
- experimentos;
- aplicaciones;
- problemas;
- temas anteriores y posteriores.

La prioridad general del proyecto es:

1. exactitud física;
2. exactitud matemática;
3. comprensión conceptual;
4. claridad pedagógica;
5. coherencia interna;
6. progresión de dificultad;
7. interpretación física;
8. utilidad para estudiantes y docentes;
9. calidad editorial;
10. mantenibilidad del código LaTeX.

---

# 2. Idioma

Todo el contenido de la obra debe escribirse en español.

Esto incluye:

- teoría;
- formularios;
- ejercicios;
- respuestas;
- explicaciones;
- títulos;
- leyendas;
- tablas;
- diagramas;
- notas pedagógicas.

Las fuentes pueden encontrarse en español o en otros idiomas, pero el contenido
final debe redactarse en español claro, académico, natural y preciso.

No traducir mecánicamente una fuente.

---

# 3. Estructura principal del repositorio

La estructura actual del proyecto utiliza, entre otras, las siguientes
carpetas y archivos:

```text
Fisica/
├── capitulos/
├── config/
├── instrucciones/
├── libros/
├── recursos/
├── volumenes/
├── clase.tex
├── formulario.tex
├── pendientes.md
└── AGENTS.md
```

Pueden existir además archivos auxiliares producidos por LaTeX durante las
compilaciones.

La carpeta:

```text
estructura_anterior/
```

pertenece a una estructura anterior del proyecto.

Mientras continúe el proceso de migración, su existencia no debe interpretarse
como parte de la arquitectura actual.

No utilizarla como referencia para decidir la organización definitiva de
archivos nuevos.

Tampoco debe eliminarse o modificarse material de la estructura anterior salvo
que la tarea solicitada consista expresamente en su migración o depuración.

---

# 4. Arquitectura de los capítulos

Los contenidos definitivos se organizan principalmente dentro de:

```text
capitulos/
```

La estructura típica de un tema es:

```text
tema/
├── teoria.tex
├── formulario.tex
├── ejercicios.tex
└── imagenes/
```

No todos los temas necesitan obligatoriamente imágenes.

No crear archivos adicionales sin una necesidad real.

No cambiar arbitrariamente:

- nombres de carpetas;
- nombres de archivos;
- numeración;
- jerarquía de capítulos;
- estructura de los volúmenes;
- convenciones establecidas.

Si una mejora requiere modificar la arquitectura consolidada del proyecto,
debe proponerse y justificarse antes de realizar el cambio.

---

# 5. Documentación obligatoria

La carpeta:

```text
instrucciones/
```

contiene los criterios especializados del proyecto.

Antes de modificar contenido debe consultarse la documentación correspondiente.

Entre los documentos principales se encuentran:

```text
instrucciones/configuracion.md
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

Pueden existir otros documentos dentro de `instrucciones/`.

Si existen, deben consultarse cuando sean relevantes para la tarea.

No asumir que `AGENTS.md` contiene todos los criterios particulares.

---

# 6. Orden obligatorio antes de trabajar

Antes de crear, completar, revisar, migrar o modificar contenido del proyecto,
seguir este procedimiento.

## Paso 1. Leer `AGENTS.md`

Determinar las reglas generales del repositorio.

## Paso 2. Leer `pendientes.md`

Es obligatorio consultar:

```text
pendientes.md
```

antes de iniciar o continuar un tema.

Este archivo determina el estado real del proyecto y permite conocer:

- qué temas están completos;
- qué componentes están terminados;
- qué componentes están pendientes;
- qué contenido ha sido migrado;
- qué contenido permanece en la estructura anterior;
- cuál es el punto exacto de continuación;
- qué saltos temporales se han realizado;
- qué numeraciones son provisionales;
- qué comprobaciones siguen pendientes.

No deducir el estado de un tema únicamente por la existencia de sus archivos.

Un archivo existente puede estar:

- vacío;
- incompleto;
- sin revisar;
- pendiente de migración;
- pendiente de compilación;
- pendiente de integración.

`pendientes.md` es la referencia principal para el estado de avance.

## Paso 3. Leer las instrucciones específicas

Según la tarea, consultar como mínimo:

### Para teoría

```text
instrucciones/teoria.md
```

### Para formulario

```text
instrucciones/formulario.md
```

### Para ejercicios, respuestas o explicaciones

```text
instrucciones/ejercicios.md
```

### Para configuración, estructura, compilación o documentos maestros

```text
instrucciones/configuracion.md
```

Si la tarea afecta varios componentes, deben consultarse todos los documentos
correspondientes.

## Paso 4. Revisar el contenido existente

Antes de escribir contenido nuevo, comprobar si ya existe material relacionado
en:

- el mismo capítulo;
- capítulos anteriores;
- la estructura antigua;
- documentos maestros;
- recursos;
- otros archivos que `pendientes.md` indique expresamente.

No rehacer material existente sin comprobar primero si debe:

- conservarse;
- corregirse;
- ampliarse;
- adaptarse;
- migrarse.

## Paso 5. Consultar las fuentes

Cuando la tarea implique desarrollar o revisar contenido físico, consultar las
fuentes bibliográficas pertinentes de `libros/`.

## Jerarquía de fuentes

Las fuentes se encuentran en `libros/` y se dividen en dos grupos.

### Fuentes principales

Consultar prioritariamente `libros/principales/`.

Para desarrollar un tema no es necesario consultar íntegramente todos los
libros. Localizar primero las secciones pertinentes.

Como regla general, contrastar al menos:

1. Sears–Zemansky / Young–Freedman;
2. Serway–Jewett;
3. Schaum / Bueche–Hecht.

Consultar Bauer–Westfall cuando aporte una perspectiva adicional o cuando
existan dudas sobre tratamiento, profundidad, notación o progresión.

### Fuentes complementarias

Las fuentes de `libros/complementarios/` se utilizan cuando aporten valor
específico, especialmente para:

- progresión pedagógica;
- explicaciones alternativas;
- ejemplos;
- aplicaciones;
- ejercicios;
- tratamiento escolar o preuniversitario.

No es obligatorio consultar todas las fuentes complementarias para cada tema.

## Paso 6. Realizar la tarea

Aplicar conjuntamente:

- estas reglas generales;
- las instrucciones especializadas;
- el estado registrado en `pendientes.md`;
- las convenciones ya utilizadas en el tema;
- las fuentes bibliográficas pertinentes.

## Paso 7. Verificar

Antes de considerar terminada una modificación, comprobar según corresponda:

- Física;
- Matemáticas;
- unidades;
- dimensiones;
- signos;
- vectores;
- resultados numéricos;
- notación;
- LaTeX;
- rutas;
- referencias;
- versiones;
- compilación.

## Paso 8. Actualizar `pendientes.md`

Cuando la tarea cambie realmente el estado del proyecto, actualizar:

```text
pendientes.md
```

con el nuevo estado y el punto exacto de continuación.

---

# 7. Función de `pendientes.md`

`pendientes.md` registra exclusivamente el estado del proyecto.

Debe contener información como:

- componente terminado;
- componente pendiente;
- material migrado;
- material todavía no migrado;
- comprobaciones realizadas;
- comprobaciones pendientes;
- punto de continuación;
- saltos temporales;
- numeraciones provisionales cuando correspondan.

No trasladar a `pendientes.md` las reglas permanentes del proyecto.

Las reglas permanentes pertenecen a:

```text
AGENTS.md
```

o a:

```text
instrucciones/
```

Cuando se complete una tarea importante, actualizar `pendientes.md` de manera
concreta.

Registrar:

```text
qué se terminó
qué se revisó
qué se migró
qué se comprobó
qué falta
dónde se encuentra
qué sigue
```

No declarar un componente terminado si todavía existen comprobaciones
esenciales pendientes.

---

# 8. Índice maestro y continuidad

Debe respetarse el índice maestro aprobado del proyecto.

No alterar arbitrariamente:

- orden conceptual;
- numeración de partes;
- numeración de capítulos;
- distribución entre volúmenes;
- nombres consolidados de capítulos.

Los saltos temporales realizados para preparar clases no modifican la secuencia
general de la obra.

Si se trabaja temporalmente en un capítulo posterior, debe mantenerse la
numeración correspondiente al índice maestro.

No renumerar capítulos para hacer coincidir el orden temporal de trabajo con el
orden editorial.

---

# 9. Fuentes bibliográficas

La carpeta:

```text
libros/
```

contiene las referencias bibliográficas principales del proyecto.

Estas fuentes deben consultarse realmente cuando se desarrolla contenido.

No basta con conocer de memoria un tema o mencionar una bibliografía sin
haberla utilizado.

Entre las fuentes centrales del proyecto se encuentran:

- Schaum / Bueche y Hecht;
- Serway y Jewett, volúmenes 1 y 2;
- Sears y Zemansky / Young y Freedman, volúmenes 1 y 2;
- Bauer y Westfall, volúmenes 1 y 2;
- Serway y Vuille, volúmenes 1 y 2;
- Walter Pérez Terrell, volúmenes I y II;
- Juan A. Cuéllar, volúmenes I y II;
- Hipertexto Física 1 y 2;
- Investiguemos Física 10 y 11.

Los nombres exactos de los archivos deben obtenerse de `libros/`.

No modificar los PDF originales.

---

# 10. Uso de las fuentes

Las fuentes deben utilizarse comparativamente.

Cuando se desarrolla un tema, revisar cuando sea pertinente:

- orden de presentación;
- profundidad;
- definiciones;
- leyes;
- principios;
- modelos;
- hipótesis;
- notación;
- deducciones;
- ejemplos;
- métodos de resolución;
- aplicaciones;
- problemas;
- progresión pedagógica.

No seguir mecánicamente un único libro.

Como criterio general:

- Schaum puede orientar una división granular y práctica de los temas;
- Serway, Sears-Zemansky y Bauer-Westfall pueden orientar profundidad, rigor,
  conexiones conceptuales y tratamiento universitario;
- Serway-Vuille puede aportar una progresión intermedia y estrategias de
  resolución;
- los textos escolares pueden aportar progresión pedagógica, ejemplos,
  contextos y aproximaciones accesibles.

Esta orientación no obliga a copiar la organización de ninguna obra.

El resultado debe integrarse coherentemente con el índice propio del proyecto.

---

# 11. Consulta eficiente de los libros

No intentar leer íntegramente todos los libros para cada tema.

Antes de desarrollar contenido:

1. identificar el tema solicitado;
2. localizar los capítulos, secciones o apartados pertinentes en varias
   fuentes;
3. consultar esas partes;
4. comparar sus tratamientos;
5. determinar la cobertura apropiada para el proyecto.

Cuando un PDF tenga problemas de extracción de texto, utilizar los medios
disponibles para inspeccionar las páginas pertinentes antes de descartarlo.

No afirmar que una fuente no contiene un tema únicamente porque una búsqueda
textual simple no produzca resultados.

---

# 12. Originalidad

El contenido final debe ser original.

No copiar extensamente:

- párrafos;
- explicaciones;
- ejemplos;
- ejercicios;
- tablas;
- soluciones;
- figuras;
- estructuras textuales particulares

de una fuente.

Las fuentes se utilizan para:

- investigar;
- comparar;
- verificar;
- seleccionar profundidad;
- contrastar métodos;
- comprobar terminología;
- inspirar la progresión pedagógica.

La redacción, organización local, ejemplos y ejercicios del proyecto deben ser
propios salvo que se indique expresamente lo contrario.

---

# 13. Discrepancias entre fuentes

Las fuentes pueden utilizar:

- convenciones diferentes;
- símbolos diferentes;
- aproximaciones diferentes;
- niveles de profundidad diferentes;
- terminología diferente.

No mezclar estas variantes automáticamente.

Cuando existan discrepancias relevantes:

1. identificar la diferencia;
2. determinar cuál formulación es físicamente más sólida;
3. comprobar la coherencia con el resto del proyecto;
4. mantener la convención elegida;
5. explicar la discrepancia si resulta pedagógicamente importante.

La coherencia global de la obra tiene prioridad sobre reproducir literalmente
la convención de una fuente particular.

---

# 14. Datos oficiales y constantes

Para:

- Sistema Internacional;
- definiciones metrológicas;
- constantes físicas;
- valores oficialmente establecidos;
- información susceptible de actualización,

utilizar cuando sea necesario fuentes oficiales como:

- BIPM;
- NIST;
- organismos científicos equivalentes.

No sustituir innecesariamente las fuentes bibliográficas del proyecto con
búsquedas generales de Internet.

Las fuentes externas deben utilizarse cuando aporten verificación o información
que los libros no puedan proporcionar adecuadamente.

---

# 15. Teoría

Los archivos:

```text
teoria.tex
```

constituyen el material principal para aprender y explicar cada tema.

Antes de modificarlos es obligatorio consultar:

```text
instrucciones/teoria.md
```

La teoría debe poder funcionar simultáneamente como:

- material de estudio autónomo;
- base rigurosa del tema;
- guion de clase para el docente.

No debe convertirse en:

- una lista de definiciones;
- un formulario ampliado;
- una colección de ecuaciones;
- una sucesión de ejemplos sin construcción conceptual.

Debe priorizar, cuando corresponda, la conexión:

```text
fenómeno
→ pregunta física
→ intuición
→ concepto
→ magnitudes
→ modelo
→ principio o ley
→ ecuación
→ interpretación
→ representación
→ aplicación
```

Las reglas detalladas se encuentran en:

```text
instrucciones/teoria.md
```

---

# 16. Formularios

Los archivos:

```text
formulario.tex
```

son materiales de consulta rápida.

Antes de modificarlos es obligatorio consultar:

```text
instrucciones/formulario.md
```

Un formulario no es una teoría resumida.

Debe permitir localizar rápidamente:

- conceptos esenciales;
- magnitudes;
- símbolos;
- unidades;
- leyes;
- principios;
- ecuaciones;
- condiciones de aplicación;
- casos especiales;
- relaciones útiles;
- procedimientos breves;
- conversiones;
- advertencias.

Toda ecuación que dependa de determinadas condiciones debe conservar dichas
condiciones.

No reducir el formulario hasta el punto de que una expresión pueda utilizarse
incorrectamente por falta de contexto.

Las reglas detalladas se encuentran en:

```text
instrucciones/formulario.md
```

---

# 17. Ejercicios

Los archivos:

```text
ejercicios.tex
```

contienen los problemas del tema y, mediante los mecanismos de versiones del
proyecto, sus respuestas y explicaciones.

Antes de modificarlos es obligatorio consultar:

```text
instrucciones/ejercicios.md
```

Los ejercicios deben organizarse de forma progresiva.

Como criterio general deben existir tres niveles:

```text
básico
intermedio
avanzado
```

El nivel avanzado no debe definirse simplemente mediante:

- números mayores;
- cuentas más largas;
- expresiones algebraicas artificialmente complicadas.

Debe aumentar principalmente:

- razonamiento físico;
- selección del modelo;
- elección del método;
- combinación de conceptos;
- interpretación;
- autonomía;
- análisis.

---

# 18. Estructura de ejercicios, respuestas y explicaciones

Utilizar los entornos vigentes establecidos por el proyecto.

La estructura actual es:

```latex
\begin{ejercicio}
...
\end{ejercicio}

\begin{respuesta}
...
\end{respuesta}

\begin{explicacion}
...
\end{explicacion}
```

No introducir un entorno alternativo para las soluciones si la configuración
actual establece:

```text
explicacion
```

Mantener un único enunciado.

No duplicar el mismo ejercicio para estudiante, respuestas y docente.

---

# 19. Versiones de ejercicios

El proyecto contempla tres salidas principales para ejercicios:

```text
estudiante
respuestas
docente
```

Su comportamiento debe ser:

```text
estudiante
→ ejercicio

respuestas
→ ejercicio + respuesta breve

docente
→ ejercicio + respuesta breve + explicación desarrollada
```

Los mecanismos condicionales se controlan mediante la configuración global del
proyecto.

No duplicar manualmente los enunciados entre versiones.

No modificar el sistema de versiones sin consultar:

```text
instrucciones/configuracion.md
```

y los archivos correspondientes de:

```text
config/
```

---

# 20. Soluciones desarrolladas

Cuando corresponda, una explicación completa puede incluir:

1. datos;
2. incógnitas;
3. esquema;
4. sistema de referencia;
5. unidades y conversiones;
6. modelo físico;
7. principio o ley;
8. ecuaciones;
9. despeje;
10. sustitución;
11. cálculo;
12. cifras significativas;
13. unidades;
14. signos;
15. dirección y sentido;
16. resultado;
17. interpretación física;
18. comprobación.

No todos los ejercicios necesitan artificialmente los dieciocho apartados.

Debe incluirse lo necesario para que el razonamiento físico sea comprensible.

No ocultar pasos conceptualmente importantes.

No reducir una explicación a una sustitución numérica cuando el problema exige
razonamiento.

---

# 21. Física antes que sustitución

En ejemplos y ejercicios debe identificarse primero el razonamiento físico.

La secuencia deseable es:

```text
situación física
→ modelo
→ principio o ley
→ ecuación
→ álgebra
→ sustitución
→ resultado
→ interpretación
```

Evitar:

```text
datos
→ búsqueda de fórmula
→ sustitución
→ número
```

cuando esto oculte la Física del problema.

---

# 22. Matemáticas

Las matemáticas deben utilizarse como lenguaje de la Física.

Pueden emplearse, según el nivel requerido:

- álgebra;
- geometría;
- trigonometría;
- vectores;
- derivadas;
- integrales;
- ecuaciones diferenciales;
- otras herramientas matemáticas pertinentes.

Cuando una herramienta matemática tenga significado físico importante, debe
explicarse dicho significado.

No convertir innecesariamente un capítulo de Física en un capítulo de
Matemáticas.

Las deducciones deben incluirse cuando:

- expliquen el origen de una relación;
- conecten conceptos;
- aclaren condiciones de validez;
- mejoren la comprensión.

No incluir formalismo únicamente para aumentar artificialmente el nivel.

---

# 23. Sistema Internacional

Utilizar prioritariamente el Sistema Internacional de Unidades.

En LaTeX utilizar los comandos establecidos mediante:

```text
siunitx
```

y la configuración global.

Mantener coherencia en:

- unidades;
- símbolos;
- prefijos;
- notación científica;
- cifras significativas.

No mezclar unidades incompatibles sin conversión explícita.

Cuando sea pertinente, comprobar la homogeneidad dimensional.

---

# 24. Notación

La notación debe mantenerse consistente entre:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

y entre capítulos relacionados.

No cambiar símbolos arbitrariamente.

Antes de introducir un símbolo nuevo, comprobar si el proyecto ya dispone de
una convención para esa magnitud.

Utilizar los comandos globales definidos en:

```text
config/
```

cuando correspondan.

Entre ellos pueden encontrarse comandos para:

```latex
\vect{}
\uvec{}
\ihat
\jhat
\khat
\pdot
\pcross
\dd
\deriv{}{}
\derivdos{}{}
\pderiv{}{}
\SI{}{}
```

No redefinir localmente comandos ya definidos globalmente.

---

# 25. Escalares y vectores

Distinguir siempre entre magnitudes escalares y vectoriales.

No utilizar indistintamente un vector y su magnitud.

Por ejemplo, debe distinguirse entre:

```latex
\vect{F}
```

y:

```latex
F=\norm{\vect{F}}.
```

Cuando se trabaje con vectores, definir según corresponda:

- sistema de referencia;
- origen;
- ejes;
- sentidos positivos;
- componentes;
- magnitud;
- dirección;
- sentido.

---

# 26. Componentes rectangulares

En problemas vectoriales debe priorizarse el método de componentes
rectangulares.

El procedimiento general es:

1. definir los ejes;
2. representar los vectores;
3. obtener las componentes;
4. aplicar la relación física por componentes;
5. resolver;
6. reconstruir magnitud y dirección cuando sea necesario;
7. comprobar el cuadrante y el sentido físico.

Esta directriz es especialmente importante en temas como:

- vectores;
- movimiento en dos dimensiones;
- dinámica;
- fuerzas mecánicas;
- ley de Coulomb;
- campo eléctrico;
- magnetismo.

Los métodos geométricos, incluida la ley de senos o la ley de cosenos, pueden
utilizarse:

- como alternativa;
- como comprobación;
- cuando aporten comprensión;
- cuando resulten especialmente eficientes.

No deben sustituir sistemáticamente el procedimiento vectorial general.

---

# 27. Sistemas de referencia y signos

Los signos no deben memorizarse como reglas independientes del sistema de
referencia.

Antes de utilizarlos debe quedar claro, cuando corresponda:

- origen;
- eje;
- sentido positivo;
- sistema de referencia.

Por ejemplo, no asumir universalmente que:

```text
g es negativa
```

El signo de la aceleración gravitatoria depende del eje elegido.

Aplicar el mismo criterio a:

- posición;
- desplazamiento;
- velocidad;
- aceleración;
- fuerzas;
- campos;
- componentes vectoriales.

---

# 28. Leyes, definiciones y modelos

Debe distinguirse correctamente entre:

- definición;
- ley física;
- principio;
- modelo;
- hipótesis;
- idealización;
- aproximación;
- consecuencia;
- convenio;
- caso particular.

No presentar todas las ecuaciones como si tuvieran el mismo estatus físico.

Cuando sea importante para la comprensión, identificar explícitamente la
naturaleza de una relación.

---

# 29. Condiciones de validez

No presentar una ecuación fuera de su contexto físico.

Siempre que una expresión dependa de condiciones particulares, conservarlas.

Por ejemplo:

- aceleración constante;
- campo uniforme;
- carga puntual;
- pequeñas oscilaciones;
- ausencia de rozamiento;
- resorte ideal;
- régimen lineal;
- sistema aislado;
- gas ideal;
- lente delgada.

No presentar una aproximación como igualdad exacta.

No presentar un caso particular como una ley universal.

---

# 30. Diagramas y gráficas

Utilizar diagramas y gráficas cuando aporten comprensión.

Pueden incluir:

- vectores;
- sistemas de referencia;
- trayectorias;
- diagramas de cuerpo libre;
- campos;
- superficies gaussianas;
- circuitos;
- rayos;
- ondas;
- procesos termodinámicos;
- gráficas de variables físicas.

Deben ser:

- claros;
- rotulados;
- físicamente correctos;
- consistentes con el texto;
- consistentes con los ejes;
- consistentes con los signos;
- consistentes con la notación.

No incluir una figura únicamente como decoración.

---

# 31. Imágenes específicas de un tema

Las imágenes propias de un tema deben almacenarse normalmente en:

```text
tema/imagenes/
```

No dispersar imágenes específicas por carpetas generales si pertenecen
exclusivamente a un tema.

Antes de mover una imagen existente, comprobar sus referencias desde los
archivos LaTeX.

No romper rutas durante una migración.

---

# 32. TikZ y figuras generadas

Cuando una figura pueda construirse adecuadamente mediante TikZ y esto facilite:

- consistencia;
- edición;
- escalabilidad;
- notación;
- integración con LaTeX,

puede preferirse TikZ.

Las figuras deben representar correctamente la Física.

No sacrificar exactitud física para obtener una figura visualmente atractiva.

Comprobar especialmente:

- direcciones de vectores;
- puntos de aplicación;
- ejes;
- ángulos;
- signos;
- etiquetas;
- escalas cualitativas.

---

# 33. Código LaTeX

Todo material definitivo debe producir código LaTeX:

- limpio;
- consistente;
- mantenible;
- legible;
- listo para copiar, compilar y editar.

No añadir comentarios que simplemente repitan un título visible.

Evitar:

```latex
% VELOCIDAD MEDIA
\subsection{Velocidad media}
```

cuando el comentario no tenga función técnica.

Los comentarios deben reservarse para información útil sobre:

- estructura;
- compilación;
- decisiones técnicas;
- rutas;
- mecanismos no evidentes.

---

# 34. Expresiones matemáticas en LaTeX

Mantener compactas las expresiones breves.

Preferir, cuando resulte legible:

```latex
\[ v=v_0+at. \]
```

en lugar de dividir innecesariamente una expresión corta en muchas líneas.

Las ecuaciones largas pueden dividirse cuando esto mejore la legibilidad.

No sacrificar legibilidad únicamente para reducir el número de líneas del
archivo fuente.

---

# 35. Jerarquía LaTeX

Respetar la jerarquía editorial establecida.

Los documentos maestros controlan normalmente niveles como:

```latex
\part{...}
\chapter{...}
```

Los archivos de tema utilizan según corresponda:

```latex
\section{...}
\subsection{...}
\subsubsection{...}
```

No introducir `\chapter` dentro de un archivo de tema si el documento maestro
es responsable de dicho nivel.

No crear numeración artificial de apartados pedagógicos que no la necesitan.

---

# 36. Configuración global

La configuración general se encuentra en:

```text
config/
```

Antes de modificar:

- paquetes;
- colores;
- comandos;
- entornos;
- versiones;
- estilos;
- mecanismos de compilación,

consultar:

```text
instrucciones/configuracion.md
```

y revisar la configuración existente.

No cargar localmente un paquete si ya se gestiona globalmente sin comprobar
antes las consecuencias.

No redefinir entornos o comandos globales dentro de capítulos individuales.

---

# 37. Documentos maestros

Los documentos maestros organizan las distintas salidas del proyecto.

Pueden existir, entre otros:

```text
volumenes/volumen_X/teoria.tex
volumenes/volumen_X/estudiante.tex
volumenes/volumen_X/respuestas.tex
volumenes/volumen_X/docente.tex
clase.tex
formulario.tex
```

Antes de modificar su estructura debe consultarse:

```text
instrucciones/configuracion.md
```

No incorporar automáticamente todos los capítulos existentes.

La existencia de una carpeta no implica que el tema esté listo para integrarse.

Consultar primero:

```text
pendientes.md
```

---

# 38. Volúmenes

La distribución de capítulos entre volúmenes debe respetar la organización
editorial vigente.

No trasladar un capítulo de volumen sin autorización.

Cada volumen puede disponer de diferentes documentos maestros para:

```text
teoría
estudiante
respuestas
docente
```

Las inclusiones deben conservar la numeración del índice maestro.

---

# 39. `clase.tex`

`clase.tex` se utiliza para preparar temporalmente contenido destinado a una
clase.

Puede seleccionar capítulos o temas sin alterar la organización definitiva de
los volúmenes.

Un salto realizado en:

```text
clase.tex
```

no modifica:

- el índice maestro;
- la numeración definitiva;
- el punto general de desarrollo.

Cuando sea necesario, conservar la numeración mediante los contadores
correspondientes.

---

# 40. `formulario.tex` maestro

El archivo maestro:

```text
formulario.tex
```

debe integrar los formularios correspondientes según la organización vigente
del proyecto.

No confundir este documento maestro con los archivos locales:

```text
tema/formulario.tex
```

Los formularios locales contienen el contenido del tema.

El documento maestro organiza su compilación conjunta.

---

# 41. Migración de material antiguo

El proyecto se encuentra en proceso de migración.

La existencia de material en una estructura anterior no significa que deba
copiarse directamente a la nueva.

Al migrar un tema:

1. localizar el archivo original;
2. revisar su contenido;
3. consultar las instrucciones actuales;
4. adaptar la teoría;
5. adaptar o crear el formulario;
6. adaptar o crear los ejercicios;
7. adaptar los entornos antiguos;
8. trasladar imágenes cuando corresponda;
9. revisar símbolos;
10. revisar unidades;
11. revisar sistemas de referencia;
12. revisar componentes vectoriales;
13. revisar rutas;
14. comprobar compilación;
15. integrar en el documento maestro correspondiente;
16. actualizar `pendientes.md`.

No eliminar inmediatamente el material antiguo.

Solo debe considerarse reemplazado cuando se haya comprobado que la nueva
versión:

- contiene lo necesario;
- respeta las convenciones actuales;
- compila;
- está correctamente integrada.

---

# 42. No confundir existencia con migración

Una carpeta o archivo vacío creado de antemano no significa que el contenido
esté migrado.

Un tema solo debe considerarse migrado cuando su contenido real haya sido
trasladado y adaptado a la arquitectura actual.

Un tema solo debe considerarse revisado cuando haya sido comprobado conforme a
las instrucciones vigentes.

Un tema solo debe considerarse completo cuando se cumplan los criterios
establecidos para todos sus componentes.

---

# 43. Criterio de tema completo

Como regla general, un tema se considera completo cuando están terminados y
revisados los componentes previstos:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

y cuando las comprobaciones correspondientes hayan sido realizadas.

Si algún componente no aplica al tema, debe registrarse expresamente en:

```text
pendientes.md
```

No declarar un tema completo simplemente porque exista su teoría.

---

# 44. Verificación física

Antes de entregar contenido nuevo o modificado, revisar especialmente:

- leyes utilizadas;
- principios;
- hipótesis;
- modelos;
- condiciones de validez;
- signos;
- dirección;
- sentido;
- carácter escalar o vectorial;
- sistemas de referencia;
- unidades;
- dimensiones;
- aproximaciones;
- resultados;
- casos límite cuando sean pertinentes.

No conservar un error simplemente porque aparezca en una versión anterior.

Si se detecta un error físico, debe corregirse respetando la estructura del
proyecto.

---

# 45. Verificación matemática

Comprobar cuando corresponda:

- álgebra;
- trigonometría;
- geometría;
- derivadas;
- integrales;
- ecuaciones diferenciales;
- vectores;
- exponentes;
- signos;
- despejes;
- sustituciones;
- resultados numéricos.

Las matemáticas deben ser coherentes con las hipótesis físicas utilizadas.

---

# 46. Verificación numérica

Los cálculos de ejemplos, respuestas y explicaciones deben comprobarse antes de
considerar terminado el contenido.

Verificar:

- conversiones;
- operaciones;
- unidades;
- redondeo;
- cifras significativas;
- signo;
- orden de magnitud;
- coherencia física.

Cuando un ejercicio incluya varios apartados, comprobar la dependencia entre
resultados intermedios.

No asumir que un resultado previo es correcto únicamente porque ya estaba
escrito en el proyecto.

---

# 47. Compilación

Cuando una tarea modifique archivos LaTeX de forma significativa, comprobar la
compilación cuando el entorno de trabajo lo permita.

La comprobación debe buscar al menos:

- errores de LaTeX;
- comandos inexistentes;
- entornos inexistentes;
- rutas incorrectas;
- imágenes ausentes;
- referencias rotas;
- conflictos de paquetes;
- problemas producidos por versiones;
- desbordamientos importantes.

No modificar la configuración global únicamente para silenciar un error local
sin comprender primero su causa.

---

# 48. Archivos auxiliares de compilación

Los archivos generados por LaTeX, como:

```text
*.aux
*.log
*.out
*.fls
*.fdb_latexmk
*.synctex.gz
*.toc
```

no constituyen contenido fuente de la obra.

No utilizarlos como referencia editorial.

No editarlos manualmente.

No confundir su presencia con archivos que deban mantenerse como parte del
contenido.

---

# 49. PDF

No generar PDF automáticamente cuando la tarea solicite únicamente código
LaTeX.

Si se solicita:

```text
dame el código
```

la salida esperada es el código fuente.

Generar PDF únicamente cuando:

- se solicite expresamente;
- sea necesario para una comprobación visual autorizada;
- forme parte explícita de la tarea.

Una compilación de comprobación no implica necesariamente que deba conservarse
o entregarse un PDF.

---

# 50. Revisión visual

Cuando se genere un documento destinado a distribución o impresión, revisar
cuando sea posible:

- saltos de página;
- ecuaciones cortadas;
- tablas;
- figuras;
- pies de figura;
- títulos;
- cajas;
- espacios;
- encabezados;
- desbordamientos;
- legibilidad general.

La ausencia de errores de compilación no garantiza por sí sola una buena
maquetación.

---

# 51. Cambios mínimos y controlados

Al realizar una tarea concreta, modificar únicamente los archivos necesarios.

No aprovechar una corrección local para realizar una refactorización amplia no
solicitada.

No cambiar por preferencia personal:

- nombres;
- terminología;
- estructura;
- colores;
- estilos;
- comandos;
- entornos;
- numeración.

Si se detecta una mejora estructural importante fuera del alcance de la tarea,
puede proponerse, pero no aplicarse automáticamente si altera decisiones
consolidadas.

---

# 52. Conservación de decisiones previas

Antes de cambiar una decisión existente, comprobar si fue establecida
deliberadamente.

Una convención repetida en varios archivos puede formar parte de una decisión
global.

No sustituirla únicamente porque exista otra forma igualmente válida.

La coherencia de la colección tiene prioridad sobre preferencias locales.

---

# 53. Corrección de errores

Sí deben corregirse errores claros de:

- Física;
- Matemáticas;
- dimensiones;
- unidades;
- signos;
- ortografía;
- tipografía;
- LaTeX;
- referencias;
- rutas.

Si corregir un error obliga a modificar una decisión estructural consolidada,
explicar primero el problema y proponer la modificación.

---

# 54. Terminología

Mantener terminología física consistente en toda la colección.

Cuando existan varios nombres válidos para un concepto:

1. seleccionar una denominación principal;
2. mencionar una alternativa si aporta valor;
3. mantener después la denominación principal.

No cambiar de término entre teoría, formulario y ejercicios sin motivo.

---

# 55. Progresión pedagógica

El proyecto no está limitado por defecto a un único grado escolar.

La profundidad debe determinarse por:

- posición del tema dentro de la obra;
- conocimientos previos;
- importancia conceptual;
- rigor necesario;
- utilidad pedagógica.

Cuando el usuario solicite expresamente material para un grado o nivel
particular, adaptar:

- dificultad;
- matemáticas;
- ejemplos;
- ejercicios;
- extensión;
- lenguaje

sin alterar innecesariamente el contenido general permanente del proyecto.

---

# 56. Conexiones entre capítulos

Cada tema debe integrarse con el resto de la obra.

Cuando corresponda, señalar brevemente:

```text
qué se conoce
→ qué problema aparece
→ qué nuevo concepto se necesita
→ qué permite explicar
→ hacia qué tema conduce
```

No repetir capítulos anteriores completos.

No desarrollar anticipadamente capítulos posteriores completos.

Utilizar conexiones únicamente cuando mejoren la continuidad conceptual.

---

# 57. Errores frecuentes

Cuando un error conceptual sea importante, debe señalarse.

No limitarse a decir que una afirmación es incorrecta.

Cuando sea pedagógicamente útil, explicar:

1. cuál es el error;
2. por qué es incorrecto;
3. cuál es la interpretación correcta.

No saturar el material con advertencias triviales.

---

# 58. Ejemplos y ejercicios

Los ejemplos de la teoría y los ejercicios de práctica cumplen funciones
diferentes.

Los ejemplos de:

```text
teoria.tex
```

forman parte de la enseñanza del concepto.

Los problemas de:

```text
ejercicios.tex
```

permiten practicar, consolidar, integrar y evaluar.

La existencia de ejercicios no elimina la necesidad de ejemplos pedagógicos en
la teoría.

---

# 59. Problemas originales

Los ejercicios nuevos deben ser originales.

Pueden inspirarse en:

- tipos de problemas;
- contextos;
- niveles;
- progresiones;
- métodos

observados en las fuentes.

No copiar mecánicamente un problema de un libro cambiando únicamente los
números.

Buscar variedad en:

- contexto;
- incógnitas;
- razonamiento;
- representaciones;
- métodos;
- interpretación.

---

# 60. Dificultad de los ejercicios

La dificultad debe aumentar por razonamiento, no simplemente por carga de
cálculo.

## Básico

Puede trabajar:

- reconocimiento;
- conceptos;
- unidades;
- interpretación;
- aplicación directa;
- lectura de gráficas sencillas.

## Intermedio

Puede requerir:

- varios pasos;
- selección de relaciones;
- combinación de conceptos;
- conversiones;
- análisis dimensional;
- interpretación de resultados.

## Avanzado

Puede requerir:

- elección autónoma del modelo;
- selección del método;
- combinación de principios;
- deducciones;
- análisis conceptual;
- análisis matemático;
- comparación de métodos;
- problemas inversos;
- interpretación profunda.

---

# 61. Representaciones múltiples

Cuando aporten comprensión, conectar diferentes representaciones de un mismo
fenómeno:

- verbal;
- algebraica;
- vectorial;
- gráfica;
- geométrica;
- diagramática;
- numérica.

El estudiante debe aprender a pasar de una representación a otra.

No incluir representaciones redundantes si no aportan información.

---

# 62. Uso de cálculo

El cálculo diferencial e integral debe utilizarse cuando mejore la comprensión
o sea necesario para la formulación correcta.

No evitarlo artificialmente si el nivel conceptual del tema lo requiere.

Tampoco introducirlo únicamente para hacer parecer el tratamiento más
avanzado.

Cuando se utilice:

```latex
v_x=\deriv{x}{t}
```

explicar su significado físico como tasa instantánea de cambio.

Cuando se utilice una integral, relacionarla con la acumulación física
correspondiente.

---

# 63. Casos especiales y casos límite

Los casos especiales importantes deben derivarse preferentemente del modelo
general.

Evitar enseñar cada caso como una fórmula aislada si puede entenderse como
consecuencia de una relación más general.

Cuando aporte comprensión, analizar casos límite para comprobar que una
expresión tenga sentido físico.

---

# 64. Homogeneidad entre componentes

Al terminar un tema, revisar la coherencia entre:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

Comprobar especialmente:

- mismos símbolos;
- mismas convenciones;
- mismas unidades;
- mismos sistemas de referencia;
- mismas condiciones de validez;
- terminología consistente;
- nivel conceptual compatible.

No permitir que el formulario contradiga la teoría o que los ejercicios
utilicen convenciones diferentes sin explicación.

---

# 65. Integración con capítulos anteriores

Antes de introducir nuevamente una definición o herramienta, comprobar si ya
fue establecida.

Si el lector necesita un recordatorio, proporcionar únicamente lo necesario.

Evitar repetir desarrollos completos sin motivo.

Esto ayuda a mantener la colección progresiva y evita convertir cada capítulo
en un documento aislado.

---

# 66. Revisión de material existente

Cuando se solicite revisar un archivo existente, no limitarse a corregir
errores de sintaxis.

Revisar según el alcance solicitado:

- cobertura conceptual;
- rigor físico;
- rigor matemático;
- coherencia con las instrucciones;
- notación;
- unidades;
- pedagogía;
- ejemplos;
- ejercicios;
- condiciones de validez;
- LaTeX.

Si el archivo ya cumple un criterio, conservarlo.

No reescribir por reescribir.

---

# 67. Trabajo con archivos completos

Cuando se solicite:

```text
dame el código completo
```

debe entregarse el contenido completo que debe tener el archivo solicitado, no
únicamente un parche o fragmento, salvo que el usuario indique lo contrario.

El código debe poder copiarse y pegarse directamente.

Cuando se solicite únicamente modificar una sección concreta, puede entregarse
el fragmento correspondiente si eso es lo más útil.

---

# 68. No inventar estado del proyecto

No afirmar que:

- un archivo existe;
- un archivo está completo;
- un capítulo está migrado;
- una compilación fue exitosa;
- una revisión fue realizada;
- una imagen está disponible

sin haberlo comprobado o sin que esté registrado de forma fiable.

Si falta información, consultar los archivos del proyecto antes de asumirla.

---

# 69. No inventar contenido de archivos

Cuando una tarea dependa del contenido de un archivo del repositorio, leer ese
archivo.

No inferir su contenido únicamente por:

- nombre;
- ruta;
- estructura habitual;
- contenido de otro capítulo.

Esto es especialmente importante para:

```text
pendientes.md
instrucciones/
config/
volumenes/
```

---

# 70. Prioridad de instrucciones

En caso de aparente conflicto, utilizar el siguiente orden de interpretación
dentro del proyecto:

1. instrucciones expresas de la tarea actual;
2. `AGENTS.md`;
3. instrucciones especializadas de `instrucciones/`;
4. estado registrado en `pendientes.md`;
5. convenciones consolidadas del proyecto;
6. contenido existente del tema;
7. preferencias editoriales generales.

Sin embargo, una instrucción puntual no debe interpretarse automáticamente
como autorización para alterar de manera permanente el índice maestro o la
arquitectura general.

Cuando exista un conflicto real entre documentos del proyecto, señalarlo antes
de realizar un cambio estructural irreversible.

---

# 71. Flujo recomendado para crear un tema

Para desarrollar un tema nuevo:

```text
1. leer AGENTS.md
2. leer pendientes.md
3. localizar el tema en el índice maestro
4. leer las instrucciones específicas
5. revisar capítulos anteriores relacionados
6. localizar las secciones pertinentes en libros/
7. consultar varias fuentes
8. comparar enfoques
9. definir cobertura y progresión
10. desarrollar teoria.tex
11. revisar teoría
12. desarrollar formulario.tex
13. revisar coherencia teoría-formulario
14. desarrollar ejercicios.tex
15. comprobar respuestas y explicaciones
16. verificar notación y unidades
17. comprobar LaTeX
18. compilar cuando corresponda
19. integrar en documentos maestros
20. actualizar pendientes.md
```

No considerar automáticamente obligatorio desarrollar los tres componentes en
una sola tarea si el usuario ha solicitado trabajar solamente en uno.

---

# 72. Flujo recomendado para continuar un tema

Para continuar trabajo existente:

```text
1. leer pendientes.md
2. identificar el punto exacto de continuación
3. abrir el componente existente
4. leer sus instrucciones específicas
5. revisar las decisiones ya tomadas
6. consultar las fuentes necesarias
7. continuar sin duplicar lo terminado
8. verificar el nuevo contenido
9. actualizar pendientes.md cuando cambie el estado
```

No comenzar nuevamente desde cero salvo que se haya decidido expresamente
rehacer el componente.

---

# 73. Flujo recomendado para migrar

Para migrar contenido antiguo:

```text
1. consultar pendientes.md
2. localizar origen y destino
3. leer instrucciones actuales
4. revisar el contenido antiguo
5. identificar material reutilizable
6. adaptar estructura y entornos
7. corregir errores detectados
8. mantener contenido válido
9. revisar notación y unidades
10. revisar vectores y signos
11. mover o adaptar imágenes
12. comprobar rutas
13. compilar
14. integrar
15. actualizar pendientes.md
16. conservar temporalmente el original hasta verificar la migración
```

Migrar no significa copiar archivos sin revisión.

---

# 74. Flujo recomendado para revisar ejercicios

Al revisar ejercicios:

```text
1. comprobar el enunciado
2. comprobar que tenga solución bien definida
3. comprobar los datos
4. comprobar unidades
5. resolver independientemente
6. comparar con la respuesta escrita
7. comprobar la explicación
8. comprobar signos
9. comprobar vectores
10. comprobar cifras significativas cuando correspondan
11. comprobar interpretación física
12. comprobar nivel de dificultad
13. comprobar versión estudiante/respuestas/docente
```

En problemas vectoriales, revisar especialmente el uso de componentes
rectangulares.

---

# 75. Actualización final de `pendientes.md`

Después de una tarea que cambie el estado del proyecto, registrar la
actualización de forma precisa.

Una entrada útil debe permitir que una futura sesión determine inmediatamente:

```text
qué se hizo
qué archivo se modificó
qué se comprobó
qué falta
cuál es el siguiente paso
```

Evitar entradas vagas como:

```text
se avanzó bastante
```

o:

```text
casi terminado
```

Utilizar estados concretos.

---

# 76. Qué no debe hacer el agente

Salvo instrucción expresa, no:

- cambiar el índice maestro;
- renumerar capítulos;
- cambiar la distribución entre volúmenes;
- modificar la arquitectura general;
- eliminar material antiguo durante una migración no verificada;
- cambiar nombres consolidados de archivos o carpetas;
- modificar PDF de `libros/`;
- copiar extensamente las fuentes;
- inventar contenido de una fuente no consultada;
- inventar el estado de un archivo;
- introducir convenciones nuevas sin comprobar las existentes;
- redefinir comandos globales localmente;
- cambiar símbolos arbitrariamente;
- modificar configuración global para solucionar apresuradamente un problema
  local;
- duplicar enunciados para crear las versiones estudiante, respuestas y
  docente;
- considerar un tema terminado solo porque exista un archivo;
- considerar una carpeta vacía como contenido migrado;
- generar un PDF cuando solo se haya solicitado código LaTeX;
- introducir complejidad matemática que no aporte comprensión;
- reducir una explicación física a sustitución numérica;
- utilizar una fórmula sin considerar sus condiciones de validez;
- asumir signos sin establecer el sistema de referencia;
- tratar vectores como escalares;
- hacer cambios extensos no relacionados con la tarea solicitada.

---

# 77. Qué debe hacer el agente ante una posible mejora estructural

Si durante una tarea se detecta una mejora que implique cambiar:

- estructura de carpetas;
- arquitectura documental;
- nombres de archivos;
- macros globales;
- entornos;
- sistema de versiones;
- índice maestro;
- distribución de volúmenes;
- una convención consolidada,

no realizar automáticamente el cambio.

En su lugar:

1. identificar el problema;
2. explicar por qué la modificación podría mejorar el proyecto;
3. indicar qué archivos se verían afectados;
4. señalar posibles consecuencias;
5. solicitar aprobación antes de aplicar el cambio.

Las correcciones locales que no alteren decisiones consolidadas pueden
realizarse normalmente.

---

# 78. Principio final

Toda modificación debe contribuir a que la colección se comporte como una obra
unitaria.

Antes de considerar terminado cualquier contenido, comprobar:

```text
¿es físicamente correcto?
¿es matemáticamente correcto?
¿se entiende?
¿explica el significado físico?
¿respeta las condiciones de validez?
¿usa correctamente unidades y vectores?
¿es coherente con los capítulos anteriores?
¿respeta las instrucciones del proyecto?
¿es coherente con teoría, formulario y ejercicios?
¿el código LaTeX es limpio y mantenible?
¿se verificaron los cálculos necesarios?
¿se comprobó la compilación cuando correspondía?
¿el estado quedó correctamente registrado?
```

La meta no es producir contenido rápidamente.

La meta es construir una colección de Física rigurosa, pedagógica, coherente,
progresiva y mantenible.