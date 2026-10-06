<!-- ELUCENIA technical documentation · bisap · fr · no clinical/professional/rights approval -->

# Score BISAP

[conditions, sources et autorisations](https://elucenia.org/fr/outils/bisap)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Urée \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### Altération de l’état mental (Glasgow \< 15)

`mental`

### SIRS (2 critères ou plus)

`sirs`

### Âge \> 60 ans

`idade`

### Épanchement pleural à l’imagerie

`derrame`

## Édition de la méthode

BISAP/Wu 2008 : 5 facteurs, premières 24 h ; BUN \>25 mg/dL ; âge \>60

## Formule documentée

1 point par item dans les premières 24 heures : BUN \>25 mg/dL (urée \>53 mg/dL), I altération mentale, SIRS, A âge \>60 ans, P épanchement pleural.

SIRS : ≥2 parmi température \<36 ou \>38 °C, FC \>90 bpm, FR \>20 respirations/min ou PaCO₂ \<32 mmHg, leucocytes \<4 000 ou \>12 000/mm³ ou \>10% formes en bande.

## Limites et population

Le BISAP de 2008 utilise les données des premières 24 heures de pancréatite aiguë pour stratifier le risque de décès hospitalier. BUN \>25 mg/dL et âge \>60 ans sont des items du score, pas des critères minimaux d’inclusion. L’évaluation de la nécrose, de la défaillance d’organe et de l’applicabilité aux sous-groupes dépend des sources respectives ; les taux observés ne constituent pas une certitude pronostique individuelle.

## Références

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

BISAP 0 à 2 : risque de mortalité plus faible

Mortalité inférieure à 1% dans le groupe de moindre risque de la dérivation ; maintenir une réévaluation clinique au cours des 48 premières h.


### 2

BISAP ≥ 3 : risque accru de mortalité et de complications

Associé à une défaillance d'organe (OR 7,4), à une défaillance persistante (OR 12,7) et à une nécrose pancréatique (OR 3,8) ; envisager une USI ou une unité intermédiaire.

