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
