# SAEB 2025 · URE Itapevi

Painel com os resultados do **SAEB 2025** na **Bonificação por Resultados (BR) 2025, 2ª etapa**, para as 57 escolas da **Unidade Regional de Ensino de Itapevi** (SEDUC-SP).

**Acesse o painel:** https://adsonlima98.github.io/saeb-itapevi/

## O que o painel mostra

- **Evolução por disciplina e quanto faltou para as metas:** NOTA FINAL 23/24 → NOTA FINAL 2025 em Língua Portuguesa e Matemática (9º ano EF e 3ª série EM), com a distância até a Meta Ouro e a Meta Diamante. Sem escola escolhida, mostra a média simples das escolas da URE.
- **Notas das escolas e metas atingidas por disciplina:** a nota de 2025 de cada disciplina-série, marcando o que chegou à Meta Ouro ou à Meta Diamante, e o SAEB da escola (nota, evolução, meta, piso, frequência, participação e ICM).
- **ICM SAEB por escola:** o índice do Anexo Escola (0 a 0,50), com destaque para escolas zeradas por gatilho.
- **Tabela por disciplina-série:** notas, evolução, metas, piso e situação, com ordenação.

Filtros por escola, resultado da escola, série, disciplina e situação. Os filtros escolhidos ficam no endereço da página, então dá para compartilhar um link já filtrado.

## Fonte dos dados

Resolução SEDUC nº 106, de 11 de novembro de 2026 (DOE de 12/11/2026), que apura o IACM da BR do exercício de 2025: Nota Técnica de Apuração (Indicador SAEB) e anexos **Disciplina-Série** e **Escola**.

Os dados extraídos estão na pasta [`dados/`](dados/):

| Arquivo | Conteúdo |
|---|---|
| `disciplinas.json` | Linhas SAEB do Anexo Disciplina-Série das escolas da URE Itapevi |
| `escolas.json` | Colunas SAEB do Anexo Escola (gatilhos, notas, meta, piso, IC e ICM) |
| `pisos.json` | Pisos do Índice de Qualidade do SAEB (Nota Técnica, item 3.1.3.b) |

**Cálculos feitos no painel** (não constam da resolução):
- **Evolução:** NOTA FINAL 2025 − NOTA FINAL de referência.
- **Faltou:** meta − NOTA FINAL 2025, ou "Atingida".
- **Médias da URE:** média simples entre as escolas com nota em 2025.

Todos os demais números (notas, metas, ICM, gatilhos, pisos) são os da resolução.

## Observações

- Painel informativo, **sem valor oficial**. Em caso de divergência, vale o texto publicado no Diário Oficial.
- A resolução apura os índices, mas não traz valores, datas nem a regra de pagamento da 2ª etapa.

## Tecnologia

Página estática em um único arquivo (`index.html`), com HTML, CSS e JavaScript ([D3.js](https://d3js.org/)) e os dados embutidos. Não precisa de servidor nem de internet depois de carregada.

---

Desenvolvido por [Adson Lima](https://www.linkedin.com/in/adson-lima-dev/).
