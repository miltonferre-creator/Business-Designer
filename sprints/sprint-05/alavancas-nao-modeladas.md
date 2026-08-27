# 19 · Alavancas não modeladas

Duas ideias levantadas em reunião do grupo: **ganhar com a venda no cartão** e **comprar passagem com milhas**. Nenhuma das duas entra na projeção. Este documento registra por quê, o que cada uma vale de fato, e o que precisaria ser verdade para incluí-las.

O critério é o mesmo que aplicamos ao fee da escola desde a Sprint 4: **receita especulativa não entra em cenário.** Parcimônia é critério de avaliação, e inflar a projeção com premissas não validadas derruba a robustez de tudo o mais.

---

## 1 · Cartão: três coisas diferentes misturadas

### "Ganhar com a taxa do cartão" está invertido

Quem aceita cartão **paga** o MDR, não recebe. E há um risco escondido: hoje o aluno paga o fornecedor e nós intermediamos. Se o ticket inteiro passar a rodar no nosso CNPJ, herdamos o custo:

| Se o ticket transitasse na nossa maquininha | MDR por viagem |
|---|---:|
| Crédito à vista (~2,99%) | R$ 61 |
| Parcelado 6× (~4,49%) | R$ 92 |
| Parcelado 12× (~5,99%) | R$ 122 |

Contra uma receita de R$ 196,80 por viagem na fase 1. Aceitar o pagamento cheio consumiria de 31% a 62% da receita. **Não é receita nova — é custo novo**, e é exatamente o que a nossa estrutura de custos variáveis evita hoje ao cobrar MDR apenas sobre a taxa de serviço.

### Parcelado sem juros também é perda

Vender em 12× sem juros significa antecipar recebível e pagar por isso, ou esperar doze meses para receber.

### O ganho real seria ser o financiador

| Spread (cliente − funding) | Ganho por aluno no ciclo | vs. receita de taxa |
|---|---:|---:|
| +0,7 p.p./mês | R$ 806 | 56% |
| +1,5 p.p./mês | R$ 1.728 | 120% |
| 0 p.p. | R$ 0 | 0% |

Pode superar a fonte principal — o instinto do grupo está certo na magnitude. Mas isso é uma **operação de crédito**, não de concierge: exige capital, cria risco de inadimplência num nicho sem histórico de crédito, tem peso regulatório, e se um parceiro é quem funda a operação, é ele quem fica com a maior parte do spread.

### A versão forte: assinatura do programa

Não como receita lateral, mas como produto. **O aluno contrata na matrícula o pacote logístico dos 12 módulos e paga parcela mensal fixa.**

| | Valor |
|---|---:|
| Pacote do programa (fase 1) | 12 × R$ 2.040 = **R$ 24.480** |
| Parcela mensal ao longo dos 20 meses | **R$ 1.224** |

O que isso resolve, tudo de uma vez:

- Entrega **literalmente** a promessa "custo previsível desde a matrícula" — a hipótese H3 da Sprint 1
- Ataca a **dor nº 1 da hierarquia da Ana Paula, que é financeira**, não logística
- Trava o aluno pelos 20 meses e elimina o churn módulo a módulo
- **Garante a concentração que a tarifa de grupo exige** — sabemos com antecedência quem viaja, que é exatamente o gargalo do slide 4 da Sprint 4
- Justifica comprar aos 90 dias, porque o dinheiro já está comprometido

### E há um efeito sobre a necessidade de capital

Se o aluno paga mensalmente e nós pagamos o fornecedor a cada módulo, os dois fluxos quase se anulam — mas a defasagem gera caixa retido:

| Ano | Alunos médios | Arrecadação mensal | Float de 1 mês |
|---|---:|---:|---:|
| 1 | 62 | R$ 76.500 | R$ 76.500 |
| 2 | 208 | R$ 239.040 | R$ 239.040 |
| 3 | 495 | R$ 540.540 | R$ 540.540 |
| 4 | 970 | R$ 1.047.600 | **R$ 1.047.600** |
| 5 | 1.529 | R$ 1.623.532 | R$ 1.623.532 |

