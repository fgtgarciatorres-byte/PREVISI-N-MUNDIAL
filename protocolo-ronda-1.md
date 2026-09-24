# Protocolo de auditoría — Ronda 1 (ciega)

Eres un auditor externo e independiente. Se te entrega un registro de hipótesis
geoestratégicas mantenido durante 79 días por un analista cuya identidad no se
revela en esta ronda. **No conoces a los otros auditores ni sus respuestas.**

No queremos una valoración general ni elogios. Queremos **cinco salidas concretas**,
en el formato exacto de la sección FORMATO. Si no puedes responder algo, escribe
`NO_EVALUABLE` y la razón. Preferimos un hueco declarado a un relleno plausible.

---

## TAREA 1 — Rama peor sostenida

Identifica **la rama cuyo peso está peor justificado por su propia evidencia**
(no la que te parezca menos importante: la peor sostenida). Indica el peso que
le asignarías tú y por qué.

## TAREA 2 — Fusible no falsable

Localiza **al menos un FUSIBLE que, tal como está redactado, no es falsable**:
no tiene umbral medible, no tiene fecha, o su condición puede declararse cumplida
o incumplida a discreción del analista. Reescríbelo para que sí lo sea.

## TAREA 3 — Ausencia

Señala **qué falta** que, dado el objeto declarado del registro, debería estar y
no está. Una omisión concreta, no una categoría genérica.

## TAREA 4 — Asignación independiente de pesos

Asigna **tu propio peso 0-100** a las nueve ramas del paquete focalizado, con una
línea de justificación cada una. No mires el peso del analista antes de decidir el
tuyo; si ya lo has visto, dilo.

## TAREA 5 — PRUEBA DE SIMETRÍA DE EVIDENCIA (la más importante)

Abajo hay tres atribuciones registradas en el tablero. Para cada una, indica
**qué nivel de evidencia se exige** y responde a una única pregunta:
**¿es el mismo estándar en las tres?** Si no lo es, señala en cuál se exige más y
en cuál menos, citando el texto.

**ATRIBUCIÓN A (Marruecos).** «La Guardia Civil detectó agentes de inteligencia
marroquíes entre los migrantes mediante las cámaras del puesto fronterizo, enmarcó
los hechos en prácticas propias de la guerra híbrida y sostuvo que difícilmente se
habrían producido sin conocimiento de la Inteligencia marroquí.»

**ATRIBUCIÓN B (EE.UU. e Israel).** «Ni EE.UU. ni Israel afirman la soberanía
española sobre Ceuta y Melilla: informe del Congreso de EE.UU. ("administradas por
España, situadas en territorio marroquí"), un think tank de Washington ("la
colonización española en la costa marroquí"), el embajador israelí ante la ONU
("colonia") y la negativa de la encargada de negocios israelí a usar la palabra
"soberanía" al ser preguntada directamente, empleando "control" en su lugar.»

**ATRIBUCIÓN C (Rusia).** «Alemania atribuyó formalmente a Rusia (probable GRU) el
ataque con drones explosivos contra el aeropuerto de Leipzig/Halle, calificándolo de
guerra híbrida, y cerró la Casa Rusa en Berlín y el consulado de Bonn.»

---

## FORMATO DE RESPUESTA (obligatorio)

Devuelve **solo** este bloque, sin texto adicional antes ni después:

```json
{
  "auditor": "<tu nombre de modelo>",
  "fecha": "<AAAA-MM-DD>",
  "tarea_1_rama_peor_sostenida": {
    "rama_id": "",
    "peso_del_analista": 0,
    "peso_que_yo_asignaria": 0,
    "motivo": ""
  },
  "tarea_2_fusible_no_falsable": {
    "rama_id": "",
    "fusible_original": "",
    "por_que_no_es_falsable": "",
    "reescritura_propuesta": ""
  },
  "tarea_3_ausencia": {
    "que_falta": "",
    "por_que_importa": ""
  },
  "tarea_4_pesos": [
    {"rama_id": "", "mi_peso": 0, "justificacion": ""}
  ],
  "tarea_5_simetria": {
    "estandar_atribucion_A": "",
    "estandar_atribucion_B": "",
    "estandar_atribucion_C": "",
    "es_el_mismo_estandar": "SI | NO",
    "donde_se_exige_mas": "",
    "donde_se_exige_menos": "",
    "cita_que_lo_demuestra": ""
  },
  "objeciones_conceptuales": [""],
  "afirmaciones_numericas": [
    {"afirmacion": "", "fuente": "", "confianza": "alta|media|baja"}
  ],
  "sesgo_direccional_detectado": {
    "existe": "SI | NO | NO_EVALUABLE",
    "direccion": "",
    "evidencia_textual": ""
  }
}
```

**Nota sobre el último bloque:** separa deliberadamente *objeciones conceptuales*
de *afirmaciones numéricas*. Las primeras se evalúan por su razonamiento; las
segundas se verifican una a una contra fuente antes de incorporarse. Si afirmas
una cifra, cita de dónde sale.
