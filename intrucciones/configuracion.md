# Configuración general del proyecto de Física

Este documento describe la arquitectura, organización técnica, convenciones
LaTeX y decisiones estructurales permanentes del proyecto de Física.

Su función es responder principalmente a la pregunta:

> ¿Cómo está construido y organizado técnicamente el proyecto?

Las reglas generales que debe seguir cualquier agente que trabaje sobre el
repositorio se encuentran en:

```text
AGENTS.md
```

Los criterios especializados se encuentran en:

```text
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

El estado actual del proyecto se encuentra en:

```text
pendientes.md
```

No duplicar innecesariamente entre estos documentos información que ya tenga
un lugar específico.

---

# 1. Función de este documento

`instrucciones/configuracion.md` registra decisiones permanentes relacionadas
con:

- arquitectura del repositorio;
- organización de capítulos;
- organización de volúmenes;
- configuración compartida de LaTeX;
- paquetes;
- colores;
- comandos;
- estilos;
- entornos;
- versiones;
- documentos maestros;
- rutas;
- imágenes;
- agregadores;
- numeración;
- compilación;
- migración estructural.

No debe utilizarse para registrar:

- el tema actualmente activo;
- componentes terminados;
- componentes pendientes;
- punto exacto de continuación;
- saltos temporales;
- progreso cotidiano.

Esa información pertenece a:

```text
pendientes.md
```

Tampoco debe repetir en detalle los criterios para desarrollar teoría,
formularios o ejercicios.

Esos criterios pertenecen a:

```text
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

---

# 2. Estructura general del proyecto

La estructura principal actual es:

```text
Fisica/
│
├── AGENTS.md
├── pendientes.md
│
├── capitulos/
├── config/
├── instrucciones/
├── libros/
├── recursos/
├── volumenes/
│
├── clase.tex
└── formulario.tex
```

La función general de cada elemento es:

```text
AGENTS.md
→ reglas generales para agentes y herramientas de IA

pendientes.md
→ estado actual y punto exacto de continuación

capitulos/
→ contenido físico real de la colección

config/
→ configuración LaTeX compartida

instrucciones/
→ documentación especializada del proyecto

libros/
→ fuentes bibliográficas

recursos/
→ recursos compartidos entre varios temas

volumenes/
→ documentos maestros de publicación

clase.tex
→ documento maestro independiente para preparar clases

formulario.tex
→ documento maestro independiente de formularios
```

Puede existir temporalmente una carpeta:

```text
teoria/
```

correspondiente a la estructura anterior.

Mientras continúe la migración, esa carpeta no debe utilizarse como modelo para
crear contenido nuevo.

No eliminarla automáticamente.

Su contenido debe migrarse progresivamente siguiendo el procedimiento
establecido en este documento y en `AGENTS.md`.

---

# 3. Carpeta `instrucciones`

La documentación especializada se encuentra en:

```text
instrucciones/
```

Su estructura principal es:

```text
instrucciones/
├── configuracion.md
├── teoria.md
├── formulario.md
└── ejercicios.md
```

Las responsabilidades son:

| Archivo | Función |
|---|---|
| `configuracion.md` | Arquitectura, organización y funcionamiento técnico |
| `teoria.md` | Criterios para desarrollar `teoria.tex` |
| `formulario.md` | Criterios para desarrollar `formulario.tex` |
| `ejercicios.md` | Criterios para desarrollar `ejercicios.tex` |

El estado del proyecto no pertenece a esta carpeta.

Se mantiene en:

```text
pendientes.md
```

en la raíz del repositorio.

---

# 4. Carpeta `config`

La carpeta:

```text
config/
```

contiene la configuración compartida por todos los documentos LaTeX.

Su estructura es:

```text
config/
├── configuracion.tex
├── paquetes.tex
├── colores.tex
├── comandos.tex
├── estilos.tex
├── entornos.tex
└── versiones.tex
```

Cada archivo tiene una responsabilidad específica.

No concentrar toda la configuración en un único archivo.

No colocar contenido físico dentro de `config/`.

---

# 5. `config/configuracion.tex`

Es el punto central de carga de la configuración compartida.

Debe proporcionar una ruta raíz por defecto mediante:

```latex
\providecommand{\rutaraiz}{.}
```

y cargar los módulos en este orden:

```latex
\input{\rutaraiz/config/paquetes}
\input{\rutaraiz/config/colores}
\input{\rutaraiz/config/comandos}
\input{\rutaraiz/config/estilos}
\input{\rutaraiz/config/entornos}
\input{\rutaraiz/config/versiones}
```

El orden debe conservarse porque algunos módulos dependen de definiciones
realizadas anteriormente.

`configuracion.tex` no debe contener:

- teoría;
- fórmulas físicas específicas de un tema;
- ejercicios;
- contenido editorial de capítulos.

Su función es exclusivamente técnica.

---

# 6. Sistema de rutas mediante `\rutaraiz`

Los documentos maestros deben definir:

```latex
\newcommand{\rutaraiz}{...}
```

antes de cargar:

```latex
\input{\rutaraiz/config/configuracion}
```

El valor depende de la profundidad del documento respecto de la raíz.

Por ejemplo, un documento ubicado directamente en la raíz puede utilizar:

```latex
\newcommand{\rutaraiz}{.}
```

Un documento situado en:

```text
volumenes/volumen_1/
```

puede requerir:

```latex
\newcommand{\rutaraiz}{../..}
```

La ruta debe calcularse desde el archivo que se compila.

No escribir rutas absolutas del sistema operativo.

Evitar construcciones como:

```text
C:/...
D:/...
/home/usuario/...
```

Los documentos deben permanecer portables.

---

# 7. `config/paquetes.tex`

Contiene únicamente los paquetes generales utilizados por el proyecto.

Puede incluir paquetes relacionados con:

- idioma;
- codificación;
- tipografía;
- matemáticas;
- unidades;
- tablas;
- imágenes;
- TikZ;
- PGFPlots;
- circuitos;
- listas;
- cajas;
- encabezados;
- referencias;
- hipervínculos;
- otras necesidades generales.

