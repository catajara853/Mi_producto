---
status: framed
segment: Familias de estrato 3–5 en Rionegro, Medellín y oriente antioqueño que pagan la obra (casa en lote propio u obra blanca) por etapas y no pueden supervisarla a diario porque trabajan tiempo completo o viven lejos o en el exterior
personas: luz-marina-y-hernan-ospina, camila-rojas-y-andres-pena, jhon-fredy-cardona, natalia-velez, ruben-dario-mesa
---

# Opportunity: Confianza con la plata durante la obra

Las familias que pagan su obra por etapas y no pueden supervisarla en persona no saben si lo que pagan corresponde con lo que avanza la obra. Compensan con visitas, fotos por WhatsApp y desconfianza. Es relevante ahora porque la constructora está empezando y necesita clientes satisfechos y obras sin roces de plata antes de crecer.

## Segment and personas
- Luz Marina y Hernán Ospina (primary): sufren el problema
- Camila Rojas y Andrés Peña (primary): lo sufren en parte (más por el atraso y la visibilidad que por el mal uso de la plata)
- Jhon Fredy Cardona (tertiary): lo sufre, es el caso más agudo; también responde la creencia de viabilidad
- Natalia Vélez (secondary): no lo sufre (su dolor son los cambios de especificación)
- Rubén Darío Mesa (negative): no lo sufre, porque supervisa en persona; marca el límite del alcance
- Missing: ninguna

## Signals
| Signal | Provenance | Source |
|---|---|---|
| Hay casos de remodelación con pagos no atados al avance, anticipos altos sin obra y retrasos de 7 a 13 meses | secondary | product/research/2026-11-09-2056-mercado-cotizador-obra.md (Séptimo Día, jul-2026) |
| La SIC registró 75 denuncias por incumplimiento en remodelación (ene-2022 a may-2026) | secondary | ídem |
| Las guías al consumidor recomiendan pólizas, contrato escrito y verificar al contratista: la desconfianza está normalizada | secondary | ídem (Metrocuadrado, Séptimo Día) |
| Las herramientas de EE. UU. y LatAm se venden por "transparencia con el propietario" y "salir de WhatsApp" | secondary | ídem (JobTread, Buildpeer) |
| Vivvidero y AcabadosVIS se venden en Colombia con seguimiento de obra en tiempo real | secondary | ídem |
| Los clientes temen el atraso, los imprevistos y los sobrecostos | unverified | Experiencia del constructor como cliente (product/overview.md) |
| Hay casos de pérdida de plata con un familiar y de obras abandonadas | synthetic | product/personas/jhon-fredy-cardona.md, luz-marina-y-hernan-ospina.md |
| No hay señales observadas en las obras propias del constructor (2 casas y varias obras blancas) | real (ausencia) | Declarado por el constructor en el framing, 2026-11-09 |

## Business outcome
Producto interno; el sponsor es el constructor.
1. **Primero:** costo evitado (menos pagos atrasados o frenados, menos discusiones por plata, menos tiempo respondiendo "¿cómo va la obra?") y satisfacción del cliente al terminar la obra.
2. **Después**, cuando la herramienta esté probada: clientes nuevos (creencia [product] #1).

El criterio del sponsor en `product/overview.md` se ajustó a este orden el 2026-11-09.

## Constraints
- Presupuesto sin definir; por ahora la inversión es el tiempo del constructor.
- Horizonte de 3–6 meses para ver resultados.
- Empresa que está empezando, con pocas obras simultáneas: cualquier prueba tiene muy pocos clientes (probablemente las próximas 1 o 2 obras).
- Zona: Rionegro, Medellín y oriente antioqueño; el financiador puede estar en el exterior (diferencia horaria, conectividad).
- Se manejan datos personales (fotos de viviendas, montos), sujetos a la Ley 1581 de 2012 de habeas data [conocimiento del modelo — verificar].

## Beliefs
Están en product/overview.md, el registro único de creencias.
- [product] [value] (#1) Las familias escogen constructor en buena parte por la transparencia… (relacionada: es la etapa posterior del resultado de negocio)
- [opportunity: confianza-plata-obra] [value] Las familias del segmento hoy gastan esfuerzo real en verificar que lo que pagaron corresponda con lo que avanzó la obra: en su última obra, al menos la mitad hizo visitas no planeadas para revisar, pidió fotos o reportes una y otra vez, o frenó un pago hasta ver el avance.
- [opportunity: confianza-plata-obra] [viability] Si la familia ve el avance ligado a cada pago, el constructor deja de recibir pagos atrasados y preguntas repetidas sobre el avance, y el cliente terminaría la obra dispuesto a recomendarlo.

## Research agenda
| Belief | Instrument | Decision it unlocks | By when |
|---|---|---|---|
| [opportunity] [value] | **1. Datos propios (gratis):** revisar los chats de WhatsApp y los registros de pago de las obras pasadas y contar cuántas preguntas de avance hubo, cuántos pagos se atrasaron y cuántas visitas de verificación hizo el cliente | Línea base: ¿el problema aparece en mis propias obras? | 2026-11-23 |
| [opportunity] [value] | **2. Entrevistas** (/design-interview): 5–8 familias del segmento que hayan construido o terminado obra blanca en los últimos 2 años, incluyendo al menos una que financie desde el exterior | Seguir con esta oportunidad o cambiar a "acabados que no caben en el presupuesto" | 2026-12-15 |
| [opportunity] [viability] | **3. Prueba de solución** (/explore-solutions y luego /design-solution-tests) en la próxima obra, comparada contra la línea base del paso 1 | Invertir plata en construir la herramienta o no | Al cumplir el primer tercio de la próxima obra |
| [product] [value] #1 | Encuesta (/design-survey) sobre cómo llegan las familias a su constructor, más preguntas en las mismas entrevistas | Usar la transparencia como argumento de venta | Después de la prueba (fase de clientes nuevos) |

No se propone investigación secundaria nueva: la del 2026-11-09 ya cubrió el mercado.

## Candidate ideas (not evaluated)
Salen de la descripción original del producto. Quedan aparcadas, no respaldadas; son el insumo de /explore-solutions.
- Envío de avances de obra con fotos fechadas al cliente
- Registro de cambios del proyecto con fechas límite para hacerlos
- Plan de pagos atado a hitos de obra visibles para el cliente
