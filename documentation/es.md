<!-- ELUCENIA technical documentation · bisap · es · no clinical/professional/rights approval -->

# Puntuación BISAP

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/bisap)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Urea \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### Alteración del estado mental (Glasgow \< 15)

`mental`

### SRIS (2 o más criterios)

`sirs`

### Edad \> 60 años

`idade`

### Derrame pleural en la imagen

`derrame`

## Edición del método

BISAP/Wu 2008: 5 factores, primeras 24 h; BUN \>25 mg/dL; edad \>60

## Fórmula documentada

1 punto por ítem en primeras 24 horas: BUN \>25 mg/dL (urea \>53 mg/dL), I alteración mental, SIRS, A edad \>60 años, P derrame pleural.

SIRS: ≥2 entre temperatura \<36 o \>38 °C, FC \>90 bpm, FR \>20 respiraciones/min o PaCO₂ \<32 mmHg, leucocitos \<4.000 o \>12.000/mm³ o \>10% bandas.

## Límites y población

El BISAP de 2008 utiliza datos de las primeras 24 horas de pancreatitis aguda para estratificar el riesgo de muerte hospitalaria. BUN \>25 mg/dL y edad \>60 años son ítems de la puntuación, no criterios mínimos de inclusión. La evaluación de necrosis, insuficiencia orgánica y aplicabilidad a subgrupos depende de sus respectivas fuentes; las tasas observadas no constituyen certeza pronóstica individual.

## Referencias

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

BISAP 0 a 2: menor riesgo de mortalidad

Mortalidad por debajo de 1% en el grupo de menor riesgo de la derivación; mantener la reevaluación clínica en las primeras 48 h.


### 2

BISAP ≥ 3: riesgo aumentado de mortalidad y complicaciones

Asociado con falla orgánica (OR 7,4), falla persistente (OR 12,7) y necrosis pancreática (OR 3,8); considerar UCI o unidad intermedia.

