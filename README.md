# Antévia

**A logística da sua formação, no tempo certo.**

Projeto do **Grupo Kairós** no programa **Business Designer** da Fundação Dom Cabral (FDC).

## O que é

A Antévia é o **concierge de viagem do aluno-executivo**: uma plataforma integrada ao calendário acadêmico que antecipa e organiza passagem, hotel e traslado de todos os módulos de um programa executivo em um só lugar — com custo previsível desde o início e a liberdade de o aluno manter companhia aérea e milhas.

## O problema

A logística de viagem para programas executivos presenciais e periódicos é fragmentada e reativa, sem integração ao calendário acadêmico — comprometendo o foco, o orçamento e a experiência da formação do aluno.

Na prática: o aluno conhece as datas desde a matrícula, mas compra com menos de 30 dias (pagando 2–3× mais), usa 3+ plataformas por viagem e fecha o reembolso na planilha. A cada módulo, tudo se repete.

## Estado do projeto

| Etapa | Status |
|---|---|
| Sprint 1 — Diagnóstico (problema, contexto, hipóteses, entrevistas) | Concluída |
| Sprint 2 — Solução, stakeholders, VPD, nome e marca | Concluída |
| Sprint 3 — Solução formalizada, BMC e personas | Concluída |
| Banca de Modelagem — pitch de 10 minutos | Deck pronto, apresentação a realizar |

## Estrutura do repositório

```
docs/            Documentação do projeto (contexto, solução, modelo, personas, jornada, financeiro)
marca/           Identidade visual e diretrizes de escrita
apresentacoes/   Decks finais (.pptx)
```

Comece por [`docs/01-contexto-e-problema.md`](docs/01-contexto-e-problema.md) e siga a numeração.

## Decisões-chave (resumo)

- **Concierge, não marketplace.** O produto é a função "gestor de viagens do aluno", que hoje não existe — não uma plataforma de compra.
- **Modelo comercial já existente.** Bloqueio de grupo: escola (CNPJ) + turma + datas fixas do calendário. Não é preciso inventar o produto comercial.
- **Números calibrados por entrevistas.** Adesão realista de 50–70% (não 100%), desconto de bloqueio de 20–30% (não 40–50%), meta de custo de −15% a −25%.
- **A dor não é universal.** Concentra-se em campi com fluxo de alunos de fora (Nova Lima, SP, Rio) — variável central de escopo.
- **Nada é imposto ao aluno.** Condição da escola para indicar o serviço; o aluno mantém companhia, voo e milhas.
