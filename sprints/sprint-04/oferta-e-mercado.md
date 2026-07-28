# 08 · Oferta e potencial de mercado

## O que será vendido

**Um serviço de concierge de viagem por assinatura de turma**, cobrado por módulo cursado. O aluno paga uma taxa de serviço por encontro; a Antévia organiza passagem, hotel e traslado dentro do bloqueio de grupo negociado com a escola.

Não vendemos a passagem. Vendemos a **função de gestor de viagens do aluno** — a compra acontece na janela certa porque a plataforma conhece o calendário do programa desde a matrícula.

## Para quem será vendido

Mercado de dois lados, com um único pagador:

| Lado | Quem | Papel | Paga? |
|---|---|---|---|
| PF | Aluno-executivo viajante de campus com fluxo de fora | Usa e paga a taxa | Sim |
| B2B | Escola de negócios (coordenação de programas) | Viabiliza o bloqueio: CNPJ + turma + datas | Não |

A escola não desembolsa. Ela empresta o CNPJ e o calendário, indica a Antévia na matrícula e ganha NPS. Essa assimetria é deliberada: nenhuma verba nova precisa ser aprovada para o negócio começar.

## Como será vendido

1. **Contrato por turma, não por aluno.** A unidade comercial é a turma — 100 alunos, 12 módulos, ciclo de 20 meses. Uma negociação abre 12 meses de receita recorrente.
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
| 5 | Volume logístico transacionável (ticket R$ 1.700) | 302.400 × 1.700 | **R$ 514 mi/ano** |
| 6 | Receita capturável (R$ 208,80 por viagem) | 302.400 × 208,80 | **R$ 63,1 mi/ano** |

### SAM — campi com fluxo de fora

A dor não é universal: concentra-se em Nova Lima, São Paulo e Rio (achado das entrevistas com Manaus e Belém). O SAM restringe o TAM às escolas de grande porte nesses campi — **25% do TAM (P3)**.

- 10.500 alunos-viajantes · 75.600 viagens/ano
- **R$ 15,8 mi/ano** de receita capturável

### SOM — 3 anos, cenário tendencial

| Fim do | Turmas ativas | Alunos aderentes | Receita anualizada | % do SAM |
|---|---|---|---|---|
| Ano 1 | 6 | 360 | R$ 541 mil | 3,4% |
| Ano 2 | 20 | 1.200 | R$ 1,80 mi | 11,4% |
| Ano 3 | 42 | 2.520 | R$ 3,79 mi | **24,0%** |

Chegar a um quarto do SAM em três anos é agressivo em qualquer mercado aberto. Aqui se sustenta por uma razão: **o canal é a escola, não o aluno.** Fechado o contrato com a coordenação, a oferta alcança a turma inteira de uma vez. O gargalo é assinar turmas — não convencer alunos, um a um.

Esse é o risco central do modelo, e a análise de sensibilidade em [cenarios-de-receita.md](cenarios-de-receita.md) o confirma.

## Ticket logístico por módulo

Aluno de fora, ida e volta mais duas diárias. Compara o que ele paga hoje com o que passa a pagar.

| Item | Hoje (compra <30 dias) | Com Antévia (bloqueio, 90 dias) | Variação |
|---|---|---|---|
| Aéreo | R$ 1.400 | R$ 1.020 | −27% |
| Hotel (2 diárias) | R$ 600 | R$ 500 | −17% |
| Traslado | R$ 200 | R$ 180 | −10% |
| **Subtotal logístico** | **R$ 2.200** | **R$ 1.700** | **−R$ 500** |
| Taxa de serviço Antévia | — | R$ 100 | +R$ 100 |
| **Total desembolsado** | **R$ 2.200** | **R$ 1.800** | **−R$ 400 (−18,2%)** |

Os −18,2% caem dentro da meta de −15% a −25% fixada no objetivo de longo prazo da Sprint 1. O modelo não foi calibrado para atingir a meta: a meta e o ticket foram construídos das mesmas premissas de desconto de bloqueio (20–30%) apuradas com a Velt.