No colocar aquí:

- comandos propios del proyecto;
- entornos pedagógicos;
- contenido físico;
- estilos específicos de un capítulo.

Antes de añadir un paquete nuevo debe comprobarse si:

1. ya está cargado;
2. otro paquete proporciona la misma funcionalidad;
3. puede producir conflictos;
4. realmente es necesario globalmente.

Si un paquete se necesita únicamente para una situación excepcional, evaluar
antes si debe formar parte de la configuración global.

---

# 8. `babel` y TikZ

Para evitar conflictos entre `babel` y TikZ se utiliza la configuración:

```latex
\usepackage[
    spanish,
    es-nodecimaldot,
    es-noshorthands
]{babel}
```

y la biblioteca:

```latex
\usetikzlibrary{babel}
```

No activar nuevamente los `shorthands` de español si esto provoca conflictos
con:

- flechas;
- coordenadas;
- sintaxis TikZ;
- operadores;
- diagramas.

Esta decisión debe mantenerse de forma global salvo que se compruebe una razón
técnica para modificarla.

---

# 9. `hyperref`

`hyperref` debe cargarse como paquete sin depender de colores que todavía no
hayan sido definidos.

La configuración cromática y visual de los hipervínculos pertenece a:

```text
config/estilos.tex
```

No duplicar configuraciones de `hyperref` en documentos individuales.

---

# 10. `config/colores.tex`

Contiene exclusivamente la paleta cromática global.

La paleta principal es:

```latex
\definecolor{AzulPrincipal}{HTML}{1F4E79}
\definecolor{AzulSecundario}{HTML}{5B9BD5}
\definecolor{AzulFondo}{HTML}{EAF3F8}

\definecolor{VerdePrincipal}{HTML}{548235}
\definecolor{VerdeFondo}{HTML}{EEF5E9}

\definecolor{AmarilloPrincipal}{HTML}{BF9000}
\definecolor{AmarilloFondo}{HTML}{FFF7DC}

\definecolor{RojoPrincipal}{HTML}{C00000}
\definecolor{RojoFondo}{HTML}{FCEBEC}

\definecolor{GrisPrincipal}{HTML}{666666}
\definecolor{GrisFondo}{HTML}{F2F2F2}

\definecolor{TextoPrincipal}{HTML}{222222}

\colorlet{ColorTitulos}{RojoPrincipal}
```

No redefinir estos colores localmente dentro de capítulos.

Si se necesita un color nuevo de uso global, añadirlo deliberadamente a
`colores.tex`.

---

# 11. Sistema pedagógico de colores

La convención general es:

| Color | Uso principal |
|---|---|
| Azul | Definiciones, principios, leyes, modelos, fórmulas, condiciones e ideas fundamentales |
| Verde | Ejemplos, aplicaciones y explicaciones desarrolladas |
| Amarillo | Consejos, estrategias, pistas y ayudas |
| Rojo | Advertencias, errores frecuentes y títulos principales |
| Gris | Observaciones, recordatorios, notas e información complementaria |

Los colores tienen función pedagógica.

No deben utilizarse únicamente como decoración.

Deben emplearse con moderación y conservar una función reconocible en toda la
colección.

---

# 12. `config/comandos.tex`

Contiene los comandos globales reutilizables.

Puede incluir comandos para:

- datos generales de la obra;
- vectores;
- vectores unitarios;
- producto punto;
- producto cruz;
- valor absoluto;
- norma;
- derivadas;
- derivadas parciales;
- operadores matemáticos;
- operadores vectoriales;
- símbolos frecuentes;
- niveles de ejercicios.

Entre los datos globales pueden definirse comandos como:

```latex
\newcommand{\tituloobra}{Física}
\newcommand{\autorlibro}{Julian David Chavarro Balanta}
```

Los niveles de ejercicios se controlan mediante:

```latex
\nivelbasico
\nivelintermedio
\nivelavanzado
```

Los comandos globales no deben redefinirse localmente sin una razón
justificada.

Antes de crear un comando nuevo debe comprobarse si ya existe una solución
equivalente.

---

# 13. Convenciones vectoriales globales

Cuando estén definidos en `comandos.tex`, deben utilizarse los comandos
globales del proyecto para mantener consistencia.

Entre ellos pueden encontrarse:

```latex
\vect{}
\uvec{}
\ihat
\jhat
\khat
\pdot
\pcross
\norm{}
\abs{}
\dd
\deriv{}{}
\derivdos{}{}
\pderiv{}{}
```

No sustituirlos arbitrariamente por notaciones locales.

Debe distinguirse entre:

```latex
\vect{F}
```

como vector y:

```latex
F=\norm{\vect{F}}
```

como magnitud.

Cuando una modificación de notación global sea necesaria, debe revisarse su
impacto sobre todo el material existente.

---

# 14. `config/estilos.tex`

Controla la apariencia general del proyecto.

Incluye, cuando corresponda:

- partes;
- capítulos;
- secciones;
- subsecciones;
- subsubsecciones;
- encabezados;
- pies de página;
- espaciado;
- listas;
- captions;
- unidades;
- hipervínculos;
- estilos base de `tcolorbox`.

Los títulos principales utilizan:

```text
ColorTitulos
```

actualmente asociado a:

```text
RojoPrincipal
```

No introducir estilos locales diferentes en cada tema salvo que exista una
razón pedagógica o técnica clara.

La identidad visual debe mantenerse en toda la colección.

---

# 15. Regla para `tcolorbox`

Dentro de bloques:

```latex
\tcbset{
    ...
}
```

evitar líneas en blanco que puedan convertirse en:

```latex
\par
```

y provocar errores de `pgfkeys`.

Mantener compactas las definiciones de opciones de `tcolorbox`.

Los estilos compartidos deben definirse globalmente y reutilizarse.

---

# 16. `config/entornos.tex`

Contiene los entornos pedagógicos y físicos compartidos por toda la colección.

Entre ellos pueden encontrarse:

