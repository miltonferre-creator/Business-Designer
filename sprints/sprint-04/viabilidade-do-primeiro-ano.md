# 13 · A dificuldade do primeiro ano

Este documento existe porque duas premissas da primeira versão da Sprint 4 não se sustentaram sob questionamento do grupo. Ele revisa o que estava errado, refaz as contas e reposiciona o primeiro ano como a fase mais difícil do negócio — que é o que ele de fato é.

## O que estava errado

### 1. O "100 alunos por turma" nunca foi validado

A premissa P5 estava registrada como "Padrão FDC · Validada". Não é.

O número tem uma única origem no repositório: o bloco **"Exemplo ilustrativo"** de [atores-e-financeiro.md](../sprint-03/banca-de-modelagem/atores-e-financeiro.md), da Banca de Modelagem. Era um número redondo escolhido para ilustrar uma conta, e foi promovido a fato validado sem que ninguém tivesse confirmado o tamanho real de uma turma executiva da FDC.

O erro importa mais do que parece, e a seção sobre tarifa de grupo abaixo mostra por quê.

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
| 1 | R$ 248 mil | Abaixo de R$ 250 mil — sem convênio | 3% |
| 2 | R$ 1,26 mi | Acima de R$ 1 mi — 8% a 12% | 5% |
| 3 | R$ 3,44 mi | Acima de R$ 1 mi — 8% a 12% | 6,4% |

O ano 1 fica logo abaixo do piso, o que confirma a fase de apoio na consolidadora. Os anos 2 e 3 usam comissões **abaixo** do que o volume permitiria — a projeção é conservadora de propósito, porque conquistar a faixa cheia leva tempo além de volume.

## O problema que ninguém tinha visto: uma turma isolada não forma grupo

Tarifa de grupo exige em torno de **10 passageiros na mesma rota e no mesmo voo**. As 5 condições obrigatórias mapeadas com a Velt já diziam "rota concentrada, 5 a 8 origens por turma". Faltou fazer a divisão.

Quantos passageiros por rota uma turma isolada produz:

| Turma | Adesão | 5 origens | 8 origens |
|---|---|---|---|
| 40 | 30% | 2,4 | 1,5 |
| 40 | 60% | 4,8 | 3,0 |
| 100 | 30% | 6,0 | 3,8 |
| 100 | 60% | **12,0** | 7,5 |

**Só uma configuração forma grupo: turma de 100 com 60% de adesão e apenas 5 origens.** É exatamente onde a Banca de Modelagem estava — o modelo funcionava porque pousou na única célula favorável da tabela, com um número de alunos que nunca foi verificado.

Tamanho de turma necessário para que uma turma isolada forme grupo sozinha:

| Adesão | 5 origens | 6 origens | 8 origens |
|---|---|---|---|
| 30% | 167 | 200 | 267 |
| 45% | 111 | 133 | 178 |
| 60% | 83 | 100 | 133 |
| 70% | 71 | 86 | 114 |

### O que isso muda no desenho do negócio

A unidade de negociação **não pode ser a turma**. Precisa ser o **campus numa data**: várias turmas que chegam ao mesmo lugar no mesmo dia, somadas.

Quantas turmas precisam coincidir em campus e data:

| Turma | Adesão | 5 origens | 8 origens |
|---|---|---|---|
| 40 | 30% | 5 | 7 |
| 40 | 60% | 3 | 4 |
| 60 | 60% | 2 | 3 |
| 100 | 60% | 1 | 2 |

Consequências diretas:

1. **A venda muda de alvo.** Não adianta uma turma numa escola. É preciso concentração — várias turmas do mesmo campus, com calendários que se sobrepõem.
2. **O bloqueio é da Antévia, não da escola.** Se o volume vem de somar turmas, quem agrega é a plataforma. Isso fortalece o negócio: o ativo passa a ser nosso, não emprestado.
3. **Existe um limiar de operação.** Abaixo de 3 a 5 turmas simultâneas no mesmo campus, a alavanca de grupo simplesmente não liga.

## O primeiro ano, refeito

Premissas revistas: **turma de 40 alunos** (a validar, ver abaixo), adesão de **30%** no ano 1 — piloto sem prova social, com o aluno decidindo módulo a módulo —, **1 a 2 instituições** e 4 turmas ativas ao fim do ano.

| | Ano 1 | Ano 2 | Ano 3 | Total |
|---|---:|---:|---:|---:|
| Receita (tendencial) | **R$ 34.042** | R$ 221.616 | R$ 703.572 | **R$ 959.230** |
| Viagens | 216 | 1.166 | 3.370 | 4.752 |

Comparação com a primeira versão da Sprint 4:

| | Antes | Agora | Variação |
|---|---:|---:|---:|
| Receita do ano 1 | R$ 293.155 | R$ 34.042 | **−88%** |
| Receita em 3 anos | R$ 4.577.731 | R$ 959.230 | **−79%** |
| Aderentes no T12 | 2.520 | 576 | −77% |
| Fatia do SAM no T12 | 24,0% | 5,5% | — |

Os 24% do SAM em três anos eram um número que não se defendia. Os 5,5% se defendem.

### O que o ano 1 significa na prática

**R$ 34 mil de receita não pagam ninguém.** É menos de R$ 3 mil por mês. O ano 1 não comporta equipe contratada, escritório ou investimento em tecnologia relevante — ou os sócios operam a coisa com as próprias mãos, ou é preciso capital para atravessar.

Isso não é defeito da projeção. É a descrição correta de um negócio que precisa de volume para ter margem e não tem volume no começo. A Sprint 5 vai dimensionar quanto custa atravessar esse período, e a Sprint 6 vai dizer quanto capital isso exige.

### O ano 1 não é sobre receita

Se o ano 1 rende R$ 34 mil, ele não pode ser medido por receita. Ele existe para produzir três ativos que destravam a fase 2:

| Ativo | Para que serve |
|---|---|
| Prova de execução | Um ciclo completo entregue permite subir a adesão de 30% para 45% |
| Volume acumulado | Cruzar R$ 1 mi/ano em aéreo abre a faixa de 8–12% |
| Concentração de campus | Chegar a 3–5 turmas simultâneas liga a alavanca de grupo |

A métrica do ano 1 é **turmas simultâneas no mesmo campus**, não faturamento.

## O que ainda precisa ser validado, em ordem

| # | Premissa | Valor usado | Impacto | Como validar |
|---|---|---|---|---|
| 1 | **Tamanho da turma** | 40 (a validar) | Define se a alavanca de grupo é viável | Secretaria FDC — é uma pergunta de dois minutos |
| 2 | Turmas simultâneas por campus e data | 3–5 necessárias | Define quando a fase 2 começa | Calendário acadêmico do campus |
| 3 | Adesão no ano 1 sem prova social | 30% | Define a receita do piloto | Aluno-executivo viajante (H6) |
| 4 | Desconto real da antecipação aos 90 dias | 13% no aéreo | É a única alavanca do ano 1 | Cotação com consolidadora |
| 5 | Repasse da consolidadora ao parceiro | 3% | É a receita variável do ano 1 | Conversa com a Velt |

A primeira é a mais barata de resolver e a que mais muda o modelo. O grupo tem alunos da FDC: basta perguntar à secretaria quantos alunos tem uma turma do programa executivo. Se a resposta for 100 e não 40, a alavanca de grupo passa a funcionar com uma turma isolada, e boa parte da dificuldade descrita aqui diminui.
