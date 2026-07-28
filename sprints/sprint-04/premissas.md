# 11 · Premissas e memória de cálculo

Todas as premissas da projeção de receitas, com origem e status. O que não tem fonte externa está marcado como estimativa do grupo — e é isso que a validação de campo precisa atacar primeiro.

## Legenda de status

- **Validada** — confirmada em entrevista ou fonte pública
- **Calibrada** — ajustada por especialista, faixa conhecida
- **A validar** — estimativa do grupo, sem confirmação externa

## Mercado

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P1 | Matriculados em pós-graduação no Brasil | 1.400.000 | IBGE (Sprint 1) | Validada |
| P2 | Fatia em programas executivos presenciais e periódicos | 12% | Estimativa do grupo | **A validar** |
| P3 | Fatia que viaja de outra cidade ("fluxo de fora") | 25% | Entrevistas Claudia e Ana Paula (direção), magnitude estimada | **A validar** |
| P4 | SAM como fatia do TAM (Nova Lima, SP, Rio) | 25% | Estimativa do grupo | **A validar** |

P2 e P3 são as premissas mais frágeis da projeção. Elas não alteram o cenário de receita — que é construído de baixo para cima, a partir de turmas contratadas — mas sustentam o denominador do market share. Se P2 e P3 estiverem superestimadas, a fatia de mercado que apresentamos fica maior do que a real; se subestimadas, menor.

## Turma

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P5 | Alunos por turma | 100 | Padrão FDC (Sprint 3) | Validada |
| P6 | Módulos por programa | 12 | Padrão FDC (Sprint 3) | Validada |
| P7 | Duração do ciclo | 20 meses | Persona Ricardo Fontes (Sprint 3) | Validada |
| P8 | Adesão da turma | 60% (faixa 50–70%) | Bruno Brant / Velt | Calibrada |

## Ticket logístico

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P9 | Aéreo ida e volta, compra <30 dias | R$ 1.400 | Estimativa, rota Norte/CO → Sudeste (ANAC/ABEAR) | **A validar** |
| P10 | Desconto do bloqueio aéreo | 27% (faixa 20–30%) | Bruno Brant / Velt | Calibrada |
| P11 | Hotel, 2 diárias próximo ao campus | R$ 600 | Estimativa do grupo | **A validar** |
| P12 | Desconto do bloqueio hoteleiro | 17% | Estimativa do grupo | **A validar** |
| P13 | Traslado (2 trajetos) | R$ 200 | Estimativa do grupo | **A validar** |
| P14 | **Ticket logístico com Antévia** | **R$ 1.700** | Derivado de P9–P13 | — |
| P15 | Economia por módulo | R$ 500 | Derivado | — |

## Receita

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P16 | Taxa de serviço por módulo | R$ 100 (faixa R$ 50–150) | H6, Sprint 1 | **A validar** |
| P17 | Comissão sobre aéreo | 4% | Prática de mercado (Velt) | Calibrada |
| P18 | Comissão sobre hotel | 10% | Prática de mercado (Velt) | Calibrada |
| P19 | Comissão sobre traslado | 10% | Prática de mercado (Velt) | Calibrada |
| P20 | **Receita por viagem** | **R$ 208,80** | Derivado de P16–P19 | — |
| P21 | Fee da escola por turma | R$ 0 | Decisão do grupo — não modelado | — |

## Ritmo comercial

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P22 | Turmas ativas no T12 (tendencial) | 42 | Estimativa do grupo | **A validar** |
| P23 | Primeira turma contratada | T1 | Estimativa do grupo | **A validar** |

P22 é a premissa de maior impacto na projeção (±30% de sensibilidade) e a que tem menos lastro. Nenhuma das três entrevistas da Sprint 1 tratou de ciclo de venda institucional. É a lacuna mais séria do modelo.

## Fórmulas

```
viagens_turma_trimestre = alunos × adesão × (módulos ÷ meses_ciclo) × 3
                        = 100 × 0,60 × (12 ÷ 20) × 3 = 108

receita_viagem = taxa_serviço + (ticket_logístico × comissão_média)
               = 100,00 + (1.700 × 6,4%) = R$ 208,80

receita_trimestre = turmas_ativas × viagens_turma_trimestre × receita_viagem

economia_aluno = ticket_hoje − ticket_antévia − taxa_serviço
               = 2.200 − 1.700 − 100 = R$ 400
```

## O que não está no modelo

Registrado para que a banca não precise perguntar:

- **Fee da escola** (P21) — receita potencial, deliberadamente zerada
- **Inadimplência e no-show** — entram como custo na Sprint 5, não como redutor de receita aqui
- **Sazonalidade** — os módulos são distribuídos uniformemente ao longo do ciclo; férias de julho e dezembro não foram modeladas
- **Reajuste de preço** — a taxa de R$ 100 é nominal e constante nos 3 anos, sem correção pela inflação
- **Churn de turma** — nenhuma turma abandona o serviço no meio do ciclo

As duas últimas puxam a projeção em direções opostas: a ausência de reajuste subestima a receita, a ausência de churn superestima. Nenhuma das duas foi quantificada.
