# 10 · Volume e cenários de receita

Horizonte de 3 anos em 12 trimestres, conforme pedido no Encontro 5. A memória de cálculo completa está na planilha [`entregaveis/Antevia_Modelo_Receitas.xlsx`](entregaveis/Antevia_Modelo_Receitas.xlsx), com as premissas isoladas para simulação.

> **Segunda versão.** A primeira projetava R$ 4,58 mi em 3 anos, assumindo turma de 100 alunos e poder de negociação desde o T1. As duas premissas caíram. O racional da revisão está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## A unidade de conta é o aluno aderente

O modelo anterior girava em torno da turma, o que escondia a premissa frágil do tamanho dela. Agora o motor é o número de **alunos aderentes ativos**; a turma é só a forma de chegar até eles.

| Parâmetro | Valor |
|---|---|
| Alunos por turma | 40 (**a validar**) |
| Módulos no programa | 12 |
| Duração do ciclo | 20 meses |
| Ritmo | 0,6 módulo por aluno por mês |
| Viagens por aderente por trimestre | **1,8** |

### Correção de um número da Banca de Modelagem

O documento [atores-e-financeiro.md](../sprint-03/banca-de-modelagem/atores-e-financeiro.md) registra "720 viagens organizadas por ano" e "R$ 72 mil por turma/ano". Os valores correspondem ao **ciclo completo de 20 meses**, não a um ano — e partem de uma turma de 100 alunos que nunca foi validada.

O deck da banca foi apresentado com esses números, então não há o que corrigir no material já exibido. O encaminhamento é usar os valores certos da Sprint 5 em diante. Conferência completa em [consistencia-com-a-banca.md](consistencia-com-a-banca.md).

## Receita por viagem, por fase

O poder de negociação evolui ao longo dos três anos. Cada fase tem o seu ticket e a sua comissão.

| | Fase 1 (ano 1) | Fase 2 (ano 2) | Fase 3 (ano 3) |
|---|---|---|---|
| Como compramos | Apoio da consolidadora | Bloqueios pontuais | Convênio próprio |
| Ticket logístico | R$ 1.920 | R$ 1.800 | R$ 1.700 |
| Taxa de serviço | R$ 100 | R$ 100 | R$ 100 |
| Comissão | 3% | 5% | 6,4% |
| **Receita por viagem** | **R$ 157,60** | **R$ 190,00** | **R$ 208,80** |
| Economia líquida do aluno | R$ 180 | R$ 300 | R$ 400 |
| Retorno do aluno sobre a taxa | 1,8× | 3,0× | 4,0× |

## Adesão por cenário e fase

| Cenário | Ano 1 | Ano 2 | Ano 3 |
|---|---|---|---|
| Pessimista | 20% | 30% | 40% |
| Tendencial | 30% | 45% | 60% |
| Otimista | 40% | 55% | 70% |

A faixa de 50–70% calibrada com a Velt descreve operação madura. Só o ano 3 do cenário tendencial chega lá.

## Turmas ativas por trimestre

| Trimestre | T1 | T2 | T3 | T4 | T5 | T6 | T7 | T8 | T9 | T10 | T11 | T12 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Pessimista | 0 | 1 | 1 | 2 | 3 | 4 | 5 | 6 | 8 | 10 | 12 | 14 |
| Tendencial | 1 | 2 | 3 | 4 | 6 | 8 | 10 | 12 | 15 | 18 | 21 | 24 |
| Otimista | 1 | 3 | 5 | 7 | 10 | 14 | 18 | 22 | 27 | 32 | 37 | 42 |

No ano 1 são 1 a 2 instituições. O primeiro trimestre do cenário pessimista fecha sem turma — é o comportamento esperado de uma venda B2B institucional.

## Receita por trimestre (R$)

