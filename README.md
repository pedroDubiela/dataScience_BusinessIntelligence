# Objetivo:
A partir de 5 bases de dados com informações sobre o cadastro dos clientes, o endereço das lojas, os produtos vendidos, as vendas e os status dos pagamentos, vamos responder as seguintes perguntas:
1) Quais lojas/produtos mais vendem e mais geram receitas em todo o período avaliado?
2) Quais as lojas e produtos mais importantes do ponto de vista econômico?
3) Qual o tempo médio para ocorrer o pagamento das vendas?
4) Existe algum padrão de vendas no tempo? Tendência, Sazonalidade?
5) Análise de Inadimplência.
6) Previsão de Inadimplência

# Descrição do banco de dados:
 A partir de 5 bases de dados, criou-se uma única, com os atributos:
1) Data da Venda;
2) Nome do Cliente;
3) Sexo do Cliente;
4) Data de Nascimento do Cliente;
5) Cidade da Loja;
6) Produto;
7) Valor do Produto;
8) Data do Pagamento.

# O que foi feito:
1) Limpeza dos dados;
2) Criação de novos atributos a partir dos existentes;
3) Aplicação de técnicas estatísticas;
4) Aplicação de modelos de Machine Learning.

# Resultados: As respostas das perguntas:
1) Quais lojas/produtos mais vendem e mais geram receitas em todo o período avaliado?
- Loja com maior número de vendas: Belo Horizonte.
- Loja com maior receita: Recife. 
- Produto mais vendido: Laptop Básico.
-  Produto que gera maior receita: Laptop Gamer.

2) Quais as lojas e produtos mais importantes do ponto de vista econômico?
- É nítido que praticamente 80% da receita é proveniente de somente dois produtos, o laptop gamer e o laptop básico.
- A contribuição para a receita é bem distribuída entre as cidades, não há uma disparidade significativa.

3) Qual o tempo médio para ocorrer o pagamento das vendas?
- Como vemos pelo teste de hipótese Shapiro, a distribuição do tempo de pagamento não é gaussiana, isso significa que a média do tempo de pagamento (23 dias) não é significativa, o que fica evidente quando se olha o histograma acima.

4) Existe algum padrão de vendas no tempo? Tendência, Sazonalidade?
- Vemos que o faturamento está seguindo uma tendência de queda a cada ano.
- Quanto a sazonalidade, está se manifesta a cada ano da seguinte forma:
- Começo e final de ano as vendas são aquecidas, provavelmente devido as datas festivas e férias.
- Por volta do mês 6-7 as vendas ganham força novamente, provavelmente devido as férias escolares, uma vez que os produtos que mais geram receitas são laptops (gamers e convencionais).

5) Análise de Inadimplência.
Vemos que:
- São Paulo ganha disparado como loja/cidade com mais inadimplência.
- A mesa ganha como produto com mais inadimplência.
- A idade em torno de 50 anos é a que mais gera inadimplência.

6) Previsão de Inadimplência.
Os dois melhores modelos de predição foram:
- Redes Neurais Artificiais.
- SVC (Suport Vector Machine).
- Ambos os modelos apresentaram capacidade de predizer a ocorrência de uma inadimplência com cerca de 85% de chances de acerto.

