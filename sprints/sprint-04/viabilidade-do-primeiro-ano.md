# 13 · A dificuldade do primeiro ano

Este documento existe porque duas premissas da primeira versão da Sprint 4 não se sustentaram sob questionamento do grupo. Ele revisa o que estava errado, refaz as contas e reposiciona o primeiro ano como a fase mais difícil do negócio — que é o que ele de fato é.

## O que estava errado

### 1. O "100 alunos" foi lido como tamanho de turma, e não é

A premissa P5 estava registrada como "100 alunos por turma · Padrão FDC · Validada". Errado duas vezes.

O número vem do bloco **"Exemplo ilustrativo"** de [atores-e-financeiro.md](../sprint-03/banca-de-modelagem/atores-e-financeiro.md), da Banca de Modelagem — e ali ele **não se refere a turma nenhuma**. O exemplo diz "100 alunos · 12 encontros", sem citar turmas, instituições ou taxa de adesão. É uma meta de captação.

Duas correções decorrem disso:

- **Turmas da FDC têm por volta de 40 alunos**, não 100 (informação do grupo).
- **Os 100 alunos são a meta do ano 1**, somando todas as turmas e instituições. O modelo passou a ser dirigido por essa variável, e a turma saiu da conta de receita.

Isso simplifica o modelo e elimina as duas premissas mais frágeis que ele tinha: tamanho de turma e taxa de adesão dentro dela.

### 2. O poder de negociação foi assumido desde o dia um

A primeira versão aplicava 6,4% de comissão e 20–30% de desconto de bloqueio já no T1. Isso pressupõe um poder de barganha que uma empresa sem histórico e sem volume não tem.

A pergunta que derruba a premissa: **por que uma companhia aérea venderia mais barato para a Antévia do que vende direto para o aluno?** No primeiro ano, com uma ou duas instituições e algumas dezenas de aderentes, a resposta honesta é: **não venderia.**

## De onde vem a economia quando não há poder de barganha

A confusão da primeira versão foi tratar como uma só coisa duas alavancas com naturezas diferentes:

| Alavanca | Depende de | Disponível quando |
|---|---|---|
| **Antecipação** — comprar aos 90 dias em vez de <30 | Nada. É a curva tarifária pública | **Desde o primeiro dia** |
| **Tarifa de grupo** — bloqueio para 10+ pax na mesma rota | Concentração de passageiros | Quando a operação concentra volume |
| **Convênio corporativo** — desconto por compromisso anual | Volume anual contratado | Quando o volume anual justifica |

A primeira alavanca é gratuita e não exige negociação com ninguém. **É ela, e só ela, que sustenta o primeiro ano.** As outras duas se conquistam com o tempo.

Vale dizer com todas as letras: no ano 1 a Antévia não negocia com companhia aérea. Ela **se apoia na consolidadora** — uma agência B2B que já tem convênio e volume, como a Velt — e recebe repasse de parte da comissão dela. É o caminho padrão de quem começa, e foi exatamente o interlocutor que o grupo já entrevistou na Sprint 1.

## As três fases de poder de negociação

As faixas vêm da entrevista com Bruno Brant (Velt): convênio de R$ 250–500 mil/ano rende 3–5%; a partir de R$ 1 milhão/ano, 8–12%.

| Fase | Ano | Como compramos | Ticket | Economia do aluno | Retorno sobre a taxa | Comissão |
|---|---|---|---|---|---|---|
| 1 | Ano 1 | Apoio da consolidadora; só antecipação | R$ 1.920 | R$ 180 líquidos | 1,8× | 3% |
| 2 | Ano 2 | Bloqueios pontuais nas rotas que concentram | R$ 1.800 | R$ 300 líquidos | 3,0× | 5% |
| 3 | Ano 3 | Convênio próprio | R$ 1.700 | R$ 400 líquidos | 4,0× | 6,4% |

Referência: hoje o aluno desembolsa R$ 2.200 por módulo comprando em cima da hora.

### As comissões batem com o volume?

Teste feito contra as faixas da Velt, usando o volume aéreo do cenário tendencial:

| Ano | Volume aéreo | Faixa que esse volume abre | Comissão assumida |
|---|---|---|---|
| 1 | R$ 518 mil | R$ 250–500 mil — entrada da faixa de 3–5% | 3% |
| 2 | R$ 1,61 mi | Acima de R$ 1 mi — 8% a 12% | 5% |
| 3 | R$ 3,64 mi | Acima de R$ 1 mi — 8% a 12% | 6,4% |

A meta de 100 alunos coloca o ano 1 **exatamente na entrada da faixa de convênio**, o que sustenta os 3% assumidos. Os anos 2 e 3 usam comissões **abaixo** do que o volume permitiria: a projeção é conservadora de propósito, porque conquistar a faixa cheia leva tempo além de volume.

Vale notar o contraste com a versão anterior, que modelava por turmas e chegava a R$ 248 mil de volume aéreo no ano 1 — abaixo do piso. A releitura dos 100 alunos como meta de captação anual muda essa conclusão: o ano 1 já entra na faixa negociável.

## A concentração é o que destrava a tarifa de grupo

Tarifa de grupo exige em torno de **10 passageiros na mesma rota e no mesmo voo**. As 5 condições mapeadas com a Velt já diziam "rota concentrada, 5 a 8 origens". Faltava fazer a divisão.

