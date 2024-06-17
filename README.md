# Projeto de recuperação de dívidas.

Temos 203 características, sendo em sua maioria mascaradas. Neste projeto realizei uma análise exploratória dos gráficos, plotando o histograma de todas as variáveis para analisar suas distribuições. Realizei tratamento para os dados nulos tanto para características que haviam muitos dados faltantes (acima de 10% do total foram removidos). Percebi que a variável alvo estava desbalanceada, por isso realizei um undersampling, já que técnicas como SMOTE ou oversampling não são tão interessantes por criar dados artificiais. Realizei o teste de diversos algoritmos de aprendizagem de máquina, e obtive como melhor resultado um classificador Stacking que combina 3 dos algoritmos utilizados. 
Sendo este resultado:

Bom pagador classificado como bom (55,9%)

Mau pagador classificado como bom (39,7%)

# Conclusões

### Análise técnica do modelo: Após realizar um pré-processamento de dados para lidar com dados nulos e features desbalanceadas, treinar diversos modelos de aprendizagem de máquina, notamos que nosso melhor modelo é o StackingClassifier. Acredito que a performance poderia ser melhorada significativamente com uma melhor qualidade dos dados, ou uma quantidade maior de dados sobre a classe alvo 1: Bom pagador, pois ao fazer os tratamentos necessários, há uma redução grande na quantidade de dados. O Stacking combina diversos modelos de treinamento, aproveitando o melhor de cada modelo, reduzindo também o risco de overfitting. 

### Análise de negócio: Esses modelos tem um impacto muito grande no negócio. Podendo reduzir o risco de oferecer crédito a mau pagadores, e também aumentando a oferta de crédito a pessoas com bom histórico de pagamento. Conseguir identificar quem são essas pessoas é essencial para estar bem posicionado no mercado e poder aumentar a receita. Ao saber quem são os bons pagadores, podemos ofertar melhores condições para o pagamento de suas dívidas, assim diminuindo possíveis perdas e recuperando o dinheiro de empréstimos condecidos. O cliente bom pagador também percebe o impacto positivo, se sentirá recompensado, sabendo que é um bom pagador e terá sua oportunidade de pagar suas dívidas com ofertas especiais, podendo até pedir novas linhas de crédito no futuro.