```latex
definicion
principio
leyfisica
modelo
hipotesis
aproximacion
idea
interpretacion
formula
condicion
ejemplo
aplicacion
consejo
estrategia
advertencia
errorfrecuente
observacion
recordatorio
nota
notapedagogica
resumen
```

Los entornos deben mantener una identidad visual común.

Los argumentos opcionales se utilizan normalmente como subtítulo.

Ejemplo:

```latex
\begin{definicion}[Aceleración]
...
\end{definicion}
```

No crear localmente entornos equivalentes con nombres diferentes sin una razón
justificada.

---

# 17. Entornos de ejercicios

El sistema de ejercicios utiliza:

```latex
ejercicio
respuesta
explicacion
```

La estructura fuente habitual es:

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

El nombre oficial del desarrollo completo será:

```text
explicacion
```

No alternarlo arbitrariamente con nombres como:

```text
solucion
soluciondesarrollada
resolucion
```

si estos no forman parte de la configuración vigente.

La respuesta y la explicación deben permanecer asociadas al ejercicio
correspondiente en el código fuente.

---

# 18. `config/versiones.tex`

Controla las distintas salidas del material de ejercicios.

Las tres versiones principales son:

```text
estudiante
respuestas
docente
```

Su comportamiento conceptual es:

```text
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
```

El mecanismo exacto debe permanecer centralizado en:

```text
config/versiones.tex
```

No implementar condicionales independientes en cada capítulo si la
configuración global ya resuelve la selección de contenido.

---

# 19. Un único archivo de ejercicios

Cada tema debe mantener un único:

```text
ejercicios.tex
```

que contenga conjuntamente:

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

Las diferentes salidas se obtienen mediante el sistema de versiones.

No crear copias independientes como:

```text
ejercicios_estudiante.tex
ejercicios_respuestas.tex
ejercicios_docente.tex
```

salvo que en el futuro se adopte expresamente una arquitectura diferente.

Esto evita:

- duplicación;
- desincronización;
- numeraciones distintas;
- correcciones repetidas;
- mantenimiento innecesario.

---

# 20. Carpeta `capitulos`

La carpeta:

```text
capitulos/
```

contiene el contenido físico real de la colección.

La organización general sigue el índice maestro.

Una estructura típica es:

```text
capitulos/
└── NN_parte/
    └── NN_nombre_del_capitulo/
        ├── teoria.tex
        ├── formulario.tex
        ├── ejercicios.tex
        └── imagenes/
```

Los números de carpetas ayudan a conservar:

- orden;
- navegación;
- correspondencia con el índice maestro.

No deben utilizarse para generar automáticamente la numeración editorial.

---

# 21. Contenido de un tema

Cada tema contiene principalmente:

```text
teoria.tex
formulario.tex
ejercicios.tex
imagenes/
```

La función de cada archivo es:

```text
teoria.tex
→ enseñanza y desarrollo conceptual

formulario.tex
→ consulta rápida

ejercicios.tex
→ práctica, respuestas y explicaciones

imagenes/
→ imágenes específicas del tema
```

Los criterios pedagógicos detallados pertenecen a:

```text
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

---

# 22. Archivos de contenido y preámbulo

Los archivos:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

ubicados dentro de los capítulos son fragmentos de contenido.

Por tanto, normalmente no deben contener:

```latex
\documentclass
\begin{document}
\end{document}
```

ni un preámbulo completo.

La configuración pertenece a los documentos maestros.

Esto permite reutilizar el mismo contenido desde distintas salidas.

---

# 23. Jerarquía de títulos

La jerarquía editorial debe mantenerse consistente.

Los documentos maestros controlan normalmente:

```latex
\part{...}
\chapter{...}
```

Los archivos internos utilizan según corresponda:

```latex
\section{...}
\subsection{...}
\subsubsection{...}
```

No introducir:

```latex
\chapter{...}
```

dentro de un archivo de tema si el capítulo ya es creado por el documento
maestro.

La numeración editorial debe controlarse desde el nivel superior apropiado.

---

# 24. Carpeta `imagenes`

Una imagen propia de un tema debe almacenarse normalmente junto al contenido
al que pertenece:

```text
tema/
└── imagenes/
```

Esto incluye imágenes que solo tengan sentido dentro de ese tema.

No almacenar en `recursos/` imágenes utilizadas exclusivamente por un único
tema.

Las rutas deben construirse mediante `\rutaraiz` cuando sea necesario.

---

# 25. Carpeta `recursos`

La carpeta:

```text
recursos/
```

contiene elementos reutilizados por varias partes del proyecto.

Puede incluir:

- imágenes compartidas;
- logotipos;
- elementos gráficos generales;
- recursos editoriales;
- otros archivos de uso transversal.

No utilizarla como depósito indiscriminado de imágenes específicas de temas.

---

# 26. Subdivisión adicional de capítulos

La estructura básica no impide crear subcarpetas adicionales.

Cuando un capítulo sea suficientemente amplio puede subdividirse en temas
independientes.

Por ejemplo:

```text
capitulos/
└── 03_dinamica_y_estatica/
    └── 19_fuerzas_mecanicas_comunes/
        ├── 01_peso/
        ├── 02_fuerza_normal/
        ├── 03_tension/
        └── 04_fuerza_elastica_y_ley_de_hooke/
```

Cada subtema puede contener:

```text
teoria.tex
formulario.tex
ejercicios.tex
imagenes/
```

Otro ejemplo:

```text
capitulos/
└── 11_fisica_termica_y_termodinamica/
    └── 69_dilatacion_termica/
        ├── 01_dilatacion_termica_lineal/
        ├── 02_dilatacion_termica_superficial/
        ├── 03_dilatacion_termica_volumetrica/
        ├── 04_dilatacion_de_liquidos/
        └── 05_dilatacion_anomala_del_agua/
