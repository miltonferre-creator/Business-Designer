# Antévia

**A logística da sua formação, no tempo certo.**

Projeto do **Grupo Kairós** no programa **Business Designer** da Fundação Dom Cabral (FDC).

## O que é

A Antévia é o **concierge de viagem do aluno-executivo**: uma plataforma integrada ao calendário acadêmico que antecipa e organiza passagem, hotel e traslado de todos os módulos de um programa executivo em um só lugar — com custo previsível desde o início e a liberdade de o aluno manter companhia aérea e milhas.

**Nome:** Antévia = antes + via — o caminho resolvido antes da hora.

## O problema

A logística de viagem para programas executivos presenciais e periódicos é fragmentada e reativa, sem integração ao calendário acadêmico — comprometendo o foco, o orçamento e a experiência da formação do aluno.

Na prática: o aluno conhece as datas desde a matrícula, mas compra com menos de 30 dias (pagando 2–3× mais), usa 3+ plataformas por viagem e fecha o reembolso na planilha. A cada módulo, tudo se repete.

## Estado do projeto

| Etapa | Status | Pasta |
|---|---|---|
| Sprint 1 — Diagnóstico: problema, contexto, hipóteses e entrevistas | ✅ Concluída | [`sprints/sprint-01/`](sprints/sprint-01/) |
| Sprint 2 — Desenho da solução: stakeholders, VPD, nome e marca | ✅ Concluída | [`sprints/sprint-02/`](sprints/sprint-02/) |
| Sprint 3 — Solução formalizada, BMC e personas | ✅ Concluída | [`sprints/sprint-03/`](sprints/sprint-03/) |
| Banca de Modelagem — pitch de 10 minutos | ✅ Apresentada | [`sprints/sprint-03/banca-de-modelagem/`](sprints/sprint-03/banca-de-modelagem/) |
| Sprint 4 — Viabilidade: projeção de receitas | ✅ Concluída | [`sprints/sprint-04/`](sprints/sprint-04/) |
| Sprint 5 — Viabilidade: custos, despesas e investimentos | ⬜ A fazer | — |
| Sprint 6 — Plano de implementação | ⬜ A fazer | — |
| Demo Day — pitch final de 10 minutos | ⬜ A fazer | — |

## Estrutura do repositório

```
sprints/
├── sprint-01/                Diagnóstico: problema, contexto, hipóteses e entrevistas
│   └── entregaveis/          Sprint_01_Kairos_Apresentacao_Final.pptx ✓
├── sprint-02/                Desenho da solução: stakeholders, VPD, nome e marca
│   └── entregaveis/          Sprint_02_Kairos_Antevia.pptx + guia da marca (PDF) ✓
├── sprint-03/                Solução formalizada, BMC e personas
│   ├── entregaveis/          Sprint_03_Kairos_Antevia.pptx ✓
│   └── banca-de-modelagem/   Pitch de 10 min: jornada, diferenciais, atores e financeiro
│       └── entregaveis/      Banca_Modelagem_Kairos_Antevia.pptx ✓
└── sprint-04/                Viabilidade: mercado, preço, cenários e o desafio do primeiro ano
    └── entregaveis/          Sprint_04_Kairos_Antevia.pptx + modelo de receitas (XLSX) ✓
marca/                        Identidade visual "Minimal Future" e diretrizes de escrita
└── assets/                   antevia_logo.png, antevia_appicon.png ✓
apresentacoes/                Cópias dos decks de Sprint 3 e da banca, reunidas para uso em sala
```

Cada pasta tem um `README.md` com o resumo da etapa. Comece por [`sprints/sprint-01/README.md`](sprints/sprint-01/README.md) e siga a ordem.

## Como navegar por tema

| Quero entender... | Onde ler |
|---|---|
| O problema e o contexto de mercado | [`sprints/sprint-01/contexto-e-problema.md`](sprints/sprint-01/contexto-e-problema.md) |
| O que as entrevistas revelaram | [`sprints/sprint-01/hipoteses-e-entrevistas.md`](sprints/sprint-01/hipoteses-e-entrevistas.md) |
| A solução, o nome e o slogan | [`sprints/sprint-03/solucao.md`](sprints/sprint-03/solucao.md) |
| O modelo de negócio e os diferenciais | [`sprints/sprint-03/modelo-de-negocio.md`](sprints/sprint-03/modelo-de-negocio.md) |
| Quem são os clientes | [`sprints/sprint-03/personas.md`](sprints/sprint-03/personas.md) |
| Como o serviço funciona na prática | [`sprints/sprint-03/banca-de-modelagem/jornada-do-cliente.md`](sprints/sprint-03/banca-de-modelagem/jornada-do-cliente.md) |
| Quem faz o negócio funcionar e as receitas | [`sprints/sprint-03/banca-de-modelagem/atores-e-financeiro.md`](sprints/sprint-03/banca-de-modelagem/atores-e-financeiro.md) |
| O tamanho do mercado e o que vendemos | [`sprints/sprint-04/oferta-e-mercado.md`](sprints/sprint-04/oferta-e-mercado.md) |
| Como o preço foi definido | [`sprints/sprint-04/precificacao.md`](sprints/sprint-04/precificacao.md) |
| Quanto o negócio fatura e em que cenários | [`sprints/sprint-04/cenarios-de-receita.md`](sprints/sprint-04/cenarios-de-receita.md) |
| De onde vem cada número | [`sprints/sprint-04/premissas.md`](sprints/sprint-04/premissas.md) |
| Por que o primeiro ano é o mais difícil | [`sprints/sprint-04/viabilidade-do-primeiro-ano.md`](sprints/sprint-04/viabilidade-do-primeiro-ano.md) |
| Se a Sprint 4 bate com o que foi à banca | [`sprints/sprint-04/consistencia-com-a-banca.md`](sprints/sprint-04/consistencia-com-a-banca.md) |
| A identidade visual | [`marca/identidade-visual.md`](marca/identidade-visual.md) |

