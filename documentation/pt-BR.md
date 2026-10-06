<!-- ELUCENIA technical documentation · bisap · pt-BR · no clinical/professional/rights approval -->

# Escore BISAP

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/bisap)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Ureia \> 53 mg/dL (BUN \> 25 mg/dL)

`bun`

### Alteração do estado mental (Glasgow \< 15)

`mental`

### SIRS (2 ou mais critérios)

`sirs`

### Idade \> 60 anos

`idade`

### Derrame pleural na imagem

`derrame`

## Edição do método

BISAP/Wu 2008:5 fatores, primeiras 24 h; BUN\>25 mg/d L; idade\>60

## Fórmula documentada

Um ponto para cada item presente nas primeiras 24 horas: BUN \> 25 mg/dL (ureia \> 53 mg/dL), Impaired mental status, SIRS, Age \> 60 anos e Pleural effusion.

SIRS: 2 ou mais entre temperatura \< 36 ou \> 38 °C, FC \> 90 bpm, FR \> 20 irpm ou PaCO₂ \< 32 mmHg, leucócitos \< 4.000 ou \> 12.000/mm³ ou \> 10% de bastões.

## Limites e população

O BISAP de 2008 utiliza dados das primeiras 24 horas da pancreatite aguda para estratificar risco de morte hospitalar. BUN \>25 mg/dL e idade \>60 anos são itens do escore, não critérios mínimos de inclusão. Avaliação de necrose, falência orgânica e aplicabilidade a subgrupos dependem das respectivas fontes; taxas observadas não constituem certeza prognóstica individual.

## Referências

- [Wu BU et al. The early prediction of mortality in acute pancreatitis: a large population-based study. Gut, 2008.](https://doi.org/10.1136/gut.2008.152702)

- [Singh VK et al. A prospective evaluation of the bedside index for severity in acute pancreatitis score in assessing mortality and intermediate markers of severity in acute pancreatitis. Am J Gastroenterol, 2009.](https://doi.org/10.1038/ajg.2009.28)

- [Banks PA et al. Classification of acute pancreatitis—2012: revision of the Atlanta classification and definitions by international consensus. Gut, 2013.](https://doi.org/10.1136/gutjnl-2012-302779)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

BISAP 0 a 2: menor risco de mortalidade

Mortalidade abaixo de 1% no grupo de menor risco da derivação; manter reavaliação clínica nas primeiras 48 h.


### 2

BISAP ≥ 3: risco aumentado de mortalidade e complicações

Associado a falência orgânica (OR 7,4), falência persistente (OR 12,7) e necrose pancreática (OR 3,8); considerar UTI ou unidade intermediária.

