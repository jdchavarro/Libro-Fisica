# Estado de avance del proyecto de Física

Este archivo registra exclusivamente el estado actual del proyecto.

Debe permitir determinar rápidamente:

- qué temas están desarrollados;
- qué componentes están terminados;
- qué componentes están pendientes;
- qué contenido ha sido migrado;
- qué contenido permanece en la estructura anterior;
- qué comprobaciones están pendientes;
- cuál es el punto exacto de continuación;
- qué saltos temporales existen.

Las instrucciones permanentes del proyecto se encuentran en:

```text
AGENTS.md
instrucciones/configuracion.md
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

No duplicar aquí esas instrucciones.

---

# 1. Estado general

El proyecto se encuentra en proceso de migración desde la estructura anterior
hacia la nueva arquitectura modular.

La estructura actual relevante es:

```text
Fisica/
├── capitulos/
├── config/
├── instrucciones/
├── libros/
├── recursos/
├── volumenes/
├── AGENTS.md
├── clase.tex
├── formulario.tex
└── pendientes.md
```

La carpeta:

```text
teoria/
```

corresponde a la estructura anterior.

No considerar migrado un contenido únicamente porque exista su carpeta o sus
archivos en la nueva estructura.

---

# 2. Configuración general

**Estado: CONFIGURADA Y FUNCIONAL**

La configuración global se encuentra en:

```text
config/
```

con los archivos correspondientes para:

- paquetes;
- colores;
- comandos;
- estilos;
- entornos;
- versiones;
- configuración general.

La configuración actual permite compilar contenido desde la nueva estructura.

Debe continuar verificándose durante la migración de nuevos temas.

---

# 3. Documentación del proyecto

**Estado: ACTUALIZADA CON REORGANIZACIÓN EN CURSO**

Las instrucciones permanentes se encuentran en:

```text
AGENTS.md
instrucciones/
```

La carpeta anteriormente denominada:

```text
notas/
```

ha sido sustituida por:

```text
instrucciones/
```

Los documentos especializados son:

```text
instrucciones/configuracion.md
instrucciones/teoria.md
instrucciones/formulario.md
instrucciones/ejercicios.md
```

Debe comprobarse que no permanezcan referencias activas a rutas antiguas
`notas/...` dentro de los documentos de instrucciones o configuración.

Este archivo:

```text
pendientes.md
```

permanece en la raíz y es el registro único del estado de avance.

---

# 4. Biblioteca de fuentes

La carpeta:

```text
libros/
```

contiene las fuentes bibliográficas utilizadas para desarrollar el proyecto.

Se ha decidido organizar las fuentes en dos niveles:

```text
libros/
├── principales/
└── complementarios/
```

## Fuentes principales previstas

```text
Sears–Zemansky / Young–Freedman, volumen 1
Sears–Zemansky / Young–Freedman, volumen 2

Serway–Jewett, volumen 1
Serway–Jewett, volumen 2

Schaum / Bueche–Hecht

Bauer–Westfall, volumen 1
Bauer–Westfall, volumen 2
```

## Fuentes complementarias previstas

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

## Estado de reorganización

**PENDIENTE DE COMPROBACIÓN EN EL REPOSITORIO LOCAL**

Comprobar que los PDF hayan sido distribuidos correctamente entre:

```text
libros/principales/
libros/complementarios/
```

No modificar los PDF originales.

---

# 5. Estado resumido de contenidos

## Cinemática

```text
Capítulo 7  — Descripción del movimiento
Capítulo 8  — Movimiento rectilíneo
Capítulo 9  — Aceleración y movimiento rectilíneo uniformemente acelerado
Capítulo 10 — Caída libre y movimiento vertical
```

## Electricidad

```text
Capítulo 78 — Carga eléctrica y electrización
Capítulo 79 — Ley de Coulomb
Capítulo 80 — Campo eléctrico
Capítulo 81 — Flujo eléctrico y ley de Gauss
Capítulo 82 — Energía potencial eléctrica
Capítulo 83 — Potencial eléctrico
```

## Temas desarrollados temporalmente fuera de secuencia

```text
Capítulo 19
└── Fuerza elástica y ley de Hooke

