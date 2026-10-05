<!-- ELUCENIA technical documentation · bisap · de · no clinical/professional/rights approval -->

# BISAP-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/bisap)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Harnstoff \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### Veränderter Bewusstseinszustand (Glasgow \< 15)

`mental`

### SIRS (2 oder mehr Kriterien)

`sirs`

### Alter \> 60 Jahre

`idade`

### Pleuraerguss in der Bildgebung

`derrame`

## Fassung der Methode

BISAP/Wu 2008: 5 Faktoren, erste 24 h; BUN \>25 mg/dL; Alter \>60

## Dokumentierte Formel

1 Punkt je Merkmal in den ersten 24 Stunden: BUN \>25 mg/dL (Harnstoff \>53 mg/dL), I beeinträchtigtes Bewusstsein, SIRS, A Alter \>60 Jahre, P Pleuraerguss.

SIRS: ≥2 aus Temperatur \<36 oder \>38 °C, Herzfrequenz \>90 bpm, Atemfrequenz \>20 Atemzüge/min oder PaCO₂ \<32 mmHg, Leukozyten \<4.000 oder \>12.000/mm³ oder \>10% Stabkernige.

## Grenzen und Population

BISAP von 2008 verwendet Daten der ersten 24 Stunden einer akuten Pankreatitis zur Einteilung des Krankenhaussterberisikos. BUN \>25 mg/dL und Alter \>60 Jahre sind Scoreitems, keine Mindesteinschlusskriterien. Die Beurteilung von Nekrose, Organversagen und Anwendbarkeit in Untergruppen hängt von den jeweiligen Quellen ab; beobachtete Raten bieten keine individuelle prognostische Gewissheit.

## Referenzen

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
