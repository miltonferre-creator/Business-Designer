# 11 · Premissas e memória de cálculo

Todas as premissas da projeção de receitas, com origem e status. O que não tem fonte externa está marcado como estimativa do grupo — e é isso que a validação de campo precisa atacar primeiro.

> **Revisão.** Terceira versão. A primeira assumia turma de 100 alunos como fato validado e poder de negociação desde o T1. A segunda reduziu a turma a 40. A terceira **elimina a turma do modelo**: a unidade passa a ser o aluno captado, como o próprio exemplo da banca já fazia. O que mudou está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## Legenda de status

- **Validada** — confirmada em entrevista ou fonte pública
- **Calibrada** — ajustada por especialista, faixa conhecida
- **A validar** — estimativa do grupo, sem confirmação externa

## Mercado

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P1 | Matriculados em pós-graduação no Brasil | 1.400.000 | IBGE (Sprint 1) | Validada |
| P2 | Fatia em programas executivos presenciais e periódicos | 12% | Estimativa do grupo | **A validar** |
| P3 | Fatia que viaja de outra cidade ("fluxo de fora") | 25% | Entrevistas Sprint 1 (direção), magnitude estimada | **A validar** |
| P4 | SAM como fatia do TAM (Nova Lima, SP, Rio) | 25% | Estimativa do grupo | **A validar** |

P2 e P3 sustentam o denominador do market share, não o cenário de receita — que é construído de baixo para cima a partir dos alunos captados.

## Captação

A unidade do modelo é o aluno captado, não a turma. Isso elimina duas premissas frágeis das versões anteriores — tamanho da turma e taxa de adesão dentro dela.

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P5 | **Alunos captados no ano 1** | **100** | Exemplo da banca, relido como meta anual | **A validar** |
| P6 | Alunos ativos no fim do ano 2 | 280 | Estimativa do grupo | **A validar** |
| P7 | Alunos ativos no fim do ano 3 | 650 | Estimativa do grupo | **A validar** |
| P8 | Módulos por programa | 12 | Exemplo da banca; coerente com a persona | **A validar** |
| P9 | Duração do ciclo | 20 meses | Persona Ricardo Fontes (Sprint 3) | Validada |
| P10 | Viagens por aluno por trimestre | 1,8 | Derivado de P8 e P9 | — |

### Nota de contexto sobre turmas

Turmas de pós-graduação da FDC têm por volta de **40 alunos** — informação do grupo, que corrige o "100 alunos por turma" usado como exemplo ilustrativo na Banca de Modelagem.

O número **não entra no cálculo de receita**, porque a captação é medida em alunos e não em turmas. Ele segue relevante para uma única coisa: estimar quanta concentração por campus e data a operação reúne, que é o que determina se a tarifa de grupo fica acessível. Ver [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## Ticket logístico, por fase

O poder de negociação evolui. Ver [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md) para o racional.

| # | Item | Hoje | Fase 1 (ano 1) | Fase 2 (ano 2) | Fase 3 (ano 3) | Status |
|---|---|---|---|---|---|---|
| P11 | Aéreo ida e volta | R$ 1.400 | R$ 1.150 | R$ 1.080 | R$ 1.020 | **A validar** |
| P12 | Hotel, 2 diárias | R$ 600 | R$ 570 | R$ 530 | R$ 500 | **A validar** |
| P13 | Traslado | R$ 200 | R$ 200 | R$ 190 | R$ 180 | **A validar** |
| P14 | **Ticket logístico** | **R$ 2.200** | **R$ 1.920** | **R$ 1.800** | **R$ 1.700** | Derivado |
| P15 | Economia bruta por módulo | — | R$ 280 | R$ 400 | R$ 500 | Derivado |

Na fase 1 a economia vem **apenas da antecipação** — comprar aos 90 dias em vez de menos de 30. Não depende de negociar com fornecedor.

## Receita

| # | Premissa | Fase 1 | Fase 2 | Fase 3 | Origem | Status |
|---|---|---|---|---|---|---|
| P16 | Taxa de serviço por módulo | R$ 100 | R$ 100 | R$ 100 | H6, Sprint 1 | **A validar** |
| P17 | Comissão média sobre o ticket | 3% | 5% | 6,4% | Faixas da Velt por volume | Calibrada |
| P18 | **Receita por viagem** | **R$ 157,60** | **R$ 190,00** | **R$ 208,80** | Derivado | — |
| P19 | Economia líquida do aluno | R$ 180 | R$ 300 | R$ 400 | Derivado | — |
| P20 | Retorno do aluno sobre a taxa | 1,8× | 3,0× | 4,0× | Derivado | — |
| P21 | Fee da escola por turma | R$ 0 | R$ 0 | R$ 0 | Decisão do grupo — não modelado | — |

As comissões de P17 foram testadas contra o volume aéreo que cada ano gera, usando as faixas de Bruno Brant (R$ 250–500 mil/ano → 3–5%; acima de R$ 1 mi/ano → 8–12%). O teste está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## Tarifa de grupo

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P22 | Passageiros mínimos na mesma rota | 10 | Prática de mercado | **A validar** |
| P23 | Origens principais por campus | 5–8 | Velt (5 condições) | Calibrada |
| P24 | Alunos no mesmo campus/data para formar grupo | 50–60 | Derivado de P22 e P23 | — |

A captação de 100 alunos concentrada num campus e numa data rende cerca de 17 passageiros por rota com 6 origens — acima do mínimo. É por isso que o volume do ano 1 já começa a destravar a fase 2.

## Fórmulas

```
viagens_trimestre = alunos_ativos × (módulos ÷ meses_ciclo) × 3
                  = alunos_ativos × 1,8

receita_viagem = taxa_serviço + (ticket_da_fase × comissão_da_fase)
               = 100,00 + (1.920 × 3%) = R$ 157,60          [fase 1]
               = 100,00 + (1.700 × 6,4%) = R$ 208,80        [fase 3]

economia_líquida_aluno = ticket_hoje − ticket_da_fase − taxa_serviço
                       = 2.200 − 1.920 − 100 = R$ 180       [fase 1]

pax_por_rota = alunos_no_mesmo_campus_e_data ÷ origens
             ≥ 10 para formar tarifa de grupo
```

## O que não está no modelo

- **Fee da escola** (P21) — receita potencial, deliberadamente zerada
- **Inadimplência e no-show** — entram como custo na Sprint 5, não como redutor de receita aqui
- **Sazonalidade** — módulos distribuídos uniformemente; julho e dezembro não modelados
- **Reajuste de preço** — a taxa de R$ 100 é nominal e constante nos 3 anos
- **Churn de aluno** — nenhum aluno abandona o serviço no meio do ciclo

As duas últimas puxam em direções opostas: a ausência de reajuste subestima a receita, a ausência de churn superestima. Nenhuma foi quantificada.
