**Desenvolvimento de uma análise de contas a pagar – Aging list**

*“Aging list é um relatório sobre títulos a pagar e a receber em uma empresa, recebendo classificação em ordem cronológica. O termo em inglês pode ser traduzido como ‘lista de envelhecimento’, tendo suas informações apresentadas na forma de tabela, permitindo uma análise mais simples e rápida sobre o saldo financeiro.”*

>**Fonte:** https://blog.contaazul.com/o-que-e-aging-list-e-como-ele-ajuda-a-receber-mais-rapido

Nessa análise será estudado as despesas do Senado Federal como exemplo, sendo que iremos utilizar como *dataset* as [Despesas do Senado Federal](http://www.senado.leg.br/transparencia/gestgov/recdesp/despesas/pesquisadespesas.asp) em sua fase de [Liquidação]([https://www.licitacao.online/pagamentos/liquidacao) referente ao ano de 2017, isso respeitando e se beneficiando da [Lei de Acesso à Informação](http://www.planalto.gov.br/ccivil_03/_ato2011-2014/2011/Lei/L12527.htm) para o desenvolvimento dessa análise.

**Aging List Contas a Pagar**

Nesse exemplo existe a necessidade de fazer uma melhor gestão de todas as despesas que devem ser pagas nos próximos 360 dias ou mais, considerando como data de referência da despesa será utilizada a data de **liquidação** e como data base para o estudo como sendo 01/01/2017.
 
  >**Observação:** Sabemos que a despesa com o *status* de liquidação consiste na apuração da obrigação reconhecida pelo Senado Federal em pagar todos seus fornecedores, e não o pagamento efetivo, mas nessa análise utilizaremos esses dados com o intuito de fazer a gestão de todas as despesas reconhecidas, considerando que todas as despesas do ano tenham sido disponibilizadas no primeiro dia de 2017.

Para isso será criado faixas de 30 em 30 dias até as liquidações com menos de 180 dias, a partir daí será de 60 em 60 até o limite definido, ficando assim:

|**Faixas**|
|--|
|Liquidações até 30 dias
|Liquidações entre 31 e 60 dias
|Liquidações entre 61 e 90 dias
|Liquidações entre 91 e 120 dias
|Liquidações entre 121 e 150 dias
|Liquidações entre 151 e 180 dias
|Liquidações entre 181 e 240 dias
|Liquidações entre 241 e 300 dias
|Liquidações entre 301 e 360 dias
|Liquidações maiores que 360 dias

A decorrência dessa análise terá como resultado as faixas definidas anteriormente, como também a quantidade de despesas do período dentro da faixa definida e o montante necessário para pagamento desses compromissos.

**Despesas do Senado Federal em 2017**

![](print 1)

**Resultado do Aging list**

![](print 2)

>**Observação:** Todos esses passos efetuados aqui, podem ser aplicados tanto num contas a pagar como também em um contas a receber. Esse tipo de análise é bastante simples de aplicar no dia a dia da empresa, mas muito efetiva porquê da uma visão geral e clara de toda a parte financeira.
