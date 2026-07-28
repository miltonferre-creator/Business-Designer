# 10 · Volume e cenários de receita

Horizonte de 3 anos em 12 trimestres, conforme pedido no Encontro 5. A memória de cálculo completa está na planilha [`entregaveis/Antevia_Modelo_Receitas.xlsx`](entregaveis/Antevia_Modelo_Receitas.xlsx), com as premissas isoladas em abas próprias para simulação.

## A unidade de negócio é a turma

Tudo no modelo deriva de uma turma padrão:

| Parâmetro | Valor |
|---|---|
| Alunos por turma | 100 |
| Módulos no programa | 12 |
| Duração do ciclo | 20 meses |
| Ritmo | 0,6 módulo por aluno por mês |
| Viagens por turma por trimestre (adesão 60%) | **108** |

### Correção de um número da Banca de Modelagem

O documento [atores-e-financeiro.md](../sprint-03/banca-de-modelagem/atores-e-financeiro.md) registra "720 viagens organizadas por ano" e "R$ 72 mil por turma/ano". Os dois valores estão certos em magnitude, mas o período está errado: **720 viagens e R$ 72 mil são o ciclo completo da turma, que dura 20 meses — não um ano.**

100 alunos × 60% × 12 módulos = 720 viagens ao longo de 20 meses. Anualizado, dá 432 viagens e R$ 43,2 mil por turma.

A projeção abaixo usa o ritmo correto. Vale corrigir o texto da banca antes da apresentação: um avaliador que dividir 12 módulos por 20 meses encontra a inconsistência em dez segundos.

## Receita por viagem, por cenário

| | Pessimista | Tendencial | Otimista |
|---|---|---|---|
| Adesão da turma | 50% | 60% | 70% |
| Taxa de serviço | R$ 50 | R$ 100 | R$ 150 |
| Comissão sobre bloqueio | 5% | 6,4% | 8% |
| Comissão em R$ (ticket R$ 1.700) | R$ 85,00 | R$ 108,80 | R$ 136,00 |
| **Receita por viagem** | **R$ 135,00** | **R$ 208,80** | **R$ 286,00** |
| Viagens por turma/trimestre | 90 | 108 | 126 |
| **Receita por turma/trimestre** | **R$ 12.150** | **R$ 22.550** | **R$ 36.036** |

Os três cenários movem quatro variáveis ao mesmo tempo, o que é realista: adesão baixa e poder de negociação baixo andam juntos. A análise de sensibilidade adiante isola cada uma.

## Turmas ativas por trimestre

| Trimestre | T1 | T2 | T3 | T4 | T5 | T6 | T7 | T8 | T9 | T10 | T11 | T12 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Pessimista | 0 | 1 | 2 | 3 | 5 | 7 | 9 | 12 | 15 | 18 | 21 | 24 |
| Tendencial | 1 | 2 | 4 | 6 | 9 | 12 | 16 | 20 | 25 | 30 | 36 | 42 |
| Otimista | 2 | 4 | 7 | 10 | 15 | 21 | 28 | 36 | 44 | 50 | 55 | 60 |

No cenário pessimista o T1 fecha sem turma: o primeiro trimestre é consumido pela negociação com a coordenação e pela montagem do bloqueio. É o comportamento esperado de uma venda B2B institucional.

## Receita por trimestre (R$)

| Trimestre | Pessimista | Tendencial | Otimista |
|---|---:|---:|---:|
| T1 | 0 | 22.550 | 72.072 |
| T2 | 12.150 | 45.101 | 144.144 |
| T3 | 24.300 | 90.202 | 252.252 |
| T4 | 36.450 | 135.302 | 360.360 |
| **Ano 1** | **72.900** | **293.155** | **828.828** |
| T5 | 60.750 | 202.954 | 540.540 |
| T6 | 85.050 | 270.605 | 756.756 |
| T7 | 109.350 | 360.806 | 1.009.008 |
| T8 | 145.800 | 451.008 | 1.297.296 |
| **Ano 2** | **400.950** | **1.285.373** | **3.603.600** |
| T9 | 182.250 | 563.760 | 1.585.584 |
| T10 | 218.700 | 676.512 | 1.801.800 |
| T11 | 255.150 | 811.814 | 1.981.980 |
| T12 | 291.600 | 947.117 | 2.162.160 |
| **Ano 3** | **947.700** | **2.999.203** | **7.531.524** |
| **Total 3 anos** | **1.421.550** | **4.577.731** | **11.963.952** |

## O que o cenário tendencial entrega em 3 anos

| Indicador | Valor |
|---|---|
| Viagens organizadas | 21.924 |
| Volume transacionado (GMV) | R$ 37,3 mi |
| Receita Antévia | R$ 4,58 mi |
| **Economia devolvida ao bolso dos alunos** | **R$ 8,77 mi** |
| Turmas ativas no T12 | 42 |
| Alunos atendidos no T12 | 2.520 |

A economia entregue aos alunos é quase o dobro da receita da empresa. Para a escola, é o número que justifica indicar o serviço: **R$ 8,8 milhões que deixam de sair do bolso dos alunos dela.**

## Análise de sensibilidade

Cada variável movida isoladamente, com as demais no cenário tendencial. Base: R$ 4,58 mi em 3 anos.

| Variável | Faixa testada | Receita 3 anos | Impacto |
|---|---|---:|---:|
| **Ritmo de contratação de turmas** | −30% | R$ 3,20 mi | **−30,0%** |
| | +30% | R$ 5,95 mi | **+30,0%** |
| Taxa de serviço | R$ 50 | R$ 3,48 mi | −23,9% |
| | R$ 150 | R$ 5,67 mi | +23,9% |
| Comissão sobre bloqueio | 4% | R$ 3,68 mi | −19,5% |
| | 9% | R$ 5,55 mi | +21,2% |
| Adesão da turma | 50% | R$ 3,81 mi | −16,7% |
| | 70% | R$ 5,34 mi | +16,7% |

### A variável crítica não é a que esperávamos

Desde a Sprint 1 o grupo tratou a **adesão** como o risco principal — foi a calibração mais dura que a entrevista com a Velt impôs (50–70%, não 100%). A sensibilidade mostra que ela é a **menos** determinante das quatro: mover a adesão de 50% para 70% mexe ±17% na receita.

O que decide o resultado é o **ritmo de contratação de turmas**, com ±30%. E isso reposiciona o esforço comercial: o gargalo está em assinar coordenações, não em convencer alunos. Uma turma a mais vale mais do que dez pontos de adesão.

Consequência prática para a Sprint 5: a estrutura de pessoal precisa privilegiar quem abre turma antes de quem opera a turma.

## Premissas críticas ainda não validadas

Três números sustentam a projeção e nenhum deles foi confirmado em campo:

| Premissa | Valor usado | Como validar |
|---|---|---|
| Disposição a pagar (H6) | R$ 100/módulo | Entrevista com aluno-executivo viajante |
| Desconto real do bloqueio | 20–30% | Cotação de bloqueio com consolidadora |
| Ritmo de contratação de turmas | 42 turmas no T12 | Conversa com coordenação de campus com fluxo de fora |

A terceira é a mais importante — é a variável de maior sensibilidade e a única sem nenhuma referência externa até agora. As outras duas têm ao menos a calibração da Velt por trás.