```

No es obligatorio subdividir desde el comienzo todos los capítulos.

La subdivisión debe realizarse cuando aporte:

- claridad conceptual;
- granularidad pedagógica;
- facilidad de mantenimiento;
- coherencia con la progresión del proyecto.

---

# 27. Capítulos contenedores y agregadores

Cuando un capítulo posea varios subtemas independientes puede disponer de
archivos agregadores en su carpeta principal.

Por ejemplo:

```text
19_fuerzas_mecanicas_comunes/
├── teoria.tex
├── formulario.tex
├── ejercicios.tex
├── 01_peso/
├── 02_fuerza_normal/
├── 03_tension/
└── 04_fuerza_elastica_y_ley_de_hooke/
```

Los archivos agregadores pueden reunir los subtemas mediante:

```latex
\input{...}
```

Esto permite que los documentos maestros incluyan el capítulo completo sin
repetir manualmente todas sus rutas.

Los agregadores no deben duplicar contenido.

Su función es ensamblarlo.

---

# 28. Índice maestro

La organización conceptual y numeración de capítulos corresponde al índice
maestro aprobado.

La numeración de los capítulos es continua en toda la colección.

Los números pertenecen al índice maestro, no al volumen editorial.

Por ejemplo:

```text
Volumen I
...
Capítulo 46

Volumen II
Capítulo 47
...
Capítulo 77

Volumen III
Capítulo 78
...
```

Los volúmenes no reinician la numeración.

Los archivos internos de contenido no deben controlar el número del capítulo.

La numeración corresponde a los documentos maestros que ensamblan la obra.

---

# 29. Uso de `\setcounter`

Cuando un documento independiente necesita conservar la numeración del índice
maestro puede configurarse el contador antes del primer capítulo.

Por ejemplo, para comenzar mostrando el capítulo 78:

```latex
\setcounter{chapter}{77}
```

antes de:

```latex
\chapter{Carga eléctrica y electrización}
```

El contador debe configurarse deliberadamente.

No modificarlo dentro de los archivos internos de contenido.

---

# 30. Partes

Las partes de la colección se controlan desde los documentos maestros.

Los archivos internos de contenido no deben introducir:

```latex
\part{...}
```

salvo que exista una razón estructural expresamente establecida.

La jerarquía general es:

```text
obra
→ volumen
→ parte
→ capítulo
→ tema o sección
→ subsección
```

---

# 31. Carpeta `volumenes`

La carpeta:

```text
volumenes/
```

contiene los documentos maestros de publicación.

La estructura general puede ser:

```text
volumenes/
├── volumen_1/
├── volumen_2/
├── volumen_3/
└── ...
```

Cada volumen puede contener documentos maestros como:

```text
teoria.tex
estudiante.tex
respuestas.tex
docente.tex
```

Estos archivos no deben duplicar el contenido físico.

Su función es ensamblar mediante:

```latex
\input{...}
```

los archivos ubicados en:

```text
capitulos/
```

---

# 32. Documento maestro de teoría

El documento:

```text
volumenes/volumen_X/teoria.tex
```

ensambla la teoría correspondiente al volumen.

Debe contener:

- clase documental;
- `\rutaraiz`;
- configuración;
- información del volumen;
- portada o elementos editoriales cuando correspondan;
- partes;
- capítulos;
- `\input` de los archivos de teoría.

No debe contener directamente el desarrollo completo de los temas.

---

# 33. Documento maestro del estudiante

El documento:

```text
volumenes/volumen_X/estudiante.tex
```

ensambla los ejercicios para estudiantes.

Debe activar la versión correspondiente antes de cargar los ejercicios.

La salida del estudiante no debe mostrar:

- respuestas;
- explicaciones desarrolladas.

Las pistas pueden mostrarse cuando las reglas de ejercicios indiquen que
corresponden.

---

# 34. Documento maestro de respuestas

El documento:

```text
volumenes/volumen_X/respuestas.tex
```

ensambla la versión con respuestas breves.

Debe mostrar:

- ejercicios;
- pistas cuando correspondan;
- respuestas.

No debe mostrar las explicaciones completas destinadas a la versión docente.

---

# 35. Documento maestro del docente

El documento:

```text
volumenes/volumen_X/docente.tex
```

ensambla la versión completa.

Debe mostrar:

- ejercicios;
- pistas cuando correspondan;
- respuestas;
- explicaciones desarrolladas.

Las tres versiones deben utilizar el mismo:

```text
ejercicios.tex
```

de cada tema.

---

# 36. `clase.tex`

El archivo:

```text
clase.tex
```

es un documento maestro independiente situado en la raíz.

Su función es permitir preparar y compilar temporalmente contenido destinado a
una clase.

Puede incluir temas fuera de la secuencia actual de desarrollo.

Esto no modifica:

- el índice maestro;
- la numeración definitiva;
- la distribución entre volúmenes;
- el punto general de continuación.

Cuando se compile un capítulo posterior debe conservarse, cuando corresponda,
su numeración real mediante:

```latex
\setcounter{chapter}{...}
```

No duplicar contenido físico dentro de `clase.tex`.

Debe reutilizar los archivos de `capitulos/`.

---

# 37. `formulario.tex` maestro

El archivo:

```text
formulario.tex
```

situado en la raíz es un documento maestro independiente.

Su función es ensamblar formularios de distintos temas.

No debe confundirse con:

```text
capitulos/.../formulario.tex
```

Los archivos locales contienen el contenido.

El archivo maestro organiza la compilación conjunta.

Debe utilizar:

```latex
\input{...}
```

para incluir los formularios correspondientes.

---

# 38. Carpeta `libros`

Las fuentes bibliográficas se almacenan en:

```text
libros/
```

La organización prevista distingue:

```text
libros/
├── principales/
└── complementarios/
```

Las fuentes principales son las que deben consultarse prioritariamente al
desarrollar contenido.

Las complementarias se utilizan cuando aporten:

- otra explicación;
- progresión pedagógica;
- ejemplos;
- aplicaciones;
- ejercicios;
- tratamiento escolar o preuniversitario;
- contraste adicional.

La clasificación concreta de los libros debe mantenerse coherente con
`AGENTS.md`.

Los PDF originales no deben modificarse.

---

# 39. Fuentes principales

La biblioteca principal prevista incluye:

```text
Sears–Zemansky / Young–Freedman, volumen 1
Sears–Zemansky / Young–Freedman, volumen 2

