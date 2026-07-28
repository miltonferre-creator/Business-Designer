# Sprint 4 — Viabilidade: Projeção de Receitas

**Objetivo da sprint (Squeeze 4):** traduzir o modelo de negócio em números — dimensionar o mercado, pesquisar e definir o preço, e projetar a receita em três cenários ao longo de 12 trimestres.

## Documentos desta pasta

- [`oferta-e-mercado.md`](oferta-e-mercado.md) — o que será vendido, para quem e como; TAM, SAM e SOM com memória de cálculo; ticket logístico por módulo
- [`precificacao.md`](precificacao.md) — pesquisa de preços dos concorrentes e substitutos, definição do preço e ancoragem no valor entregue
- [`cenarios-de-receita.md`](cenarios-de-receita.md) — volume por trimestre, três cenários e análise de sensibilidade
- [`premissas.md`](premissas.md) — todas as premissas com origem e status, fórmulas e o que ficou fora do modelo

## Números-síntese (cenário tendencial, 3 anos)

| Indicador | Valor |
|---|---|
| Receita acumulada | **R$ 4,58 mi** |
| Volume transacionado (GMV) | R$ 37,3 mi |
| Viagens organizadas | 21.924 |
| Economia devolvida aos alunos | **R$ 8,77 mi** |
| Turmas ativas no T12 | 42 |
| Receita por viagem | R$ 208,80 |

Faixa dos três cenários: **R$ 1,42 mi** (pessimista) · **R$ 4,58 mi** (tendencial) · **R$ 11,96 mi** (otimista).

## Principais resultados

- **O preço se ancora na economia, não na disposição a pagar.** O aluno paga R$ 100 por módulo e recebe R$ 400 líquidos de volta — retorno de 4× sobre a taxa. Isso tira a precificação da discussão subjetiva e a prende a um número verificável.
- **A variável crítica não é a adesão.** A sensibilidade aponta o ritmo de contratação de turmas (±30%) como o fator determinante, bem à frente da adesão (±17%) — que era o risco que o grupo vinha tratando como principal desde a Sprint 1. O gargalo é assinar coordenações, não convencer alunos.
- **A receita não depende só do aluno.** A comissão paga pelos fornecedores responde por 52% da receita por viagem. Se H6 se confirmar no piso da faixa (R$ 50), o modelo perde 24% da receita — não deixa de existir.
- **Correção de um número da Banca de Modelagem.** As "720 viagens e R$ 72 mil por turma/ano" são, na verdade, o ciclo completo de 20 meses. Anualizado, dá 432 viagens e R$ 43,2 mil. Detalhe em [`cenarios-de-receita.md`](cenarios-de-receita.md).

## Entregáveis

- ✅ [`entregaveis/Sprint_04_Kairos_Antevia.pptx`](entregaveis/Sprint_04_Kairos_Antevia.pptx) — 10 slides para o Squeeze 4
- ✅ [`entregaveis/Antevia_Modelo_Receitas.xlsx`](entregaveis/Antevia_Modelo_Receitas.xlsx) — modelo com premissas isoladas para simulação, 12 trimestres, 3 cenários e sensibilidade

Cobertura dos itens pedidos no Encontro 5:

| Item | Onde |
|---|---|
| a. O que será ofertado, para quem e como | [`oferta-e-mercado.md`](oferta-e-mercado.md) |
| b. Potencial do negócio + memória de cálculo | [`oferta-e-mercado.md`](oferta-e-mercado.md) · [`premissas.md`](premissas.md) |
| c. Volume de ganhos por período | [`cenarios-de-receita.md`](cenarios-de-receita.md) |
| d. Pesquisa de preços | [`precificacao.md`](precificacao.md) |
| e. Definição de preços | [`precificacao.md`](precificacao.md) |
| f. Cenários de receitas por período | [`cenarios-de-receita.md`](cenarios-de-receita.md) |

## Validações pendentes

Em ordem de impacto sobre a projeção:

1. **Ritmo de contratação de turmas** — variável de maior sensibilidade e sem nenhuma referência externa. Entrevistar coordenação de campus com fluxo de fora.
2. **H6 — disposição a pagar R$ 50–150** — entrevistar aluno-executivo viajante, o único stakeholder pagante ainda não ouvido.
3. **Desconto real do bloqueio (20–30%)** — cotar um bloqueio de turma com consolidadora.
4. **P2 e P3 (fatias de mercado)** — sustentam o denominador do market share, não o cenário de receita.

## Próxima etapa

Sprint 5 — projeção de custos, despesas e investimentos; macroprocesso do negócio; estrutura de pessoal; consolidação em DFC trimestral de 3 anos.