**No ano 4, que é o pico de exposição da Sprint 5, um mês de float equivale a 188% da necessidade de capital de R$ 559 mil.**

### Por que isso não entra na projeção — e não deveria

O número acima é sedutor e perigoso. **Esse dinheiro não é nosso.** É pagamento antecipado por uma viagem que ainda não entregamos, e portanto é passivo, não capital.

Usar prepagamento de cliente como capital de giro é exatamente o mecanismo que quebrou operadoras de turismo. Se a captação parar, o passivo continua e não há receita nova para honrá-lo.

A Velt já havia listado **garantia financeira** entre as cinco condições do bloqueio de grupo. Com assinatura, essa exigência deixa de ser condição de fornecedor e passa a ser obrigação com o próprio aluno.

**Encaminhamento:** a assinatura é a evolução mais promissora do modelo, e vale desenvolver — mas como produto que melhora retenção e concentração, não como fonte de financiamento. Se for adiante, o float precisa ficar segregado, com garantia, e nunca aparecer como redução do capital pedido.

### Um conflito de posicionamento a evitar

Toda a proposta de valor é "economizamos o seu dinheiro". Cobrar juros é ganhar com o problema de caixa do aluno — são coisas que brigam, e um avaliador atento pergunta.

A saída limpa: **parcelado sem juros para o aluno, financiado por parceiro, e a Antévia recebe comissão do parceiro.** Ganha-se menos que segurando o spread, mas não se vende contra o próprio discurso.

---

## 2 · Milhas: a conta é ótima, o gargalo é outro

| Resgate | Custo | vs. tarifa de R$ 1.400 |
|---|---:|---:|
| 20.000 milhas a R$ 20/mil + taxas | R$ 500 | −64% |
| 25.000 milhas a R$ 18/mil + taxas | R$ 550 | −61% |
| 30.000 milhas a R$ 22/mil + taxas | R$ 760 | −46% |

Economia muito maior que os 27% do bloqueio de grupo. O problema não é o preço da milha.

### O gargalo é disponibilidade em data fixa

Assento-prêmio é o ativo mais escasso do sistema, e a escassez se concentra exatamente onde precisamos: **sexta à noite e domingo à tarde, nas datas fixas dos módulos.** Toda a lógica da Antévia depende de datas que não podem mudar — é justamente a pior condição possível para depender de resgate.

E a escala inviabiliza:

| Ano | Assentos-prêmio necessários em datas fixas |
|---|---:|
| 1 | 450 |
| 3 | 3.564 |
| 5 | 11.007 |

Some-se a isso que compra de milhas em volume costuma violar os termos dos programas de fidelidade e leva ao bloqueio de contas.

### Duas versões legítimas

**As milhas do próprio aluno.** A persona Ricardo diz explicitamente que quer manter as milhas dele. Ajudá-lo a usar ou acumular reforça o posicionamento, não exige estoque nenhum e a receita continua sendo serviço, não arbitragem. **É a versão que recomendamos desenvolver.**

**Canal oportunista.** Parceria com marketplace de milhas para rotas e datas onde houver disponibilidade, como complemento de uma minoria das emissões — nunca como base de suprimento.

---

## Resumo do encaminhamento

| Ideia | Entra na projeção? | O que fazer |
|---|---|---|
| Ganhar com a taxa do cartão | Não | Descartar — é custo, não receita |
| Financiar o parcelamento (spread) | Não | Só com parceiro, e sem cobrar juros do aluno |
| **Assinatura do programa** | **Não** | **Desenvolver como produto na Sprint 6 — resolve retenção e concentração** |
| Float como capital de giro | **Não** | Nunca abater da necessidade de capital. É passivo |
| Milhas como base de suprimento | Não | Inviável em datas fixas e em escala |
| Milhas do próprio aluno | Não | Desenvolver como funcionalidade — reforça o posicionamento |

Nenhuma dessas alavancas altera um único número da Sprint 5. Todas ficam registradas para a Sprint 6 e para o Demo Day, onde a pergunta "como esse negócio cresce depois do ano 5" tem que ter resposta.