Serway–Jewett, volumen 1
Serway–Jewett, volumen 2

Schaum / Bueche–Hecht

Bauer–Westfall, volumen 1
Bauer–Westfall, volumen 2
```

No es necesario consultar íntegramente todos los libros para cada tema.

Deben localizarse las secciones pertinentes.

La selección y comparación de fuentes se rige por `AGENTS.md`.

---

# 40. Fuentes complementarias

La biblioteca complementaria puede incluir:

```text
Serway–Vuille, volumen 1
Serway–Vuille, volumen 2

Walter Pérez Terrel, volumen I
Walter Pérez Terrel, volumen II

Juan A. Cuéllar, volumen I
Juan A. Cuéllar, volumen II

Hipertexto Física 1
Hipertexto Física 2

Investiguemos Física 10
Investiguemos Física 11
```

No es obligatorio consultar todas estas fuentes para cada tema.

Su uso debe responder a una necesidad concreta.

---

# 41. Sistema Internacional y `siunitx`

Las unidades deben escribirse prioritariamente mediante:

```latex
siunitx
```

cuando la configuración vigente lo permita.

Ejemplos:

```latex
\SI{9.81}{\metre\per\second\squared}
```

```latex
\SI{3.0}{\micro\coulomb}
```

```latex
\SI{25}{\degreeCelsius}
```

No escribir manualmente unidades de formas inconsistentes si existe un comando
normalizado disponible.

La configuración global de `siunitx` pertenece a:

```text
config/estilos.tex
```

o al módulo técnico que corresponda según la arquitectura vigente.

---

# 42. TikZ

TikZ puede utilizarse para:

- vectores;
- sistemas de referencia;
- diagramas de cuerpo libre;
- trayectorias;
- superficies gaussianas;
- campos;
- rayos;
- circuitos;
- esquemas físicos.

Las bibliotecas necesarias deben cargarse globalmente cuando sean de uso
general.

No cargar repetidamente las mismas bibliotecas dentro de cada capítulo.

Las figuras deben ser físicamente correctas.

---

# 43. PGFPlots

PGFPlots puede utilizarse para representar gráficas físicas.

Las gráficas deben:

- rotular ejes;
- indicar magnitudes;
- indicar unidades cuando corresponda;
- utilizar escalas coherentes;
- respetar el sistema de referencia;
- representar correctamente los datos o funciones.

La configuración común debe centralizarse cuando sea reutilizable.

---

# 44. Circuitos

Cuando se desarrollen capítulos de electricidad y circuitos pueden utilizarse
las herramientas de circuitos definidas globalmente.

No introducir paquetes o convenciones de dibujo diferentes en cada capítulo sin
una razón clara.

Las convenciones gráficas deben mantenerse uniformes.

---

# 45. Etiquetas y referencias

Las etiquetas deben ser suficientemente descriptivas para evitar colisiones.

Pueden utilizar prefijos como:

```text
eq:
fig:
tab:
sec:
subsec:
```

Ejemplos:

```latex
\label{eq:movimiento-mru-posicion}
```

```latex
\label{fig:caida-libre-eje-vertical}
```

Evitar etiquetas excesivamente genéricas como:

```latex
\label{ecuacion1}
```

cuando puedan producir conflictos al ensamblar varios capítulos.

---

# 46. Rutas de imágenes

Las rutas de imágenes deben funcionar desde el documento maestro que realiza la
compilación.

Preferir rutas construidas con:

```latex
\rutaraiz
```

cuando sea necesario.

Por ejemplo:

```latex
\includegraphics{
    \rutaraiz/capitulos/02_cinematica/10_caida_libre_y_movimiento_vertical/imagenes/archivo
}
```

La sintaxis concreta puede compactarse en una sola línea cuando resulte más
legible.

No utilizar rutas absolutas del equipo.

---

# 47. Rutas de `\input`

Los documentos maestros deben utilizar rutas explícitas y coherentes.

Ejemplo conceptual:

```latex
\input{
    \rutaraiz/capitulos/02_cinematica/10_caida_libre_y_movimiento_vertical/teoria
}
```

Puede escribirse de forma compacta:

```latex
\input{\rutaraiz/capitulos/02_cinematica/10_caida_libre_y_movimiento_vertical/teoria}
```

si mejora la legibilidad.

No depender del directorio de trabajo accidental del editor.

La ruta debe ser reproducible desde la estructura del proyecto.

---

# 48. Extensión `.tex` en `\input`

La inclusión puede realizarse sin escribir explícitamente:

```text
.tex
```

por ejemplo:

```latex
\input{\rutaraiz/config/configuracion}
```

Esta convención puede mantenerse de forma uniforme.

No alternar arbitrariamente entre rutas con y sin extensión si no existe una
razón técnica.

---

# 49. Numeraciones provisionales

Algunos temas pueden desarrollarse antes de que su organización interna
definitiva esté completamente consolidada.

En esos casos puede utilizarse temporalmente una numeración provisional.

Debe registrarse en:

```text
pendientes.md
```

Antes de convertirla en definitiva deben revisarse:

- carpetas;
- archivos;
- rutas;
- `\input`;
- `label`;
- referencias internas;
- agregadores;
- documentos maestros.

No cambiar arbitrariamente una numeración ya consolidada.

---

# 50. Migración de contenido anterior

Si existe contenido desarrollado antes de la arquitectura actual, su migración
debe realizarse progresivamente.

Al retomar un tema antiguo:

1. localizar el contenido existente;
2. identificar su destino en la nueva estructura;
3. trasladar y revisar la teoría;
4. trasladar y revisar el formulario;
5. trasladar y revisar los ejercicios;
6. trasladar las imágenes específicas a `imagenes/`;
7. adaptar los entornos a las convenciones actuales;
8. comprobar la notación;
9. comprobar las unidades;
10. comprobar las rutas;
11. comprobar la compilación;
12. actualizar los documentos maestros cuando corresponda;
13. actualizar `pendientes.md`.

Migrar no significa copiar mecánicamente el contenido antiguo.

Debe adaptarse a las reglas actuales.

No incluir simultáneamente en la compilación la copia antigua y la nueva del
mismo contenido.

La versión antigua puede conservarse temporalmente como respaldo mientras la
migración no haya sido comprobada.

---

# 51. Coherencia entre componentes

La teoría, el formulario y los ejercicios de un mismo tema deben utilizar:

- los mismos símbolos;
- las mismas unidades;
- las mismas convenciones;
- los mismos nombres de magnitudes;
- los mismos sistemas de referencia cuando corresponda;
- la misma terminología física.

No cambiar arbitrariamente un símbolo entre documentos.

Cuando un cambio de notación sea necesario debe revisarse el tema completo.

---

# 52. Compilación

La estructura debe permitir compilar independientemente los documentos
maestros.

Según corresponda:

```text
volumenes/volumen_X/teoria.tex
volumenes/volumen_X/estudiante.tex
volumenes/volumen_X/respuestas.tex
volumenes/volumen_X/docente.tex
clase.tex
formulario.tex
```

Los archivos internos de capítulos no necesitan ser documentos compilables de
forma independiente.

No añadir preámbulos locales únicamente para permitir compilar un fragmento si
esto rompe la arquitectura compartida.

---

# 53. Comprobación de compilación

Después de modificaciones estructurales o cambios LaTeX importantes debe
comprobarse, cuando el entorno lo permita:

- ausencia de errores;
- rutas;
- imágenes;
- referencias;
- comandos;
- entornos;
- versiones;
- tablas;
- TikZ;
- PGFPlots;
- circuitos;
- hipervínculos;
- encabezados;
- desbordamientos relevantes.

No considerar que un archivo está correctamente integrado únicamente porque su
código parece válido de forma aislada.

---

# 54. Archivos auxiliares

Los archivos producidos automáticamente durante la compilación no forman parte
del contenido fuente.

Entre ellos pueden encontrarse:

```text
*.aux
*.log
*.out
*.toc
*.fls
*.fdb_latexmk
*.synctex.gz
```

No editarlos manualmente.

No utilizarlos como fuente de configuración.

Cuando corresponda, deben excluirse del control de versiones mediante las reglas
del repositorio.

---

# 55. PDF

Los PDF son productos de compilación.

No forman parte del contenido fuente principal salvo que exista una razón
editorial concreta para conservarlos.

Cuando una tarea solicite únicamente código LaTeX, no es necesario generar un
PDF definitivo.

Puede realizarse una compilación temporal para comprobar:

- errores;
- maquetación;
- figuras;
- tablas;
- desbordamientos.

La generación o entrega de un PDF definitivo debe realizarse cuando se solicite
expresamente.

---

# 56. Documentos maestros y contenido físico

Debe mantenerse la separación:

```text
documento maestro
→ organiza

