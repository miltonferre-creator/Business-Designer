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
| Banca de Modelagem — pitch de 10 minutos | 🎤 Deck pronto, apresentação a realizar | [`sprints/sprint-03/banca-de-modelagem/`](sprints/sprint-03/banca-de-modelagem/) |
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
└── sprint-04/                Viabilidade: mercado, preço e cenários de receita
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
| A identidade visual | [`marca/identidade-visual.md`](marca/identidade-visual.md) |

## Decisões-chave (resumo)

- **Concierge, não marketplace.** O produto é a função "gestor de viagens do aluno", que hoje não existe — não uma plataforma de compra.
- **Modelo comercial já existente.** Bloqueio de grupo: escola (CNPJ) + turma + datas fixas do calendário. Não é preciso inventar o produto comercial.
- **Números calibrados por entrevistas.** Adesão realista de 50–70% (não 100%), desconto de bloqueio de 20–30% (não 40–50%), meta de custo de −15% a −25%.
- **A dor não é universal.** Concentra-se em campi com fluxo de alunos de fora (Nova Lima, SP, Rio) — variável central de escopo.
- **Nada é imposto ao aluno.** Condição da escola para indicar o serviço; o aluno mantém companhia, voo e milhas.
- **O preço se ancora na economia entregue.** R$ 100 por módulo contra R$ 500 de economia — o aluno recebe R$ 400 líquidos de volta. Isso tira a precificação da disposição a pagar declarada (Sprint 4).
- **O gargalo é assinar turmas, não convencer alunos.** A análise de sensibilidade aponta o ritmo de contratação (±30%) à frente da adesão (±17%) — invertendo a prioridade que o grupo vinha adotando (Sprint 4).

## Números do negócio (cenário tendencial, 3 anos)

| Indicador | Valor |
|---|---|
| Receita acumulada | R$ 4,58 mi |
| Economia devolvida aos alunos | R$ 8,77 mi |
| Viagens organizadas | 21.924 |
| Turmas ativas no T12 | 42 |

Faixa dos cenários: R$ 1,42 mi (pessimista) · R$ 4,58 mi (tendencial) · R$ 11,96 mi (otimista). Memória de cálculo em [`sprints/sprint-04/`](sprints/sprint-04/).

## Próximos passos

- Apresentar à Banca de Modelagem e registrar o feedback em [`sprints/sprint-03/banca-de-modelagem/`](sprints/sprint-03/banca-de-modelagem/)
- Corrigir "720 viagens / R$ 72 mil por turma/ano" no material da banca — os valores são do ciclo de 20 meses, não de um ano ([detalhe](sprints/sprint-04/cenarios-de-receita.md))
- Entrevistar coordenação de campus com fluxo de fora para validar o ritmo de contratação de turmas — variável de maior impacto na projeção
- Validar H2 (tempo por encontro) e H6 (disposição a pagar R$ 50–150) com alunos-executivos
- Iniciar a Sprint 5: custos, despesas, investimentos, macroprocesso e DFC de 3 anos
- Adicionar os PDFs complementares da Sprint 1 (resumos, mapa de contexto, hipóteses), se localizados
- Acompanhar o registro formal da marca no INPI
