# IDEB

# Sobre
A base estudada está relacionada a um dos principais exames nacional feitos dentro do Brasil, o IDEB (Índice de Desenvolvimento da Educação do Básica) é um indicador criado pelo governo federal para medir e obsrvar a qualidade do ensino público, federal, estadual e partícular. Basicamente a nota desse indicador vária entre 0 e 10 e tem como base o Fluxo de Aluno (taxade aprovação) e a Aprovação (São os resultado do Saeb e Aneb que são as notas das redes públicas e partículares).
A partir disso, foi estímulado a entender como as notas de cada sertor de ensino se comportava ao longo do tempo e se era possível uma conclusão a partir dos gráficos obtidos.

# Objetivo
O objetivo desse estudo é a criação de um EDA (Exploratory Data Analysis) onde será feito a exploração dos dados para obter conhecimento sobre os dataset utilizando gráficos de linhas, boxplots e utilizando técnicas de estatística inferencial como a utilização de testes de hipóteses.

# Ferramentas
## Python
Manipulação dos dados: Pandas

Gráficos: Seaborn, Matplotlib, Plotly.express
## Base de dados
Base de dados públicos retirado denro do site Basededados.org

link: https://basedosdados.org/dataset/96eab476-5d30-459b-82be-f888d4d0d6b9?table=bc84dea9-1126-4423-86d2-8835e6b19a72


# Resultados
<div align="center">
<img src="https://github.com/renanwta/IDEB/assets/161327900/7b90c3aa-9bdd-4830-b5cf-4509ad09df55" width="1000px" />
</div>

A partir dos resultados é possível observar que durantes os anos houve um aprimoramento nos ensinos públicos, estaduais e federais, porém ainda infeiror a nota 6, já as rede de escolas privadas sempre manteve próximo da nota 6 desde o ínicio, porém não teve uma melhoria igual as das outras sedes.

# Step by step
1. Importação dos dados

   -> Obs: os dados que foi importando no Collab vem direto do meu Drive, portanto para rodar em outra máquina é importante baixar os dados, inserir no collab e em seguinda mudar o caminho do 'pd_read'
   
3. Conhecendo os dados

   Para conhecer os dados foi utlizando .info para observar a natureza dos dados e se há algum tipo dados nulos, além disso, foi utilizado um laço para ler cada coluna em seguida usado .unique para observar cada valor presente em cada coluna, isso, para obervar os valores nulos e como são separados os valores de cada coluna.
   
5. Validação dos dados

   A validação dos dados foi feito utilizando o boxplot para cada setor em relação a nota de IDEB e as notas de matéria base como língua portuguesa e matemática
   
6. Análisando as notas dos IDEB para cada rede de escola por ano

   Para fazer a análise temporal das notas IDEB em relação as redes, foi feita utilizando gráfico de linhas, assim foi utilziado a biblioteca matplotlib e seaborn, nela foi feita por 2 métodos, a primeira vez foi feita criando o data set para cada tipo de rede e em seguida criando o gráfico separadamente, o segundo método foi utilizando o laço for e em seguida criando gráficos para cada tipo de rede para que possamos comprar os gráficos de forma mais fácil.
   Assim o segundo método consistiu a criação de um um dicionário para cada rede e em seguida um laço duplo para a criação de gráficos para cada parte da matriz de 2x2 e por fim um laço duplo para facilitar a edição de colocar linhas pontilhadas e os valores do eixos X
   
7. Teste de hipóteses
   Para ter maior garantia que as notas da Rede Privada é maior que a das demais redes foi feita um teste de hipóteses para se confirmar.
   Assim a partir de testes paramétricos para duas população chegamos no resultado que a rede privada possui a sua média de notas maiores que as demais redes com 95% de certeza

8. Conclusão
 