Capítulo 69
└── Dilatación térmica lineal
```

---

# 6. Parte II — Cinemática

Ruta:

```text
capitulos/02_cinematica/
```

---

# 7. Capítulo 7 — Descripción del movimiento

Ruta:

```text
capitulos/02_cinematica/07_descripcion_del_movimiento/
```

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

Archivo:

```text
teoria.tex
```

La teoría se encuentra en la nueva estructura.

## Formulario

**Estado: PENDIENTE DE REVISIÓN O DESARROLLO**

Archivo:

```text
formulario.tex
```

## Ejercicios

**Estado: DESARROLLADOS; PENDIENTES DE VERIFICACIÓN FINAL DEL ESTADO LOCAL**

Archivo:

```text
ejercicios.tex
```

El contenido fue desarrollado durante el trabajo de Cinemática.

Antes de modificarlo nuevamente, comprobar el archivo existente y verificar:

- niveles de dificultad;
- respuestas;
- explicaciones;
- notación;
- unidades;
- compilación de las tres versiones.

## Estado del capítulo

**NO COMPLETO**

Falta completar o verificar todos los componentes y realizar la revisión
conjunta.

---

# 8. Capítulo 8 — Movimiento rectilíneo

Ruta:

```text
capitulos/02_cinematica/08_movimiento_rectilineo/
```

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

Archivo:

```text
teoria.tex
```

## Formulario

**Estado: PENDIENTE DE REVISIÓN O DESARROLLO**

Archivo:

```text
formulario.tex
```

## Ejercicios

**Estado: DESARROLLADOS; PENDIENTES DE VERIFICACIÓN FINAL DEL ESTADO LOCAL**

Archivo:

```text
ejercicios.tex
```

El contenido fue desarrollado durante el trabajo de Cinemática.

Antes de modificarlo nuevamente, comprobar el archivo existente y verificar:

- niveles;
- respuestas;
- explicaciones;
- cálculos;
- unidades;
- notación;
- compilación de las tres versiones.

## Estado del capítulo

**NO COMPLETO**

---

# 9. Capítulo 9 — Aceleración y movimiento rectilíneo uniformemente acelerado

Ruta:

```text
capitulos/02_cinematica/09_aceleracion_y_movimiento_rectilineo_uniformemente_acelerado/
```

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

Archivo:

```text
teoria.tex
```

## Formulario

**Estado: PENDIENTE DE REVISIÓN O DESARROLLO**

Archivo:

```text
formulario.tex
```

## Ejercicios

**Estado: DESARROLLADOS; PENDIENTES DE VERIFICACIÓN FINAL DEL ESTADO LOCAL**

Archivo:

```text
ejercicios.tex
```

El contenido fue desarrollado durante el trabajo de Cinemática.

Debe comprobarse el archivo existente antes de realizar cambios adicionales.

## Estado del capítulo

**NO COMPLETO**

---

# 10. Capítulo 10 — Caída libre y movimiento vertical

Ruta:

```text
capitulos/02_cinematica/10_caida_libre_y_movimiento_vertical/
```

## Teoría

**Estado: DESARROLLADA**

Archivo:

```text
teoria.tex
```

La teoría contiene el desarrollo del tema y fue utilizada para mantener
coherencia de cobertura, notación y convenciones durante la elaboración de los
ejercicios.

**Pendiente:**

realizar una revisión integral de la teoría antes de declarar definitivamente
revisado este componente.

## Formulario

**Estado: PENDIENTE**

Archivo:

```text
formulario.tex
```

Actualmente conserva únicamente la estructura inicial de plantilla.

Este es el componente inmediato que debe desarrollarse.

## Ejercicios

**Estado: DESARROLLADOS, REVISADOS Y COMPROBADOS**

Archivo:

```text
ejercicios.tex
```

Contiene:

```text
24 ejercicios originales
├── 8 básicos
├── 8 intermedios
└── 8 avanzados
```

Cada ejercicio contiene:

```text
ejercicio
respuesta
explicacion
```

Se incluyen, cuando corresponde:

- esquemas;
- gráficas;
- interpretación conceptual;
- problemas inversos;
- encuentros;
- análisis experimental.

Los cálculos fueron contrastados.

Se comprobó el funcionamiento con la configuración actual en las versiones:

```text
estudiante
respuestas
docente
```

La visibilidad de ejercicios, respuestas y explicaciones funciona de acuerdo
con cada versión.

No se detectaron errores de compilación ni desbordamientos horizontales durante
la comprobación realizada.

La revisión visual de una salida PDF definitiva permanece pendiente hasta que
se genere expresamente dicho formato.

## Integración en volumen

```text
volumenes/volumen_1/estudiante.tex
```

ya incluye el componente correspondiente.

La integración completa en:

```text
volumenes/volumen_1/respuestas.tex
volumenes/volumen_1/docente.tex
```

permanece pendiente de comprobación o incorporación definitiva.

## Estado del capítulo

**NO COMPLETO**

Falta:

1. desarrollar `formulario.tex`;
2. revisar integralmente `teoria.tex`;
3. revisar coherencia entre teoría, formulario y ejercicios;
4. completar la integración en los documentos maestros;
5. realizar la comprobación final del capítulo.

---

# 11. Electricidad

Los capítulos trabajados son:

```text
78_carga_electrica_y_electrizacion
79_ley_de_coulomb
80_campo_electrico
81_flujo_electrico_y_ley_de_gauss
82_energia_potencial_electrica
83_potencial_electrico
```

Las teorías correspondientes fueron migradas a la nueva estructura.

---

# 12. Capítulo 78 — Carga eléctrica y electrización

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

## Formulario

**Estado: EXISTE MATERIAL DESARROLLADO; PENDIENTE DE REVISIÓN/MIGRACIÓN**

## Ejercicios

**Estado: EXISTE MATERIAL DESARROLLADO; PENDIENTE DE REVISIÓN/MIGRACIÓN**

## Estado del capítulo

**NO COMPLETO**

---

# 13. Capítulo 79 — Ley de Coulomb

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

## Formulario

**Estado: DESARROLLADO; PENDIENTE DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

## Ejercicios

**Estado: DESARROLLADOS Y REVISADOS DURANTE EL TRABAJO DE ELECTRICIDAD; PENDIENTES DE COMPROBACIÓN FINAL EN LA NUEVA ESTRUCTURA**

Durante su revisión debe mantenerse la directriz de resolver prioritariamente
los problemas vectoriales mediante componentes rectangulares.

## Estado del capítulo

**NO COMPLETO**

---

# 14. Capítulo 80 — Campo eléctrico

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

La teoría fue modificada para utilizar componentes rectangulares como método
principal en problemas vectoriales.

## Formulario

**Estado: DESARROLLADO; PENDIENTE DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

## Ejercicios

**Estado: DESARROLLADOS; PENDIENTES DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

Debe comprobarse especialmente:

- componentes rectangulares;
- signos de las cargas;
- dirección y sentido del campo;
- sistemas de referencia;
- unidades;
- resultados numéricos.

## Estado del capítulo

**NO COMPLETO**

---

# 15. Capítulo 81 — Flujo eléctrico y ley de Gauss

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

## Formulario

**Estado: DESARROLLADO; PENDIENTE DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

## Ejercicios

**Estado: DESARROLLADOS; PENDIENTES DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

Los ejercicios pueden incluir diagramas cuando sean necesarios para comprender:

- superficies gaussianas;
- orientación;
- vectores normales;
- campos;
- simetrías.

## Estado del capítulo

**NO COMPLETO**

---

# 16. Capítulo 82 — Energía potencial eléctrica

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

## Formulario

**Estado: DESARROLLADO; PENDIENTE DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

## Ejercicios

**Estado: DESARROLLADOS; PENDIENTES DE COMPROBACIÓN FINAL DEL ESTADO LOCAL**

## Estado del capítulo

**NO COMPLETO**

---

# 17. Capítulo 83 — Potencial eléctrico

## Teoría

**Estado: DESARROLLADA Y MIGRADA**

## Formulario

**Estado: PENDIENTE**

## Ejercicios

**Estado: PENDIENTE**

## Estado del capítulo

**NO COMPLETO**

---

# 18. Fuerza elástica y ley de Hooke

Ruta prevista:

```text
capitulos/
└── 03_dinamica_y_estatica/
    └── 19_fuerzas_mecanicas_comunes/
        └── 04_fuerza_elastica_y_ley_de_hooke/