archivo de capítulo
→ contiene el contenido físico
```

Por tanto, evitar desarrollar teoría extensa directamente dentro de:

```text
volumenes/volumen_X/teoria.tex
```

o ejercicios directamente dentro de:

```text
volumenes/volumen_X/estudiante.tex
volumenes/volumen_X/respuestas.tex
volumenes/volumen_X/docente.tex
```

Los documentos maestros deben ensamblar.

Los capítulos deben contener.

---

# 57. Reutilización

La arquitectura debe permitir reutilizar un mismo contenido desde diferentes
documentos.

Por ejemplo:

```text
capitulos/.../teoria.tex
```

puede incluirse desde:

```text
volumenes/volumen_X/teoria.tex
clase.tex
```

sin duplicarlo.

De forma similar:

```text
capitulos/.../formulario.tex
```

puede incluirse desde:

```text
formulario.tex
```

y eventualmente desde otros documentos que lo necesiten.

La reutilización debe realizarse mediante ensamblaje, no mediante copias.

---

# 58. Evitar duplicación

No mantener dos copias activas del mismo contenido.

Si el mismo texto aparece en:

```text
estructura antigua
estructura nueva
```

solo una de ellas debe formar parte de la compilación activa.

Durante la migración puede conservarse la versión antigua como respaldo, pero
no debe ensamblarse simultáneamente.

---

# 59. Modificaciones estructurales

Antes de modificar:

- arquitectura;
- nombres;
- numeración;
- estilos globales;
- colores;
- comandos;
- entornos;
- división en volúmenes;
- sistema de versiones;
- rutas;

debe comprobarse el impacto sobre:

- `config/`;
- `capitulos/`;
- `volumenes/`;
- `recursos/`;
- `formulario.tex`;
- `clase.tex`;
- rutas de imágenes;
- `\input`;
- `label`;
- referencias;
- versiones de ejercicios;
- material ya desarrollado.

Las decisiones estructurales deben realizarse deliberadamente.

No cambiar de convención entre temas sin una razón clara.

Si una mejora exige modificar una decisión consolidada, debe evaluarse primero
su impacto general.

---

# 60. Nuevas decisiones permanentes

Cuando se adopte una nueva decisión permanente relacionada con la arquitectura
o funcionamiento técnico del proyecto debe actualizarse:

```text
instrucciones/configuracion.md
```

Cuando la decisión afecte específicamente al desarrollo de teoría, formulario o
ejercicios debe actualizarse preferiblemente:

```text
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

según corresponda.

Cuando se trate de una regla general para agentes y herramientas de IA debe
evaluarse su incorporación a:

```text
AGENTS.md
```

Cuando la información corresponda únicamente al estado actual debe actualizarse:

```text
pendientes.md
```

No duplicar innecesariamente una misma decisión en varios documentos.

---

# 61. Prioridad documental

Para comprender el funcionamiento del proyecto deben interpretarse los archivos
según su función.

