# Sprint 4 — Viabilidade: Projeção de Receitas

**Objetivo da sprint (Squeeze 4):** traduzir o modelo de negócio em números — dimensionar o mercado, pesquisar e definir o preço, e projetar a receita em três cenários ao longo de 12 trimestres.

> **Segunda versão.** A primeira projetava R$ 4,58 mi em 3 anos apoiada em duas premissas que não se sustentaram: turma de 100 alunos tratada como fato validado, e poder de negociação com fornecedores desde o primeiro trimestre. A revisão está em [`viabilidade-do-primeiro-ano.md`](viabilidade-do-primeiro-ano.md).

## Documentos desta pasta

- [`oferta-e-mercado.md`](oferta-e-mercado.md) — o que será vendido, para quem e como; TAM, SAM e SOM; ticket por módulo em três fases
- [`precificacao.md`](precificacao.md) — pesquisa de preços, definição do preço e ancoragem no valor entregue
- [`cenarios-de-receita.md`](cenarios-de-receita.md) — volume por trimestre, três cenários e análise de sensibilidade
- [`premissas.md`](premissas.md) — as premissas com origem e status, fórmulas e o que ficou fora do modelo
- [`viabilidade-do-primeiro-ano.md`](viabilidade-do-primeiro-ano.md) — **por que o ano 1 é a fase mais difícil**, as três fases de poder de negociação e o problema do tamanho de grupo
- [`consistencia-com-a-banca.md`](consistencia-com-a-banca.md) — conferência contra o que foi defendido na Banca de Modelagem

## Números-síntese (cenário tendencial, 3 anos)

| Indicador | Valor |
|---|---|
| Receita acumulada | **R$ 959 mil** |
| Receita do ano 1 | **R$ 34 mil** |
| Volume transacionado (GMV) | R$ 8,24 mi |
| Viagens organizadas | 4.752 |
| Economia devolvida aos alunos | R$ 1,74 mi |
| Aderentes no T12 | 576 (5,5% do SAM) |

Faixa dos três cenários: **R$ 348 mil** (pessimista) · **R$ 959 mil** (tendencial) · **R$ 2,01 mi** (otimista).

## Principais resultados

- **O primeiro ano rende R$ 34 mil e não paga ninguém.** É menos de R$ 3 mil por mês. Ou os sócios operam com as próprias mãos, ou é preciso capital para atravessar. A Sprint 5 dimensiona o custo desse período.
- **No ano 1 não há poder de negociação.** A economia vem apenas da antecipação — comprar aos 90 dias em vez de menos de 30 —, que é a curva tarifária pública e não exige negociar com fornecedor. A compra é feita através de uma consolidadora parceira. Tarifa de grupo e convênio próprio vêm depois, com volume.
- **Uma turma isolada não forma tarifa de grupo.** Com 40 alunos e 30% de adesão em 5 origens, são 2,4 passageiros por rota — o mínimo de mercado é 10. A unidade de negociação precisa ser o campus numa data, somando 3 a 5 turmas simultâneas, e não a turma individual.
- **O retorno para o aluno começa em 1,8×, não em 4×.** Ele paga R$ 100 e recebe R$ 180 líquidos no ano 1, chegando a R$ 400 no ano 3. No começo a venda não se sustenta só no desconto: apoia-se no tempo devolvido.
- **O tamanho da turma é a premissa mais barata de validar e a que mais move o modelo.** Move a receita em +50% para cima. Nunca foi verificada com a escola.

## Entregáveis

- ✅ [`entregaveis/Sprint_04_Kairos_Antevia.pptx`](entregaveis/Sprint_04_Kairos_Antevia.pptx) — 11 slides para o Squeeze 4
- ✅ [`entregaveis/Antevia_Modelo_Receitas.xlsx`](entregaveis/Antevia_Modelo_Receitas.xlsx) — modelo com premissas isoladas para simulação, 12 trimestres, 3 cenários e sensibilidade

Cobertura dos itens pedidos no Encontro 5:

| Item | Onde |
|---|---|
| a. O que será ofertado, para quem e como | [`oferta-e-mercado.md`](oferta-e-mercado.md) |
| b. Potencial do negócio + memória de cálculo | [`oferta-e-mercado.md`](oferta-e-mercado.md) · [`premissas.md`](premissas.md) |
| c. Volume de ganhos por período | [`cenarios-de-receita.md`](cenarios-de-receita.md) |
| d. Pesquisa de preços | [`precificacao.md`](precificacao.md) |
| e. Definição de preços | [`precificacao.md`](precificacao.md) |
| f. Cenários de receitas por período | [`cenarios-de-receita.md`](cenarios-de-receita.md) |

Conferências adicionais, não pedidas pelo Encontro 5: [`viabilidade-do-primeiro-ano.md`](viabilidade-do-primeiro-ano.md) e [`consistencia-com-a-banca.md`](consistencia-com-a-banca.md).

## Validações pendentes

Em ordem de impacto sobre a projeção:

1. **Tamanho da turma** — usamos 40; a banca usou 100 sem verificação. Move a receita em +50%. Pergunta de dois minutos à secretaria da FDC.
2. **Adesão no ano 1, sem prova social** — usamos 30%. É a variável de maior queda (−33%). Entrevistar aluno-executivo viajante, que responde também a H6.
3. **Ritmo de contratação de turmas** — 24 turmas no T12, sem nenhuma referência externa. Entrevistar coordenação de campus com fluxo de fora.
4. **Desconto real da antecipação aos 90 dias** — 13% no aéreo. É a única alavanca do ano 1. Cotar com consolidadora.
5. **Repasse da consolidadora no ano 1** — 3%. Conversa com a Velt.
6. **Mínimo de passageiros para tarifa de grupo** — usamos 10. Define quando a fase 2 começa.

## Próxima etapa

Sprint 5 — projeção de custos, despesas e investimentos; macroprocesso do negócio; estrutura de pessoal; consolidação em DFC trimestral de 3 anos. A pergunta que ela precisa responder: **quanto capital é preciso para atravessar um primeiro ano de R$ 34 mil de receita.**
