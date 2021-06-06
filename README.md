
<p align="center">
  <img src="https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/image2.png" />
</p>

# **INTRODUÇÃO**

Neste projeto estou aplicando os conhecimentos obtidos  nos módulos 1 e 2 do Bootcamp de Data Science Aplicada da Alura, analisando os dados do [Programa Nacional de Imunizações](http://tabnet.datasus.gov.br/cgi/tabcgi.exe?pni/cnv/cpniuf.def). As análises realizadas aqui envolvem a cobertura vacinal das vacinas incluídas nos calendários de vacinação do SUS (Sistema Único de Saúde). Além disso, foi feita uma análise mais profunda em relação à vacinação contra o HPV (*Human papillomavirus* - Papilomavírus Humano). 

O Notebook com a análise completa e código pode ser encontrado aqui. 

Um PDF sumarizando as análises, sem conter os códigos e etapas de tratamento dos dados, pode ser encontrado aqui.

![Alt Text](https://media.giphy.com/media/ZyuSUCXjt3E0T6Vwb2/giphy.gif)

## O que é o Programa Nacional de Imunizações?
O Programa Nacional de Imunizações (PNI) envolve a distribuição anual de mais de 300 milhões de doses de vacinas, soros e imunoglobulinas. Esse programa é extremamente importante, pois contribuiu, por exemplo, com a erradicação da varíola e da poliomielite, além da redução dos casos e mortes derivadas do sarampo, da rubéola, do tétano, da difteria e da coqueluche.

O PNI define os calendários de vacinação considerando a situação epidemiológica, o risco, a vulnerabilidade e as especificidades sociais. O programa sempre segue com orientações específicas para crianças, adolescentes, adultos, gestantes, idosos e povos indígenas. E, para que o programa continue representando um sucesso na saúde pública, cada vez mais esforços devem ser despendidos. Todas as doenças prevenidas pelas vacinas que constam no calendário de vacinação, se não forem alvo de ações prioritárias, podem voltar a se tornar recorrentes. E atualmente, temos outro problema: narrativas falsas e sem nenhuma comprovação científica, têm se disseminado pelas redes sociais, dando sustentação ao discurso do movimento antivacina.

## O que é cobertura vacinal? 
A cobertura vacinal é o número de doses aplicadas (correspondente ao esquema completo de vacinação) de determinado imunobiológico dividido pela população alvo e multiplicado por 100, em uma área e tempo considerados. Este indicador corresponde ao percentual de pessoas vacinadas e potencialmente protegidas contra determinada doença.

## O que é HPV?
O papilomavírus humano, conhecido como HPV, é um vírus que se instala na pele ou em mucosas. Sua ação pode provocar infecções e o câncer de colo do útero. 

![Alt Text](https://media.giphy.com/media/BXOEmFSzNkOObZhIA3/giphy.gif)


- Há mais de 100 diferentes tipos de HPV. Alguns tipos de HPV podem provocar câncer e outros podem causar verrugas genitais.
- Existem 12 tipos identificados como de alto risco (HPV tipos 16, 18, 31, 33, 35, 39, 45, 51, 52, 56, 58 e 59) que têm probabilidade maior de persistir e estar associados a lesões pré- cancerígenas. 
- O HPV de tipos 16 e 18 causam a maioria dos casos de câncer de colo do útero em todo o mundo (cerca de 70%). 
- O câncer de colo do útero é uma doença grave que pode levar ao óbito. No Brasil, é a quarta maior causa de morte entre as mulheres. 
- Em 2019, ocorreram 6.596 óbitos por esta neoplasia, representando uma taxa ajustada de mortalidade por este câncer de 5.33/100 mil mulheres.

### Transmissão do HPV:
- A transmissão do vírus ocorre por contato direto com a pele ou mucosa infectada.
- A principal forma de transmissão é pela via sexual, que inclui contato oral-genital, genital-genital ou mesmo manual-genital. Portanto, o contágio com o HPV pode ocorrer mesmo na ausência de penetração vaginal ou anal.
- Também pode ocorrer transmissão durante o parto.
- Não está comprovada a possibilidade de contaminação por meio de objetos, do uso de vaso sanitário e piscina ou pelo compartilhamento de toalhas e roupas íntimas.


### Vacinação contra o HPV:
A vacina HPV quadrivalente confere proteção contra HPV 6, 11, 16 e 18, ou seja, abrange os dois principais tipos responsáveis pelo câncer de colo do útero. Com isso, a fim reforçar as atuais ações de prevenção do câncer de colo do útero, o Ministério da Saúde, com as Secretarias Estaduais e Municipais de Saúde, dá continuidade à estratégia de vacinação contra o HPV. 

Essa vacina foi incluída no Calendário Nacional de Vacinação do SUS em março de 2014, tendo como população-alvo as meninas de 11 a 13 anos de idade. Em 2015, a oferta da vacina foi ampliada para as meninas na faixa etária de 9 a 13 anos de idade.

O Ministério da Saúde adotava o esquema vacinal estendido, composto por três doses (0, 6 e 60 meses), entretanto, para meninas de 9 a 13 anos, o esquema vacinal mudou para duas doses (0 e 6 meses). A mudança se deu com base em estudos que comprovaram a efetividade da imunização em duas doses em meninas nessa faixa etária. Para as demais faixas etárias devem ser aplicadas as três doses. A vacinação poderá ocorrer nas Unidades de Saúde do SUS e em parceria com as Secretarias de Saúde e Educação.

De acordo com o registro na Anvisa, a vacina quadrivalente é aprovada para mulheres entre 9 a 45 anos e homens entre 9 e 26 anos, e a vacina bivalente para mulheres entre 10 e 25 anos. No momento, as clínicas não estão autorizadas a aplicar as vacinas em faixas etárias diferentes às estabelecidas pela Anvisa.

Ambas as vacinas possuem maior indicação para meninas e meninos que ainda não iniciaram a vida sexual, uma vez que apresentam maior eficácia na proteção de indivíduos não expostos aos tipos virais presentes nas vacinas.

A vacina para o sexo masculino é importante para oferecer proteção contra as verrugas genitais, associadas à infecção pelos tipos 6 e 11 do HPV, que, além dos prejuízos estéticos e do desconforto, podem aumentar o risco de transmissão de HIV. Além disso, uma vez vacinado, o homem terá menos chances de transmitir o vírus para a mulher, ampliando a eficácia geral da vacina. No entanto, a vacina ainda é pouco difundida entre os homens.

![Alt Text](https://media.giphy.com/media/BY8ORoRpnJDXeBNwxg/giphy.gif) 