```text
AGENTS.md
→ reglas generales del proyecto para agentes

instrucciones/configuracion.md
→ arquitectura y decisiones técnicas permanentes

instrucciones/teoria.md
→ desarrollo de teoría

instrucciones/formulario.md
→ desarrollo de formularios

instrucciones/ejercicios.md
→ desarrollo de ejercicios

pendientes.md
→ estado actual y punto de continuación
```

No utilizar `pendientes.md` como sustituto de la documentación permanente.

No utilizar `configuracion.md` para registrar el avance cotidiano.

---

# 62. Consulta antes de modificar configuración

Antes de realizar cambios en:

```text
config/
volumenes/
clase.tex
formulario.tex
```

debe revisarse este documento.

Si el cambio afecta además contenido físico, deben consultarse las instrucciones
especializadas correspondientes.

Si el cambio puede afectar decisiones consolidadas, revisar también:

```text
AGENTS.md
pendientes.md
```

para comprobar el contexto actual.

---

# 63. Consistencia de nombres

Los nombres de carpetas y archivos deben mantenerse estables.

Utilizar nombres:

- descriptivos;
- consistentes;
- compatibles con rutas;
- coherentes con el índice maestro.

No renombrar carpetas únicamente por preferencia estilística.

Cuando un cambio de nombre sea necesario deben actualizarse todas las
referencias relacionadas:

- `\input`;
- imágenes;
- documentos maestros;
- agregadores;
- etiquetas cuando corresponda;
- documentación.

---

# 64. Consistencia entre sistemas operativos

La estructura debe evitar depender de características particulares de Windows,
Linux o macOS.

Preferir:

- rutas relativas;
- nombres de archivo estables;
- ausencia de rutas absolutas;
- estructura portable.

Evitar depender de la ubicación concreta del repositorio en un equipo.

---

# 65. Espacios y caracteres en nombres de archivos

Para archivos internos del proyecto se prefieren nombres compatibles con rutas
LaTeX y herramientas de desarrollo.

En carpetas y archivos de contenido se recomienda mantener la convención ya
utilizada:

```text
minusculas_con_guion_bajo
```

Ejemplo:

```text
10_caida_libre_y_movimiento_vertical
```

No renombrar material existente únicamente para aplicar esta convención si el
cambio puede romper rutas y no existe una necesidad real.

Los PDF bibliográficos pueden conservar sus nombres originales si esto facilita
su identificación.

---

# 66. Comentarios en código LaTeX

Los comentarios deben utilizarse para información técnica útil.

Son apropiados para:

- separar bloques estructurales;
- explicar una decisión técnica;
- documentar una ruta;
- aclarar un mecanismo de compilación;
- indicar una dependencia no evidente.

Evitar comentarios redundantes como:

```latex
% VELOCIDAD MEDIA
\subsection{Velocidad media}
```

cuando el comentario no añade información.

---

# 67. Expresiones compactas

Las expresiones matemáticas cortas deben mantenerse compactas cuando esto
mejore la legibilidad del código.

Por ejemplo:

```latex
\[ v=v_0+at. \]
```

es preferible a dividir artificialmente una ecuación breve en muchas líneas.

Las expresiones largas pueden dividirse cuando sea necesario.

La legibilidad del código tiene prioridad sobre reglas mecánicas de longitud de
línea.

---

# 68. No duplicar configuración

No redefinir localmente:

- colores;
- estilos;
- entornos;
- comandos;
- unidades;
- configuración de hipervínculos;
- mecanismos de versiones;

si ya existen globalmente.

Cuando una característica vaya a utilizarse en varios capítulos, debe
considerarse su incorporación a `config/`.

Cuando sea estrictamente local, puede permanecer en el archivo correspondiente
si no altera la identidad general.

---

# 69. Nuevos comandos

Antes de crear un comando nuevo:

1. comprobar si ya existe;
2. determinar si será global o local;
3. elegir un nombre descriptivo;
4. evitar conflictos con paquetes;
5. comprobar su uso en todas las versiones pertinentes.

Los comandos globales deben añadirse a:

```text
config/comandos.tex
```

No llenar `comandos.tex` con abreviaturas utilizadas una sola vez.

---

# 70. Nuevos entornos

Antes de crear un entorno nuevo:

1. comprobar si un entorno existente cumple la función;
2. determinar su función pedagógica;
3. asignarle una identidad visual coherente;
4. comprobar su comportamiento con saltos de página;
5. comprobar su comportamiento en las diferentes versiones cuando corresponda.

Los entornos globales deben definirse en:

```text
config/entornos.tex
```

No crear múltiples entornos visualmente distintos para funciones equivalentes.

---

# 71. Nuevos estilos

Los estilos reutilizables deben centralizarse en:

```text
config/estilos.tex
```

No repetir configuraciones extensas de:

```latex
tcolorbox
TikZ
PGFPlots
```

en múltiples capítulos cuando puedan abstraerse de forma limpia.

La abstracción debe mejorar el mantenimiento.

No crear una macro global únicamente para evitar unas pocas líneas que son
realmente específicas de un único tema.

---

# 72. Compatibilidad con las versiones

Cualquier cambio en:

```text
ejercicio
respuesta
explicacion
pistas
niveles
```

debe comprobarse en las tres salidas:

```text
estudiante
respuestas
docente
```

Una modificación que funcione en la versión docente pero revele soluciones en
la versión estudiante no es aceptable.

El comportamiento debe comprobarse desde los documentos maestros.

---

# 73. Numeración de ejercicios

La numeración de ejercicios debe permanecer coherente entre:

```text
estudiante
respuestas
docente
```

El mismo ejercicio debe conservar el mismo número en todas las versiones.

La ocultación de respuestas o explicaciones no debe alterar la numeración de
los ejercicios.

No duplicar enunciados para resolver problemas de numeración.

---

# 74. Imágenes en ejercicios

Las imágenes asociadas a ejercicios deben formar parte del contenido común.

La ocultación de respuestas y explicaciones no debe eliminar una figura
necesaria para comprender el enunciado.

Una figura que forme parte exclusivamente de una explicación docente debe
colocarse dentro del contenido condicionado correspondiente.

Debe comprobarse el resultado en las tres versiones.

---