| Trimestre | Pessimista | Tendencial | Otimista |
|---|---:|---:|---:|
| T1 | 0 | 3.404 | 4.539 |
| T2 | 2.269 | 6.808 | 13.617 |
| T3 | 2.269 | 10.212 | 22.694 |
| T4 | 4.539 | 13.617 | 31.772 |
| **Ano 1** | **9.078** | **34.042** | **72.622** |
| T5 | 12.312 | 36.936 | 75.240 |
| T6 | 16.416 | 49.248 | 105.336 |
| T7 | 20.520 | 61.560 | 135.432 |
| T8 | 24.624 | 73.872 | 165.528 |
| **Ano 2** | **73.872** | **221.616** | **481.536** |
| T9 | 48.108 | 135.302 | 284.135 |
| T10 | 60.134 | 162.363 | 336.753 |
| T11 | 72.161 | 189.423 | 389.370 |
| T12 | 84.188 | 216.484 | 441.988 |
| **Ano 3** | **264.591** | **703.572** | **1.452.246** |
| **Total 3 anos** | **347.541** | **959.230** | **2.006.404** |

## Síntese dos três cenários

| Indicador | Pessimista | Tendencial | Otimista |
|---|---:|---:|---:|
| Receita 3 anos | R$ 347.541 | **R$ 959.230** | R$ 2.006.404 |
| Receita do ano 1 | R$ 9.078 | **R$ 34.042** | R$ 72.622 |
| Viagens | 1.714 | 4.752 | 9.950 |
| GMV | R$ 2,96 mi | R$ 8,24 mi | R$ 17,27 mi |
| Economia dos alunos | R$ 634 mil | R$ 1,74 mi | R$ 3,63 mi |
| Aderentes no T12 | 224 | 576 | 1.176 |
| Fatia do SAM no T12 | 2,1% | 5,5% | 11,2% |

A economia devolvida aos alunos continua sendo quase o dobro da receita da empresa — é o argumento que sustenta a indicação pela escola.

## Análise de sensibilidade

Cada variável movida isoladamente, com as demais no cenário tendencial. Base: R$ 959.230 em 3 anos.

| Variável | Baixo | Alto | Impacto − | Impacto + |
|---|---:|---:|---:|---:|
| **Tamanho da turma** (30 / 60 alunos) | R$ 719.423 | R$ 1.438.845 | **−25,0%** | **+50,0%** |
| **Adesão** (20/30/40% vs 40/55/70%) | R$ 639.487 | R$ 1.137.087 | **−33,3%** | +18,5% |
| **Ritmo de contratação de turmas** (±30%) | R$ 671.461 | R$ 1.246.999 | −30,0% | +30,0% |
| Comissão (uma faixa abaixo / acima) | R$ 824.602 | R$ 1.236.730 | −14,0% | +28,9% |
| Taxa de serviço (R$ 50 / R$ 150) | R$ 721.630 | R$ 1.196.830 | −24,8% | +24,8% |

### Correção de uma conclusão da primeira versão

A primeira versão afirmava que **a adesão era a variável menos determinante** e que o gargalo estava em assinar turmas. Essa conclusão não se sustenta no modelo revisto.

Ela era um artefato de duas escolhas: manter a turma fixa em 100 e a adesão fixa em 60% nos três anos. Com o tamanho da turma tratado como variável e a adesão evoluindo por fase, o quadro muda:

- **O tamanho da turma tem o maior potencial de alta** (+50%) — e é a única premissa do topo da lista que ninguém verificou.
- **A adesão tem a maior queda** (−33,3%), porque o cenário ruim comprime os três anos, não só um.
- **O ritmo de contratação segue relevante** (±30%), mas dividindo espaço com as outras duas em vez de dominar.

As três estão na mesma faixa de importância. Tratar qualquer uma como resolvida é o que produziu o erro anterior.

## Premissas críticas ainda não validadas

| # | Premissa | Valor usado | Como validar |
|---|---|---|---|
| 1 | Tamanho da turma | 40 | Secretaria FDC — pergunta de dois minutos |
| 2 | Adesão no ano 1, sem prova social | 30% | Aluno-executivo viajante (H6) |
| 3 | Ritmo de contratação de turmas | 24 no T12 | Coordenação de campus com fluxo de fora |
| 4 | Desconto real da antecipação aos 90 dias | 13% no aéreo | Cotação com consolidadora |
| 5 | Repasse da consolidadora no ano 1 | 3% | Conversa com a Velt |

A primeira é a mais barata e a que mais move o resultado.
