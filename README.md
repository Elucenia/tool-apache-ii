# APACHE II

Identificador: `apache-ii`. Pacote independente da interface ELUCENIA, para navegador e Node.js.

## Situação

- Revisão: **needs-review**. Revisão documental e clínica independente pendente.
- Execução: **disponível para reprodução técnica da fórmula**.
- Validação clínica independente: **não realizada**. Os testes abaixo verificam aritmética e transporte dos campos.
- Fonte importada: Panorama Médico; arquivo `app/content/ferramentas/urgencia.php`.
- 4/4 casos de referência conferidos na importação. 0 casos independentes desta ferramenta.
- Dados: o exemplo funciona localmente, sem rede, armazenamento ou identificação de pacientes.

## Uso no Node.js

```js
const { calculate } = require('./calculator.js');
const example = require('./examples.json')[0];
console.log(calculate(example.input));
```

Execute `node test.cjs` (ou `npm test`) para conferir os exemplos. Abra `index.html` para usar a versão local do navegador. Não há dependências npm.

## Contrato

`calculate(input)` recebe um objeto, devolve `{id, main, label, raw, clinicalValidation}` ou `{error, code, field?}`. Consulte `tool.json` e `metadata.fields` para nomes, unidades, opções e intervalos. Números aceitam valores finitos ou strings numéricas; opções precisam corresponder às chaves documentadas. Campos obrigatórios vazios, booleanos inválidos, valores fora de intervalo e resultados não finitos são rejeitados. Somente checkbox omitido representa falso; um campo numérico ou uma opção obrigatória nunca é preenchido automaticamente.

Interpretações, ordens terapêuticas e tabelas herdadas não são retornadas pelo adaptador. Classificações e valores ainda dependem da população e das limitações da fonte.

## Fórmula / versão

APACHE II = escore fisiológico agudo (12 variáveis, 0 a 4 pontos cada; Glasgow entra como 15 − Glasgow) + pontos de idade (≤ 44 = 0; 45–54 = 2; 55–64 = 3; 65–74 = 5; ≥ 75 = 6) + doença crônica (5 pontos em admissão clínica ou pós-operatório de urgência; 2 pontos no pós-operatório eletivo).Oxigenação: com FiO₂ ≥ 50%, pontua o gradiente A-a [FiO₂ × 713 − PaCO₂/0,8 − PaO₂]: ≥ 500 = 4; 350–499 = 3; 200–349 = 2; < 200 = 0. Com FiO₂ < 50%, pontua a PaO₂: > 70 = 0; 61–70 = 1; 55–60 = 3; < 55 = 4. A creatinina tem pontos dobrados na insuficiência renal aguda.Mortalidade hospitalar prevista: ln[R/(1 − R)] = −3,517 + 0,146 × APACHE II + 0,603 (se cirurgia de urgência) + peso da categoria diagnóstica.

A transcrição acima documenta o acervo de origem e pode requerer atualização. 

## Condições e limites

Estima a gravidade da doença e a mortalidade hospitalar de pacientes adultos admitidos na UTI, a partir de 12 variáveis fisiológicas, idade, doença crônica e categoria diagnóstica.

Confirme população, exclusões, unidades, versão e diretriz aplicável ao país e serviço. O resultado não deve ser utilizado isoladamente para diagnóstico, alta ou prescrição. O pacote não representa certificação clínica, aprovação regulatória ou indicação para toda população. Veja a revisão completa em `tool.json`.

## Fontes originais

- [Knaus WA, Draper EA, Wagner DP, Zimmerman JE. APACHE II: a severity of disease classification system. Crit Care Med, 1985.](https://doi.org/10.1097/00003246-198510000-00009)

## Exemplos e rastreabilidade

`examples.json` preserva `originalInput`, expectativa e entrada explícita do exemplo. Não foi necessário expandir opções zero nos exemplos.

## Direitos e repositório

Este pacote integra o acervo privado de desenvolvimento da ELUCENIA. A publicação externa depende de liberação expressa. A licença MIT (arquivo LICENSE) cobre o código de integração, preservando o aviso de autoria e a licença; não transfere direitos sobre instrumentos, traduções, questionários, artigos, marcas ou outros materiais de terceiros. Consulte NOTICE.md e as condições de cada titular. O acesso a este adaptador não publica nem licencia automaticamente o restante da plataforma ELUCENIA.

## Acesso ao repositório

Repositório privado da organização ELUCENIA. A abertura pública depende de liberação expressa.