# 75. Agregadores

Un archivo agregador tiene como única función reunir contenido de subtemas.

Por ejemplo:

```latex
\input{.../01_peso/teoria}
\input{.../02_fuerza_normal/teoria}
\input{.../03_tension/teoria}
\input{.../04_fuerza_elastica_y_ley_de_hooke/teoria}
```

No copiar el contenido de esos archivos dentro del agregador.

Los agregadores reducen la cantidad de rutas que deben conocer los documentos
maestros.

---

# 76. Granularidad

La estructura debe permitir capítulos suficientemente granulares sin crear una
fragmentación innecesaria.

Un tema puede convertirse en subcarpeta propia cuando:

- posee teoría sustancial;
- posee formulario propio;
- posee ejercicios propios;
- constituye una unidad pedagógica reconocible;
- su separación mejora el mantenimiento.

No crear subcarpetas para apartados mínimos que funcionan mejor como secciones
de un mismo archivo.

---

# 77. Relación entre índice y carpetas

La estructura de carpetas debe reflejar razonablemente el índice maestro.

Sin embargo, el índice editorial es la autoridad conceptual.

No modificar el índice maestro únicamente para acomodarlo a una estructura de
archivos accidental.

Si existe discrepancia entre la organización de carpetas y una decisión
editorial consolidada, debe corregirse deliberadamente la arquitectura y no
improvisarse una nueva numeración.

---

# 78. Migración y carpeta antigua `teoria/`

La carpeta antigua:

```text
teoria/
```

se conserva temporalmente mientras exista contenido pendiente de migración.

Durante este periodo:

- no crear contenido nuevo allí;
- no utilizarla como arquitectura de referencia;
- no eliminar contenido no migrado;
- no incluir simultáneamente versiones antigua y nueva del mismo tema;
- consultar `pendientes.md` antes de determinar qué versión está activa.

Cuando toda la información necesaria haya sido migrada y verificada, podrá
evaluarse la eliminación definitiva de la estructura antigua.

Esa eliminación debe realizarse únicamente después de comprobar que no queden:

- rutas activas;
- imágenes necesarias;
- archivos no migrados;
- referencias;
- contenido exclusivo.

---

# 79. Revisión antes de eliminar archivos

Antes de eliminar un archivo o carpeta durante una migración debe comprobarse:

1. que exista una versión nueva equivalente;
2. que el contenido haya sido revisado;
3. que las imágenes hayan sido trasladadas;
4. que las rutas hayan sido actualizadas;
5. que ningún documento maestro lo incluya;
6. que compile la nueva versión;
7. que no contenga material todavía no migrado.

No eliminar contenido únicamente porque parezca antiguo.

---

# 80. Revisión física y matemática

Aunque este documento se concentra en arquitectura y configuración, ninguna
modificación estructural debe provocar pérdida de contenido o alterar
inadvertidamente la Física.

Antes de considerar completa la migración de un tema debe comprobarse:

- exactitud física;
- exactitud matemática;
- coherencia dimensional;
- signos;
- unidades;
- conversiones;
- cifras significativas;
- resultados numéricos;
- dirección y sentido de vectores;
- gráficas;
- diagramas;
- condiciones de validez;
- aproximaciones;
- consistencia entre teoría, formulario y ejercicios.

Los criterios detallados pertenecen a las instrucciones especializadas.

---

# 81. Coherencia visual

La obra debe conservar una identidad visual común.

No debe parecer que cada capítulo fue diseñado como un documento independiente.

Deben mantenerse coherentes:

- colores;
- cajas;
- tipografía;
- títulos;
- listas;
- encabezados;
- pies de página;
- fórmulas;
- ejemplos;
- advertencias;
- ejercicios;
- explicaciones.

Los cambios visuales globales deben realizarse desde `config/`.

---

# 82. Principio de mantenibilidad

La arquitectura debe facilitar que un cambio global pueda realizarse en el menor
número razonable de lugares.

Por ejemplo:

```text
cambiar el color de las definiciones
→ modificar configuración global

cambiar el estilo de capítulos
→ modificar configuración global

cambiar la visibilidad de respuestas
→ modificar versiones

corregir un ejercicio
→ modificar un único ejercicios.tex
```

Evitar arquitecturas que obliguen a corregir el mismo contenido en múltiples
archivos.

---

# 83. Principio de separación de responsabilidades

Cada tipo de archivo debe cumplir principalmente una función.

```text
AGENTS.md
→ reglas generales

pendientes.md
→ estado

instrucciones/configuracion.md
→ arquitectura técnica

instrucciones/teoria.md
→ teoría

instrucciones/formulario.md
→ formularios

instrucciones/ejercicios.md
→ ejercicios

config/
→ implementación LaTeX compartida

capitulos/
→ contenido

volumenes/
→ ensamblaje editorial

libros/
→ fuentes

recursos/
→ recursos compartidos
```

Evitar mezclar estas responsabilidades.

---

# 84. Principio de continuidad

La arquitectura debe servir a una colección continua y no a documentos
aislados.

Todo nuevo contenido debe poder integrarse coherentemente con:

- capítulos anteriores;
- capítulos posteriores;
- documentos maestros;
- versiones;
- formularios;
- material de clase.

Los saltos temporales para preparar clases no alteran la estructura definitiva.

---

# 85. Regla final

Antes de realizar una modificación técnica importante, comprobar:

```text
¿ya existe una solución global?
¿el cambio afecta otros capítulos?
¿rompe alguna ruta?
¿afecta documentos maestros?
¿afecta las tres versiones?
¿afecta imágenes?
¿afecta numeración?
¿afecta comandos o entornos existentes?
¿introduce duplicación?
¿dificulta el mantenimiento?
¿es compatible con la arquitectura actual?
```

Si la modificación afecta una decisión consolidada de arquitectura, debe
evaluarse antes de aplicarla.

El objetivo técnico es mantener una estructura:

```text
modular
coherente
reutilizable
portable
escalable
compilable
mantenible
```

al servicio del contenido físico y pedagógico de la colección.