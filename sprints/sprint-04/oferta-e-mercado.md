# 08 · Oferta e potencial de mercado

## O que será vendido

**Um serviço de concierge de viagem por assinatura de turma**, cobrado por módulo cursado. O aluno paga uma taxa de serviço por encontro; a Antévia organiza passagem, hotel e traslado do programa inteiro.

No primeiro ano a compra é feita **através de uma consolidadora parceira**, aproveitando o convênio que ela já tem. O bloqueio de grupo próprio só entra quando a operação concentra volume suficiente — ver [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

Não vendemos a passagem. Vendemos a **função de gestor de viagens do aluno** — a compra acontece na janela certa porque a plataforma conhece o calendário do programa desde a matrícula.

## Para quem será vendido

Mercado de dois lados, com um único pagador:

| Lado | Quem | Papel | Paga? |
|---|---|---|---|
| PF | Aluno-executivo viajante de campus com fluxo de fora | Usa e paga a taxa | Sim |
| B2B | Escola de negócios (coordenação de programas) | Dá acesso à turma e ao calendário das datas | Não |

A escola não desembolsa. Ela empresta o CNPJ e o calendário, indica a Antévia na matrícula e ganha NPS. Essa assimetria é deliberada: nenhuma verba nova precisa ser aprovada para o negócio começar.

## Como será vendido

1. **A meta é captar alunos, não turmas.** O ano 1 tem meta de 100 alunos captados, somando todas as turmas e instituições. Cada aluno gera 12 módulos ao longo de 20 meses — receita recorrente por quase dois anos.
2. **Distribuição pelo canal da escola.** A oferta chega ao aluno no ato da matrícula, junto com o calendário. Custo de aquisição próximo de zero por aluno.
3. **Adesão voluntária.** O aluno decide módulo a módulo. Nada é imposto — condição da escola para indicar (ver [personas.md](../sprint-03/personas.md)).

## Potencial de mercado

Construído de baixo para cima, a partir da base do IBGE já usada na Sprint 1. Cada premissa está identificada e rastreada em [premissas.md](premissas.md).

### TAM — Brasil

| # | Etapa | Cálculo | Resultado |
|---|---|---|---|
| 1 | Matriculados em pós-graduação (IBGE) | base | 1.400.000 |
| 2 | Em programas executivos presenciais e periódicos (P1: 12%) | 1.400.000 × 12% | 168.000 |
| 3 | Que viajam de outra cidade — "fluxo de fora" (P2: 25%) | 168.000 × 25% | **42.000 alunos-viajantes** |
| 4 | Viagens por ano (12 módulos ÷ 20 meses × 12) | 42.000 × 7,2 | **302.400 viagens/ano** |
| 5 | Volume logístico transacionável (ticket maduro R$ 1.700) | 302.400 × 1.700 | **R$ 514 mi/ano** |
| 6 | Receita capturável (R$ 208,80 por viagem) | 302.400 × 208,80 | **R$ 63,1 mi/ano** |

O TAM usa o ticket e a comissão da **fase 3** — é o tamanho do mercado para um operador maduro, não para quem está começando.

### SAM — campi com fluxo de fora

A dor não é universal: concentra-se em Nova Lima, São Paulo e Rio (achado das entrevistas com Manaus e Belém). O SAM restringe o TAM às escolas de grande porte nesses campi — **25% do TAM (P3)**.

- 10.500 alunos-viajantes · 75.600 viagens/ano
- **R$ 15,8 mi/ano** de receita capturável

### SOM — 3 anos, cenário tendencial

| Fim do | Alunos ativos | Receita anualizada | % do SAM |
|---|---|---|---|
| Ano 1 | 100 | R$ 113 mil | 1,0% |
| Ano 2 | 280 | R$ 383 mil | 2,7% |
| Ano 3 | 650 | R$ 977 mil | **6,2%** |

Chegar a 6,2% do SAM em três anos é defensável para um negócio que capta aluno a aluno, pelo canal da escola.

A primeira versão deste documento projetava 24% do SAM, apoiada em turma de 100 alunos e adesão de 60% desde o primeiro trimestre. Não se sustentava. O racional da revisão está em [viabilidade-do-primeiro-ano.md](viabilidade-do-primeiro-ano.md).

## O que é receita e o que não é

Uma distinção que precisa ficar explícita, porque muda a leitura de todos os números desta sprint.

**A Antévia não compra e revende passagem.** O aluno paga a companhia aérea e o hotel; a Antévia intermedeia. Isso significa que **o ticket de R$ 1.920 não é custo nosso** — é dinheiro que passa pelo aluno para o fornecedor.

| Conceito | O que é | Valor por viagem (fase 1) |
|---|---|---|
| **GMV** — volume transacionado | O que o aluno paga aos fornecedores | R$ 1.920 |
| **Receita da Antévia** | Taxa de serviço + comissão dos fornecedores | R$ 157,60 |
| Custo direto de vendas | Não existe neste modelo | R$ 0 |

Consequências:

1. **Não há margem bruta a apresentar na Sprint 4.** Sem custo de mercadoria vendida, receita e margem de contribuição se confundem. Os R$ 1,10 milhão dos três anos são receita líquida de intermediação, não faturamento bruto.
2. **Todos os custos são operacionais.** Time de concierge, plataforma, administrativo, conformidade, meios de pagamento e capital de giro entram como custos e despesas — matéria da **Sprint 5**, que trata de OPEX e CAPEX.
3. **O GMV importa mesmo assim**, por dois motivos: é o que determina a faixa de comissão junto aos fornecedores, e é a base sobre a qual se calcula a economia entregue ao aluno.

Se o modelo fosse de revenda — a Antévia comprando em nome próprio e faturando o valor cheio —, a receita de 3 anos seria o GMV de R$ 9,61 milhões e apareceria um custo de mercadoria de cerca de R$ 8,5 milhões. O resultado final seria o mesmo; a apresentação, bem diferente. Optamos pela forma que descreve o negócio como ele funciona.

## Estrutura para atuar em cada segmento

O Encontro 5 pede quais segmentos serão acessados em cada período e com que estrutura. O dimensionamento de pessoas e custos é da Sprint 5; aqui fica o desenho de cobertura.

| Período | Segmento acessado | Estrutura para atuar |
|---|---|---|
| **Ano 1** | 1 a 2 campi com fluxo de fora, priorizando Nova Lima | Operação conduzida pelos sócios. Compra via consolidadora parceira, sem estrutura de compras própria. Atendimento por WhatsApp e planilha |
| **Ano 2** | Ampliação para São Paulo e Rio; múltiplas turmas por campus | Primeiros concierges dedicados. Plataforma com calendário e painel de custos. Negociação de bloqueios pontuais nas rotas que concentram |
| **Ano 3** | Escolas de negócios além da FDC, mesmos eixos | Time de concierge por carteira de campus. Convênio próprio com companhias e hotéis. Área de relacionamento institucional para abrir novas escolas |

A progressão é deliberada: **a estrutura só cresce depois que o volume aparece.** No ano 1 não há equipe contratada porque não há receita que a sustente — o que a [`viabilidade-do-primeiro-ano.md`](viabilidade-do-primeiro-ano.md) detalha.

## Ticket logístico por módulo

Aluno de fora, ida e volta mais duas diárias. Hoje ele desembolsa R$ 2.200 comprando em cima da hora.

O que a Antévia consegue **depende do poder de negociação, que ela não tem no começo**. Por isso o ticket evolui em três fases:

| Item | Hoje | Fase 1 (ano 1) | Fase 2 (ano 2) | Fase 3 (ano 3) |
|---|---|---|---|---|
| Aéreo | R$ 1.400 | R$ 1.150 | R$ 1.080 | R$ 1.020 |
| Hotel (2 diárias) | R$ 600 | R$ 570 | R$ 530 | R$ 500 |
| Traslado | R$ 200 | R$ 200 | R$ 190 | R$ 180 |
| **Subtotal logístico** | **R$ 2.200** | **R$ 1.920** | **R$ 1.800** | **R$ 1.700** |
| Taxa de serviço Antévia | — | R$ 100 | R$ 100 | R$ 100 |
| **Total desembolsado** | **R$ 2.200** | **R$ 2.020** | **R$ 1.900** | **R$ 1.800** |
| **Economia líquida do aluno** | — | **R$ 180** | **R$ 300** | **R$ 400** |
| Redução no desembolso | — | 8,2% | 13,6% | 18,2% |

Na **fase 1 a economia vem apenas da antecipação** — comprar aos 90 dias em vez de menos de 30. Essa alavanca não exige negociar com nenhum fornecedor: é a curva tarifária pública. É o que torna o ano 1 possível sem poder de barganha, e também o que limita o que ele entrega.

A meta de −15% a −25% fixada no objetivo de longo prazo da Sprint 1 só é atingida na **fase 3**. Nas fases anteriores o aluno economiza menos, e isso precisa ser dito — inclusive para ele.
