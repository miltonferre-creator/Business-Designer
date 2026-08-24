# 12 · Consistência com a Banca de Modelagem

A Banca de Modelagem foi apresentada com o deck registrado em [`../sprint-03/banca-de-modelagem/entregaveis/`](../sprint-03/banca-de-modelagem/entregaveis/). Este documento confronta cada número afirmado ali com o modelo construído na Sprint 4.

O objetivo é prático: garantir que a Sprint 4 não contradiga o que o grupo já defendeu em público e, onde contradiz, deixar claro qual das duas versões vale.

## Quadro de conferência

| Afirmação na banca | Sprint 4 | Situação |
|---|---|---|
| Turma de 100 alunos · 12 encontros | Igual | Confere |
| Adesão de 60% (faixa 50–70%) | Igual, e a faixa vira os cenários | Confere |
| Taxa de R$ 50–150, média R$ 100 | R$ 100 no tendencial; R$ 50 e R$ 150 nos extremos | Confere |
| Bloqueio de grupo com 20–30% de desconto | 22,7% de desconto médio | Confere |
| Três fontes de receita | Duas modeladas; fee da escola zerado | Confere, com ressalva |
| Programa de 18–24 meses, módulos a cada 4–6 semanas | Ciclo de 20 meses, 0,6 módulo/mês | Confere |
| "Compra a menos de 7 dias custa 2–3× mais" | Modelo usa 1,37× no aéreo | **Escalas diferentes** |
| "Aluno economiza 20–30%" | 22,7% na logística, 18,2% no bolso | **Reconciliar** |
| "720 viagens organizadas por ano" | 720 no ciclo de 20 meses | **Erro apresentado** |
| "R$ 72 mil por turma/ano" | R$ 72 mil por ciclo; R$ 43,2 mil/ano | **Erro apresentado** |

## 1. O "2–3× mais caro" e o 1,37× do modelo

A banca afirma que comprar com menos de 7 dias custa 2 a 3 vezes mais do que com 21 dias ou mais. O modelo da Sprint 4 usa aéreo de R$ 1.400 na compra tardia contra R$ 1.020 no bloqueio — uma razão de 1,37×.

As duas coisas não se contradizem, porque medem comparações diferentes:

- A banca compara o **extremo**: véspera contra três semanas.
- O modelo compara o **caso típico**: o aluno que compra com menos de 30 dias, que é o comportamento descrito na H1, contra o bloqueio disparado aos 90 dias.

O 2–3× é real, mas descreve a cauda. Se o modelo o adotasse como base, a economia por módulo saltaria e a receita de comissão junto. A projeção ficaria maior e mais frágil.

**Encaminhamento:** manter o 2–3× para descrever o problema e usar o 22,7% para descrever a entrega. Não usar o 2–3× como base de cálculo.

## 2. "Economiza 20–30%" contra os 18,2% do modelo

Os dois números estão certos e medem coisas distintas:

| O que se mede | Valor |
|---|---|
| Desconto obtido na logística (aéreo, hotel, traslado) | **22,7%** |
| Redução no desembolso total do aluno, já pagando a taxa de R$ 100 | **18,2%** |

A banca disse "economiza 20–30%" sem qualificar se era antes ou depois da taxa de serviço. O modelo separa as duas medidas.

**Encaminhamento:** passar a dizer "20–30% na logística; 18,2% no bolso, já descontada a nossa taxa". A versão qualificada é mais forte, não mais fraca — mostra que a taxa já está dentro da conta e não é um custo escondido que aparece depois.

## 3. O erro de período que foi ao ar

O slide 9 do deck apresentado afirma:

> **720** viagens organizadas por ano
> **R$ 72 mil** por turma/ano só em taxas de serviço (média R$ 100)

Os dois valores estão corretos em magnitude e errados em período. A conta é 100 alunos × 60% × 12 módulos = 720 viagens — mas esses 12 módulos acontecem ao longo dos **20 meses** do programa, não de 12.

| | Apresentado | Correto |
|---|---|---|
| Viagens por turma/ano | 720 | **432** |
| Receita de taxa por turma/ano | R$ 72 mil | **R$ 43,2 mil** |
| Viagens no ciclo completo | — | 720 |
| Receita de taxa no ciclo completo | — | R$ 72 mil |

O erro superestima a receita anual por turma em 67%.

### O que isso afeta e o que não afeta

**Não afeta a projeção da Sprint 4.** O modelo foi construído a partir do ritmo correto (0,6 módulo por aluno por mês) e nunca usou o número anualizado da banca. Os R$ 4,58 milhões do cenário tendencial permanecem válidos.

**Afeta o que foi dito à banca.** Se algum avaliador dividir 12 módulos por 20 meses, encontra a inconsistência. Como a apresentação já ocorreu, não há o que corrigir no material apresentado.

**Encaminhamento:** usar os valores corretos daqui em diante — Sprint 5, Sprint 6 e Demo Day. Se a banca tiver apontado o problema no feedback, registrar isso em [`../sprint-03/banca-de-modelagem/README.md`](../sprint-03/banca-de-modelagem/README.md). Se não apontou, seguir sem reabrir o assunto: o número correto é mais conservador, e chegar ao Demo Day com ele já ajustado é a postura defensável.

## 4. A terceira fonte de receita

A banca apresentou três fontes: taxa de serviço, comissão sobre bloqueios e fee da escola por turma. A Sprint 4 modela apenas as duas primeiras e mantém o fee da escola em zero.

Não é uma contradição — a banca já classificava o fee como "receita potencial, a validar como evolução do modelo". A Sprint 4 leva isso a sério e o mantém fora da projeção, porque incluí-lo contrariaria o próprio desenho comercial: a escola participa sem desembolso, e é justamente isso que torna a venda fácil.

**Encaminhamento:** manter fora dos cenários. Citá-lo como alavanca futura, nunca como receita projetada.

## O que a Sprint 4 acrescenta ao que foi apresentado

A banca tratou o financeiro em um único slide ilustrativo. A Sprint 4 substitui aquele slide por um modelo:

- **A comissão ganhou número.** A banca dizia "percentual sobre as tarifas negociadas". Agora são 6,4% do ticket, abertos por aéreo (4%), hotel (10%) e traslado (10%).
- **O mercado ganhou tamanho.** TAM, SAM e SOM com memória de cálculo, ausentes da banca.
- **O preço ganhou justificativa.** R$ 100 deixou de ser o meio da faixa da H6 e passou a ser ancorado na economia de R$ 500 entregue.
- **A projeção ganhou horizonte e cenários.** 12 trimestres, três cenários e análise de sensibilidade.
- **O risco principal mudou de lugar.** A sensibilidade mostra que o ritmo de contratação de turmas pesa mais que a adesão, que era o risco enfatizado na banca.