```

## Teoría

**Estado: DESARROLLADA EN LA ESTRUCTURA ANTERIOR**

## Formulario

**Estado: PENDIENTE DE REVISIÓN O DESARROLLO**

## Ejercicios

**Estado: PENDIENTE DE REVISIÓN O DESARROLLO**

## Migración

**Estado: PENDIENTE**

No eliminar el material de la estructura anterior hasta comprobar la nueva
versión.

## Estado del tema

**NO COMPLETO**

---

# 19. Dilatación térmica lineal

Ruta prevista:

```text
capitulos/
└── 11_fisica_termica_y_termodinamica/
    └── 69_dilatacion_termica/
        └── 01_dilatacion_termica_lineal/
```

## Teoría

**Estado: DESARROLLADA EN LA ESTRUCTURA ANTERIOR**

## Formulario

**Estado: PENDIENTE**

## Ejercicios

**Estado: PENDIENTE**

## Migración

**Estado: PENDIENTE**

No eliminar el material de la estructura anterior hasta comprobar la nueva
versión.

## Estado del tema

**NO COMPLETO**

---

# 20. Subtemas pendientes del capítulo 69

Todavía no se consideran desarrollados:

```text
02_dilatacion_termica_superficial
03_dilatacion_termica_volumetrica
04_dilatacion_de_liquidos
05_dilatacion_anomala_del_agua
```

Su desarrollo se realizará posteriormente manteniendo la progresión del
capítulo.

---

# 21. Estado de migración resumido

## Teoría migrada

### Cinemática

```text
07_descripcion_del_movimiento/teoria.tex
08_movimiento_rectilineo/teoria.tex
09_aceleracion_y_movimiento_rectilineo_uniformemente_acelerado/teoria.tex
10_caida_libre_y_movimiento_vertical/teoria.tex
```

### Electricidad

```text
78_carga_electrica_y_electrizacion/teoria.tex
79_ley_de_coulomb/teoria.tex
80_campo_electrico/teoria.tex
81_flujo_electrico_y_ley_de_gauss/teoria.tex
82_energia_potencial_electrica/teoria.tex
83_potencial_electrico/teoria.tex
```

## Desarrollado pero todavía no migrado

```text
19_fuerzas_mecanicas_comunes/
└── 04_fuerza_elastica_y_ley_de_hooke/
    └── teoria