Com a captação medida em alunos, a pergunta certa passa a ser: **quantos alunos a operação reúne no mesmo campus e na mesma data?**

| Alunos no mesmo campus/data | 5 origens | 6 origens | 8 origens |
|---|---|---|---|
| 100 | 20,0 pax | 16,7 pax | 12,5 pax |
| 50 | 10,0 pax | 8,3 pax | 6,2 pax |
| 25 | 5,0 pax | 4,2 pax | 3,1 pax |

**O limiar prático fica entre 50 e 60 alunos por campus e data.** A meta de 100 alunos no ano 1, se concentrada, ultrapassa esse limiar com folga — e é isso que torna a fase 2 alcançável.

O contraste com a turma isolada é o ponto: uma turma de 40 alunos, mesmo com metade viajando, rende 20 alunos por data e cerca de 3 passageiros por rota. **Nenhuma turma sozinha forma grupo.** A concentração tem que vir de somar turmas no mesmo campus e data.

### O que isso muda no desenho do negócio

A unidade de negociação **não pode ser a turma**. Precisa ser o **campus numa data**: alunos de várias turmas que chegam ao mesmo lugar no mesmo dia, somados.

Quantos alunos concentrados são necessários para formar grupo:

| Origens principais | Alunos no mesmo campus/data |
|---|---|
| 5 origens | 50 alunos |
| 6 origens | 60 alunos |
| 8 origens | 80 alunos |

Com 100 alunos captados no ano 1, o limiar é alcançável — desde que a captação seja concentrada e não pulverizada entre campi e datas.

Consequências diretas:

1. **A venda muda de alvo.** Não adianta captar alunos dispersos. É preciso concentrá-los — mesmo campus, datas que se sobrepõem.
2. **O bloqueio é da Antévia, não da escola.** Se o volume vem de somar alunos de várias turmas, quem agrega é a plataforma. O ativo passa a ser nosso, não emprestado.
3. **A meta do ano 1 tem duas dimensões.** Captar 100 alunos é metade; a outra metade é que eles se concentrem o bastante para ligar a alavanca de grupo.

## O primeiro ano, refeito

Premissa revista: **100 alunos captados até o fim do ano 1**, somando todas as turmas e instituições, com rampa trimestral de 25 → 50 → 75 → 100.

| | Ano 1 | Ano 2 | Ano 3 | Total |
|---|---:|---:|---:|---:|
| Alunos ativos ao fim do ano | 100 | 280 | 650 | — |
| Receita (tendencial) | **R$ 70.920** | R$ 283.860 | R$ 744.163 | **R$ 1.098.943** |
| Viagens | 450 | 1.494 | 3.564 | 5.508 |

Comparação com a primeira versão da Sprint 4:

| | Antes | Agora | Variação |
|---|---:|---:|---:|
| Receita do ano 1 | R$ 293.155 | R$ 70.920 | **−76%** |
| Receita em 3 anos | R$ 4.577.731 | R$ 1.098.943 | **−76%** |
| Fatia do SAM no T12 | 24,0% | 6,2% | — |

Os 24% do SAM em três anos não se defendiam. Os 6,2% se defendem.

### O que o ano 1 significa na prática

**R$ 71 mil de receita não pagam uma equipe.** É menos de R$ 6 mil por mês. O ano 1 não comporta equipe contratada, escritório ou investimento em tecnologia relevante — ou os sócios operam a coisa com as próprias mãos, ou é preciso capital para atravessar.

Isso não é defeito da projeção. É a descrição correta de um negócio que precisa de volume para ter margem e não tem volume no começo. A Sprint 5 vai dimensionar quanto custa atravessar esse período, e a Sprint 6 vai dizer quanto capital isso exige.

### O ano 1 não é sobre receita

Se o ano 1 rende R$ 71 mil, ele não pode ser medido por receita. Ele existe para produzir três ativos que destravam a fase 2:

| Ativo | Para que serve |
|---|---|
| Prova de execução | Um ciclo entregue vira referência para captar os alunos do ano 2 |
| Volume acumulado | Cruzar R$ 1 mi/ano em aéreo abre a faixa de 8–12% de comissão |
| Concentração de campus | Reunir 50–60 alunos numa data liga a tarifa de grupo |

A métrica do ano 1 é **alunos captados e concentração por campus**, não faturamento.

## O que ainda precisa ser validado, em ordem

| # | Premissa | Valor usado | Impacto | Como validar |
|---|---|---|---|---|
| 1 | **Alunos captados no ano 1** | 100 | É a variável dominante (±30%) | Coordenação de campus com fluxo de fora |
| 2 | Concentração por campus e data | 50–60 alunos | Define quando a tarifa de grupo liga | Calendário acadêmico dos campi |
| 3 | Disposição a pagar (H6) | R$ 100/módulo | Responde por 63% da receita no ano 1 | Aluno-executivo viajante |
| 4 | Desconto real da antecipação aos 90 dias | 13% no aéreo | É a única alavanca do ano 1 | Cotação com consolidadora |
| 5 | Repasse da consolidadora ao parceiro | 3% | É a receita variável do ano 1 | Conversa com a Velt |

A primeira é a que o grupo mais controla — e também a que não tem nenhuma referência externa. Nenhuma das três entrevistas da Sprint 1 tratou de ciclo de captação.
