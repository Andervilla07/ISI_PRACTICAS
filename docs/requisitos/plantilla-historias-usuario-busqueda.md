# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [29/10/2026] |
| Versión | [Versión de trabajo] |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como [rol], quiero [capacidad amplia], para [beneficio].

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

[Justificación de los resultados útiles que separa la división.]

## US-01

**Título:** Buscar mediante una palabra o frase.

Como usuario registrado, quiero buscar una receta mediante una palabra o frase, para poder descargarla y hacerla.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que existen recetas publicadas que estan validadas, cuando el usuario busca una receta por texto, entonces el sistema mostrará todas las recetas que contengan el texto propuesta.
- **CA-02.** Dado la frase propuesta, cuando se busca una receta y no exista ninguna receta, entonces el sistema mandará un mensaje diciendo que no hay resultados para la busqueda.
- **CA-03.** Dado que la palabra permita una corrección ortográfica, cuando se buscque una receta, entonces el sistema propondrá una corrección.

## US-02

**Título:** Buscar por ingredientes incluidos.

Como usuario registrado, quiero poder filtrar la búsqueda por ingredientes, para poder incluir determinados ingredientes en las recetas.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado los ingredientes filtrados, cuando se busquen recetas, entonces el sistema mostrará todas las recetas que contengan esos ingredientes.
- **CA-02.** Dado que filtrar unos ingredientes que no pertenezcan a ninguna receta, cuando se busque por filtración de ingredientes, entonces el sistema indicará que no hay resultados para esa búsqueda.
- **CA-03.** Dado la inclusión y exclusión del mismo ingrediente, cuando se realiza la búsqueda por filtrado, entonces el sistema señalará el conflicto y no ejecutará ninguna busqueda hasta que el usuario lo corrija.

## US-03

**Título:** Excluir ingredientes.

Como usuario registrado, quiero poder excluir ingredientes, para que las recetas que busque no tengan esos ingredientes.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que no se encuentre ninguna receta, cuando el usuario excluya varios elementos , entonces el sistema mostrará un mensaje pero mantendrá el criterio de exclusión.
- **CA-02.** Dado que el usuario rellena todos los criterios, cuando realiza la búsqueda, entonces el sistema mostrará las recetas válidas para todos sus criterios.
- **CA-03.** Dado la inclusión y exclusión del mismo ingrediente, cuando se realiza la búsqueda por filtrado, entonces el sistema señalará el conflicto y no ejecutará ninguna busqueda hasta que el usuario lo corrija.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | [Sí] | [Sí] | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | [Sí] | [Sí] | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | [Sí] | [Sí] | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | [Sí] | [Sí] | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | [Sí] | [Sí] | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | [Sí] | [Sí] | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