```

```text
69_dilatacion_termica/
└── 01_dilatacion_termica_lineal/
    └── teoria
```

---

# 22. Temas que actualmente no se consideran completos

```text
07_descripcion_del_movimiento
08_movimiento_rectilineo
09_aceleracion_y_movimiento_rectilineo_uniformemente_acelerado
10_caida_libre_y_movimiento_vertical

19_fuerzas_mecanicas_comunes/
└── 04_fuerza_elastica_y_ley_de_hooke

69_dilatacion_termica/
└── 01_dilatacion_termica_lineal

78_carga_electrica_y_electrizacion
79_ley_de_coulomb
80_campo_electrico
81_flujo_electrico_y_ley_de_gauss
82_energia_potencial_electrica
83_potencial_electrico
```

Un tema solo debe pasar a:

```text
COMPLETO
```

cuando los componentes previstos estén terminados y revisados y se hayan
realizado las comprobaciones necesarias.

---

# 23. Saltos temporales registrados

Durante el desarrollo se realizaron saltos temporales para preparar clases.

Se ha trabajado temporalmente en:

```text
fuerza elástica y ley de Hooke
dilatación térmica lineal
electricidad
cinemática
```

Estos saltos no modifican:

- el índice maestro;
- la numeración;
- el orden conceptual general;
- la distribución definitiva de capítulos.

---

# 24. Punto exacto de continuación

El trabajo activo se encuentra actualmente en:

```text
Parte II — Cinemática
Capítulo 10 — Caída libre y movimiento vertical
```

Estado:

```text
teoria.tex
→ desarrollada
→ pendiente de revisión integral final

