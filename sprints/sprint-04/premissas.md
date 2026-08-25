# 11 · Premissas e memória de cálculo

Todas as premissas da projeção de receitas, com origem e status. O que não tem fonte externa está marcado como estimativa do grupo — e é isso que a validação de campo precisa atacar primeiro.

> **Revisão.** Esta é a segunda versão. A primeira assumia turma de 100 alunos como fato validado e aplicava poder de negociação desde o primeiro trimestre. As duas premissas caíram sob questionamento do grupo. O que mudou e por quê está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

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

P2 e P3 sustentam o denominador do market share, não o cenário de receita — que é construído de baixo para cima a partir de turmas contratadas.

## Turma

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P5 | **Alunos por turma** | **40** | **Estimativa do grupo** | **A validar** |
| P6 | Módulos por programa | 12 | Exemplo ilustrativo da banca; coerente com a persona | **A validar** |
| P7 | Duração do ciclo | 20 meses | Persona Ricardo Fontes (Sprint 3) | Validada |
| P8 | Origens principais por turma | 5–8 | Velt / Bruno Brant (5 condições) | Calibrada |

### Nota sobre P5

Na primeira versão desta sprint, P5 valia 100 e estava marcada como "Padrão FDC · Validada". **Estava errado.** O número tem uma única origem no repositório — o bloco "Exemplo ilustrativo" de [atores-e-financeiro.md](../sprint-03/banca-de-modelagem/atores-e-financeiro.md) — e nunca foi verificado com a escola.

O valor foi reduzido a 40 como estimativa conservadora e continua **a validar**. É a premissa mais barata de resolver e a que mais muda o modelo: em 40, uma turma isolada não forma tarifa de grupo; em 100 com 60% de adesão e 5 origens, forma. A tabela completa está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## Adesão, por fase

Adesão não é constante. No ano 1 não há prova social — ninguém viu o serviço funcionar.

| # | Premissa | Ano 1 | Ano 2 | Ano 3 | Origem | Status |
|---|---|---|---|---|---|---|
| P9 | Adesão da turma (tendencial) | 30% | 45% | 60% | Faixa 50–70% da Velt aplicada só na maturidade | **A validar** |
| | Cenário pessimista | 20% | 30% | 40% | | |
| | Cenário otimista | 40% | 55% | 70% | | |

A faixa de 50–70% calibrada com a Velt descreve uma operação madura. Aplicá-la ao primeiro ano era o erro da versão anterior.

## Ticket logístico, por fase

O poder de negociação evolui. Ver [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md) para o racional.

| # | Item | Hoje | Fase 1 (ano 1) | Fase 2 (ano 2) | Fase 3 (ano 3) | Status |
|---|---|---|---|---|---|---|
| P10 | Aéreo ida e volta | R$ 1.400 | R$ 1.150 | R$ 1.080 | R$ 1.020 | **A validar** |
| P11 | Hotel, 2 diárias | R$ 600 | R$ 570 | R$ 530 | R$ 500 | **A validar** |
| P12 | Traslado | R$ 200 | R$ 200 | R$ 190 | R$ 180 | **A validar** |
| P13 | **Ticket logístico** | **R$ 2.200** | **R$ 1.920** | **R$ 1.800** | **R$ 1.700** | Derivado |
| P14 | Economia bruta por módulo | — | R$ 280 | R$ 400 | R$ 500 | Derivado |

Na fase 1 a economia vem **apenas da antecipação** — comprar aos 90 dias em vez de menos de 30. Não depende de negociar com fornecedor.

## Receita

| # | Premissa | Fase 1 | Fase 2 | Fase 3 | Origem | Status |
|---|---|---|---|---|---|---|
| P15 | Taxa de serviço por módulo | R$ 100 | R$ 100 | R$ 100 | H6, Sprint 1 | **A validar** |
| P16 | Comissão média sobre o ticket | 3% | 5% | 6,4% | Faixas da Velt por volume | Calibrada |
| P17 | **Receita por viagem** | **R$ 157,60** | **R$ 190,00** | **R$ 208,80** | Derivado | — |
| P18 | Economia líquida do aluno | R$ 180 | R$ 300 | R$ 400 | Derivado | — |
| P19 | Retorno do aluno sobre a taxa | 1,8× | 3,0× | 4,0× | Derivado | — |
| P20 | Fee da escola por turma | R$ 0 | R$ 0 | R$ 0 | Decisão do grupo — não modelado | — |

As comissões de P16 foram testadas contra o volume aéreo que cada ano gera, usando as faixas de Bruno Brant (R$ 250–500 mil/ano → 3–5%; acima de R$ 1 mi/ano → 8–12%). O teste está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## Tarifa de grupo

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P21 | Passageiros mínimos na mesma rota para tarifa de grupo | 10 | Prática de mercado | **A validar** |
| P22 | Turmas simultâneas por campus e data necessárias | 3–5 | Derivado de P5, P9 e P21 | Derivado |

P21 é a premissa que redefine o desenho comercial. Se o mínimo real for menor — 7, por exemplo —, a alavanca de grupo liga mais cedo.

## Ritmo comercial

| # | Premissa | Valor | Origem | Status |
|---|---|---|---|---|
| P23 | Turmas ativas no T4 (fim do ano 1) | 4 | Estimativa do grupo | **A validar** |
| P24 | Turmas ativas no T12 (tendencial) | 24 | Estimativa do grupo | **A validar** |
| P25 | Instituições no ano 1 | 1–2 | Estimativa do grupo | **A validar** |

P24 permanece a premissa de maior impacto na projeção e a que tem menos lastro. Nenhuma das três entrevistas da Sprint 1 tratou de ciclo de venda institucional.

## Fórmulas

```
viagens_trimestre = turmas × alunos_turma × adesão_da_fase × (módulos ÷ meses_ciclo) × 3
                  = turmas × 40 × 0,30 × (12 ÷ 20) × 3     [ano 1]

receita_viagem = taxa_serviço + (ticket_da_fase × comissão_da_fase)
               = 100,00 + (1.920 × 3%) = R$ 157,60          [fase 1]
               = 100,00 + (1.700 × 6,4%) = R$ 208,80        [fase 3]

economia_líquida_aluno = ticket_hoje − ticket_da_fase − taxa_serviço
                       = 2.200 − 1.920 − 100 = R$ 180       [fase 1]

pax_por_rota = (turmas_simultâneas × alunos_turma × adesão) ÷ origens
             ≥ 10 para formar tarifa de grupo
```

## O que não está no modelo

- **Fee da escola** (P20) — receita potencial, deliberadamente zerada
- **Inadimplência e no-show** — entram como custo na Sprint 5, não como redutor de receita aqui
- **Sazonalidade** — módulos distribuídos uniformemente; julho e dezembro não modelados
- **Reajuste de preço** — a taxa de R$ 100 é nominal e constante nos 3 anos
- **Churn de turma** — nenhuma turma abandona o serviço no meio do ciclo

As duas últimas puxam em direções opostas: a ausência de reajuste subestima a receita, a ausência de churn superestima. Nenhuma foi quantificada.
