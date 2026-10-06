<!-- ELUCENIA technical documentation · bisap · it · no clinical/professional/rights approval -->

# Punteggio BISAP

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/bisap)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Urea \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### Alterazione dello stato mentale (Glasgow \< 15)

`mental`

### SIRS (2 o più criteri)

`sirs`

### Età \> 60 anni

`idade`

### Versamento pleurico all’imaging

`derrame`

## Edizione del metodo

BISAP/Wu 2008: 5 fattori, prime 24 h; BUN \>25 mg/dL; età \>60

## Formula documentata

1 punto per item nelle prime 24 ore: BUN \>25 mg/dL (urea \>53 mg/dL), I alterazione mentale, SIRS, A età \>60 anni, P versamento pleurico.

SIRS: ≥2 tra temperatura \<36 o \>38 °C, FC \>90 bpm, FR \>20 atti/min o PaCO₂ \<32 mmHg, leucociti \<4.000 o \>12.000/mm³ o \>10% forme a banda.

## Limiti e popolazione

Il BISAP del 2008 utilizza i dati delle prime 24 ore della pancreatite acuta per stratificare il rischio di morte ospedaliera. BUN \>25 mg/dL ed età \>60 anni sono item del punteggio, non criteri minimi di inclusione. La valutazione di necrosi, insufficienza d’organo e applicabilità nei sottogruppi dipende dalle rispettive fonti; i tassi osservati non costituiscono una certezza prognostica individuale.

## Riferimenti

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

BISAP 0 a 2: minore rischio di mortalità

Mortalità inferiore a 1% nel gruppo a minor rischio della derivazione; mantenere la rivalutazione clinica nelle prime 48 h.


### 2

BISAP ≥ 3: aumento del rischio di mortalità e complicanze

Associato a insufficienza d'organo (OR 7,4), insufficienza persistente (OR 12,7) e necrosi pancreatica (OR 3,8); considerare terapia intensiva o unità di intensità intermedia.