## Decisões-chave (resumo)

- **Concierge, não marketplace.** O produto é a função "gestor de viagens do aluno", que hoje não existe — não uma plataforma de compra.
- **Modelo comercial já existente — mas não desde o dia um.** O bloqueio de grupo é praticado no mercado e não precisa ser inventado. Só que ele exige volume: no início a compra passa por uma consolidadora parceira.
- **Números calibrados por entrevistas.** Desconto de bloqueio de 20–30% (não 40–50%) — faixa que descreve a **operação madura**. O ano 1 opera sem bloqueio próprio, apoiado numa consolidadora.
- **A dor não é universal.** Concentra-se em campi com fluxo de alunos de fora (Nova Lima, SP, Rio) — variável central de escopo.
- **Nada é imposto ao aluno.** Condição da escola para indicar o serviço; o aluno mantém companhia, voo e milhas.
- **O preço se ancora na economia entregue,** mas a economia cresce com o tempo. O aluno recebe R$ 180 líquidos por módulo no ano 1 e R$ 400 no ano 3 — retorno de 1,8× subindo para 4× (Sprint 4).
- **No primeiro ano não há poder de negociação.** A economia vem só da antecipação, que é a curva tarifária pública e não exige negociar com fornecedor. A compra é feita através de uma consolidadora parceira; bloqueio próprio e convênio vêm com volume (Sprint 4).
- **A unidade de negociação é o campus numa data, não a turma.** A tarifa de grupo exige 10 passageiros por rota, o que pede 50 a 60 alunos concentrados numa mesma data. Nenhuma turma isolada chega lá — a captação precisa ser concentrada (Sprint 4).

## Números do negócio (cenário tendencial, 3 anos)

| Indicador | Valor |
|---|---|
| Receita acumulada | R$ 1,10 mi |
| Receita do ano 1 | R$ 70,9 mil |
| Economia devolvida aos alunos | R$ 1,95 mi |
| Viagens organizadas | 5.508 |
| Alunos ativos no T12 | 650 — 6,2% do mercado onde podemos atuar |

Faixa dos cenários: R$ 551 mil (pessimista) · R$ 1,10 mi (tendencial) · R$ 1,83 mi (otimista). Memória de cálculo em [`sprints/sprint-04/`](sprints/sprint-04/).

A meta do ano 1 é **captar 100 alunos**, somando todas as turmas e instituições. Isso rende R$ 71 mil — menos de R$ 6 mil por mês, que não paga equipe. Quanto custa atravessar esse período é a pergunta da Sprint 5.

## Próximos passos

- Registrar o feedback da Banca de Modelagem em [`sprints/sprint-03/banca-de-modelagem/`](sprints/sprint-03/banca-de-modelagem/)
- Parar de usar "720 viagens / R$ 72 mil por turma/ano" do deck da banca — com 100 alunos captados são 180 viagens no ano 1, não 720 ([conferência](sprints/sprint-04/consistencia-com-a-banca.md))
- Validar a meta de captação de 100 alunos no ano 1 com coordenação de campus com fluxo de fora — é a variável dominante do modelo (±30%)
- Conferir, no calendário acadêmico dos campi, se dá para concentrar 50 a 60 alunos numa mesma data — é o que liga a tarifa de grupo
- Validar H2 (tempo por encontro) e H6 (disposição a pagar R$ 50–150) com alunos-executivos
- Iniciar a Sprint 5: custos, despesas, investimentos, macroprocesso e DFC de 3 anos — respondendo quanto capital é preciso para atravessar um ano 1 de R$ 71 mil
- Adicionar os PDFs complementares da Sprint 1 (resumos, mapa de contexto, hipóteses), se localizados
- Acompanhar o registro formal da marca no INPI