formulario.tex
→ pendiente
→ siguiente componente a desarrollar

ejercicios.tex
→ desarrollado
→ revisado
→ cálculos comprobados
→ funcionamiento estudiante/respuestas/docente comprobado
```

## Siguiente tarea inmediata

Desarrollar:

```text
capitulos/
└── 02_cinematica/
    └── 10_caida_libre_y_movimiento_vertical/
        └── formulario.tex
```

utilizando:

```text
AGENTS.md
instrucciones/formulario.md
```

y consultando la teoría existente y las fuentes bibliográficas pertinentes.

Después:

```text
1. revisar conjuntamente teoria.tex + formulario.tex + ejercicios.tex;
2. comprobar notación, unidades y sistemas de referencia;
3. comprobar compilación;
4. completar integración del capítulo 10 en los documentos maestros;
5. determinar si el capítulo 10 puede marcarse como COMPLETO.
```

---

# 25. Pendientes anteriores de Cinemática

Aunque el punto activo sea el capítulo 10, permanecen pendientes comprobaciones
y componentes de:

```text
Capítulo 7
Capítulo 8
Capítulo 9
```

Antes de declarar completa la Parte II deberán revisarse.

No interpretar el avance al capítulo 10 como cierre automático de los capítulos
anteriores.

---

# 26. Pendientes de Electricidad

Debe realizarse posteriormente una revisión sistemática de los capítulos:

```text
78
79
80
81
82
83
```

Comprobar para cada uno:

```text
teoria.tex
formulario.tex
ejercicios.tex
```

y determinar el estado real de los archivos existentes.

Debe prestarse especial atención a:

- adaptación de ejercicios antiguos al entorno `explicacion`;
- componentes rectangulares;
- signos de cargas;
- dirección y sentido de fuerzas y campos;
- unidades;
- cálculos;
- diagramas;
- compilación;
- integración en documentos maestros.

---

# 27. Pendientes estructurales

Actualmente permanecen las siguientes tareas:

1. comprobar que `notas/` haya sido sustituida completamente por
   `instrucciones/`;
2. corregir referencias internas que todavía apunten a `notas/...`;
3. comprobar la organización de `libros/principales/` y
   `libros/complementarios/`;
4. completar el formulario del capítulo 10;
5. revisar conjuntamente el capítulo 10;
6. revisar el estado real de formularios y ejercicios de los capítulos 7--9;
7. comprobar la compilación conjunta de Cinemática desde los documentos
   maestros correspondientes;
8. revisar sistemáticamente los capítulos 78--83 de Electricidad;
9. migrar fuerza elástica y ley de Hooke;
10. migrar dilatación térmica lineal;
11. actualizar los documentos maestros a medida que los temas queden
    comprobados;
12. mantener actualizado este archivo después de cada avance importante.

---

# 28. Próxima continuación

Si no existe una nueva petición temporal, continuar en:

```text
Parte II — Cinemática
Capítulo 10 — Caída libre y movimiento vertical
Componente: formulario.tex
```

Después de completar y revisar el capítulo 10, volver a comprobar los pendientes
de los capítulos 7, 8 y 9 antes de considerar cerrada la sección correspondiente
de Cinemática.