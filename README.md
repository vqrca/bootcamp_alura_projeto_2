[![Badge](https://img.shields.io/badge/Author-Valquíria_Alencar-%237159c1?style=flat-square&logo=ghost)](https://github.com/vqrca/)
[![Gmail Badge](https://img.shields.io/badge/-valquiria.c.alencar@gmail.com-6633cc?style=flat-square&logo=Gmail&logoColor=white&link=mailto:valquiria.c.alencar@gmail.com)](mailto:valquiria.c.alencar@gmail.com)
[![Linkedin Badge](https://img.shields.io/badge/-Valquíria_Alencar-6633cc?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/valquiria-alencar/)](https://www.linkedin.com/in/valquiria-alencar/) 

<p align="center">
  <img src="https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/cover_hpv.png" />
</p>

<h4 align="center"> 
	🚀 Em construção...
</h4>

Tabela de conteúdo
=================
<!--ts-->
   * [Introdução](#intro)
   * [Objetivos](#obj)
   * [Métodos](#met)
   * [Conclusões](#conclusoes)
   * [Considerações finais](#final)
   * [Referências](#ref)
   * [Documentação](#doc)
   * [Agradecimentos](#agra)
   <!--te-->

<a name="intro"></a>
# **Introdução**

Neste projeto estou aplicando os conhecimentos obtidos  nos módulos 1 e 2 do Bootcamp de Data Science Aplicada da Alura, analisando os dados do [Programa Nacional de Imunizações](http://tabnet.datasus.gov.br/cgi/tabcgi.exe?pni/cnv/cpniuf.def). As análises realizadas aqui envolvem a cobertura vacinal das vacinas incluídas nos calendários de vacinação do SUS (Sistema Único de Saúde). Além disso, foi feita uma análise mais profunda em relação à vacinação contra o HPV (*Human papillomavirus* - Papilomavírus Humano).

O Notebook com a análise completa e código pode ser encontrado aqui. 

Um PDF sumarizando as análises, sem conter os códigos e etapas de tratamento dos dados, pode ser encontrado aqui.

<p align="center"><img src="https://media.giphy.com/media/wKnx6Tas1aSTJES3O0/giphy.gif"</p>

## O que é o Programa Nacional de Imunizações?
O Programa Nacional de Imunizações (PNI) envolve a distribuição anual de mais de 300 milhões de doses de vacinas, soros e imunoglobulinas. Esse programa é extremamente importante, pois contribuiu, por exemplo, com a erradicação da varíola e da poliomielite, além da redução dos casos e mortes derivadas do sarampo, da rubéola, do tétano, da difteria e da coqueluche.

O PNI define os calendários de vacinação considerando a situação epidemiológica, o risco, a vulnerabilidade e as especificidades sociais. O programa sempre segue com orientações específicas para crianças, adolescentes, adultos, gestantes, idosos e povos indígenas. E, para que o programa continue representando um sucesso na saúde pública, cada vez mais esforços devem ser despendidos. Todas as doenças prevenidas pelas vacinas que constam no calendário de vacinação, se não forem alvo de ações prioritárias, podem voltar a se tornar recorrentes. E atualmente, temos outro problema: narrativas falsas e sem nenhuma comprovação científica, têm se disseminado pelas redes sociais, dando sustentação ao discurso do movimento antivacina.

## O que é cobertura vacinal? 
A cobertura vacinal é o número de doses aplicadas (correspondente ao esquema completo de vacinação) de determinado imunobiológico dividido pela população alvo e multiplicado por 100, em uma área e tempo considerados. Este indicador corresponde ao percentual de pessoas vacinadas e potencialmente protegidas contra determinada doença.

## O que é HPV?
O papilomavírus humano, conhecido como HPV, é um vírus que se instala na pele ou em mucosas. Sua ação pode provocar infecções e o câncer de colo do útero. 

<p align="center"><img src="https://media.giphy.com/media/BXOEmFSzNkOObZhIA3/giphy.gif"</p>	

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
A vacina HPV quadrivalente proporciona proteção contra HPV 6, 11, 16 e 18, então, abrange os dois principais tipos responsáveis pelo câncer de colo do útero. Com isso, a fim reforçar as atuais ações de prevenção do câncer de colo do útero, o Ministério da Saúde, com as Secretarias Estaduais e Municipais de Saúde, dá continuidade à estratégia de vacinação contra o HPV. 

Essa vacina foi incluída no Calendário Nacional de Vacinação do SUS em março de 2014, tendo como população-alvo as meninas de 11 a 13 anos de idade. No entanto, em 2015, a oferta da vacina foi ampliada para as meninas na faixa etária de 9 a 13 anos de idade.

O Ministério da Saúde adotava o esquema vacinal estendido, composto por três doses (0, 6 e 60 meses), entretanto, para meninas de 9 a 13 anos, o esquema vacinal mudou para duas doses (0 e 6 meses). A mudança se deu com base em estudos que comprovaram a efetividade da imunização em duas doses em meninas nessa faixa etária. Para as demais faixas etárias devem ser aplicadas as três doses. A vacinação poderá ocorrer nas Unidades de Saúde do SUS e em parceria com as Secretarias de Saúde e Educação.

É importante destacar que a vacina também é aplicada em indivíduos do sexo masculino e que essa vacina possui maior indicação para essa faixa etária (9-13 anos), pois considera que os individuos ainda não iniciaram a vida sexual, uma vez que a vacina apresenta maior eficácia na proteção de indivíduos não expostos aos tipos virais presentes nas vacinas.

A vacina para o sexo masculino é importante para oferecer proteção contra as verrugas genitais, associadas à infecção pelos tipos 6 e 11 do HPV, que, além dos prejuízos estéticos e do desconforto, podem aumentar o risco de transmissão de HIV. Além disso, uma vez vacinado, o homem terá menos chances de transmitir o vírus para a mulher, ampliando a eficácia geral da vacina. No entanto, a vacina ainda é pouco difundida entre os homens.

<p align="center"><img src="https://media.giphy.com/media/BY8ORoRpnJDXeBNwxg/giphy.gif"</p>

<a name="obj"></a>
# Objetivos

O projeto aqui apresentado teve por objetivo analisar a cobertura da vacinação nas Unidades da Federação por ano, no período disponibilizado pelo DATASUS (1994-2019) e verificar a cobertura dos imunos aplicados em cada uma das Unidades da Federação.
Além disso, como a vacinação contra HPV não está incluída nos dados de cobertura vacinal, outros datasets foram obtidos, como os seguintes objetivos:

- Verificar se houve aumento na aplicação de doses após o período que a vacina foi incluída no calendário de vacinação;
- Comparar a aplicação de doses nos sexos feminino e masculino e verificar se houve aumento de adesão no sexo masculino ao longo dos anos;
- Analisar o número de doses aplicadas por faixa etária; 
- Calcular a cobertura vacinal para o último ano disponível e verificar como essa cobertura está distribuída nas Unidades da Federação.


<p align="center"><img src="https://media.giphy.com/media/BpGWitbFZflfSUYuZ9/giphy.gif"</p>	

<a name="met"></a>
# Métodos

## Coleta dos dados:

Os dados utilizados neste projeto foram obtidos do [Tabnet - DATSUS](http://www2.datasus.gov.br/DATASUS/index.php?area=0202&id=11637), um banco de dados que disponibiliza dados relacionados à saúde. Entre os dados disponibilizados, podemos encontrar  Imunizações - desde 1994, na opção Assistência à saúde. Em imunizações há dados sobre cobertura vacinal, número de doses aplicadas e taxas de abandono.
Neste projeto os seguintes datasets foram obtidos:

### Coberturas Vacinais por Ano segundo Unidade da Federação
Aplicando os seguintes filtros:
- Linha: Ano
- Coluna: Unidade da Federação
- Conteúdo: Coberturas Vacinais
- Período disponível: 1994 - 2019

O arquivo *.csv* desse dataset pode ser encontrado [aqui](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/cobertura_vacinas_1994-2021_por_ano.csv)

### Coberturas Vacinais por Imuno segundo Unidade da Federação
Aplicando os seguintes filtros:
- Linha: Unidade da Federação
- Coluna: Imuno
- Conteúdo: Coberturas Vacinais
- Período disponível: 1994 - 2019

O arquivo *.csv* desse dataset pode ser encontrado [aqui](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/cobertura_vacinas_1994-2021_por_imuno.csv) 
 
### HPV - Doses aplicadas: Imunobiológicos: HPV Quadrivalente - Feminino/Masculino
Os datasets sobre HPV estavam disponibilizados apenas na opção [Doses aplicadas](http://tabnet.datasus.gov.br/cgi/dhdat.exe?bd_pni/dpnibr.def)

por ano:
- Linha: Unidade da Federação
- Coluna: Ano
- Conteúdo: Doses aplicadas 
- Período disponível:  2009-20219 (feminino), 2013-2019 (masculino)

Os arquivos *.csv* desse datasets podem ser encontrados aqui:

[Feminino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_ano_feminino.csv)

[Masculino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_ano_masculino.csv)

por faixa etária:
- Linha: Unidade da Federação
- Coluna: Faixa etária 
- Conteúdo: Doses aplicadas 
- Período disponível:  2009-20219 (feminino), 2013-2019 (masculino)

Os arquivos *.csv* desse datasets podem ser encontrados aqui:

[Feminino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_faixa_etaria_feminino.csv)

[Masculino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_faixa_etaria_feminino.csv) 

## Bibliotecas utilizadas 

- Pandas: para realizar a manipulação dos datasets

- Numpy: para realizar de cálculos numéricos 

- Matplotlib: para plotar os gráficos

- Seaborn: para plotar os gráficos

O notebook *.ipynb* foi construído no google colab usando Python 3.7.10. 

<a name="conclusoes"></a>
# Conclusões

....

<a name="final"></a>
# Considerações finais

...

<a name="ref"></a>
# Referências

[ Campanha - Programa Nacional de Imunizações](https://portalarquivos.saude.gov.br/campanhas/pni/o-que-e.html)

[Cobertura da Vacina Papilomavírus Humano (HPV) no Brasil: Heterogeneidade Espacial e entre Coortes Etárias](https://www.scielo.br/j/rbepid/a/TStbZmwdZTG3rmZZFsqvNFx/?lang=pt)

[Crescimento da Adesão de Público Masculino à Vacina Contra HPV](https://www.fleury.com.br/noticias/cresce-adesao-de-publico-masculino-a-vacina-contra-hpv)

[Desigualdades Sociais e Cobertura Vacinal: uso de inquéritos domiciliares](https://www.scielo.br/j/rbepid/a/7LVm96t5JssG46Bw5sRD74Q/?lang=pt&format=pdf)

[Fiocruz - Movimento Antivacina e Suas Ameaças](https://portal.fiocruz.br/video/movimento-antivacina-e-suas-ameacas-sala-de-convidados)

[Fiocruz - Com fake news, discurso antivacina se espalha nas redes](https://portal.fiocruz.br/noticia/com-fake-news-discurso-antivacina-se-espalha-nas-redes)

[Informe Técnico Sobre a Vacina Papilomavírus Humano (HPV) na Atenção Básica](https://portalarquivos2.saude.gov.br/images/pdf/2015/junho/26/Informe-T--cnico-Introdu----o-vacina-HPV-18-2-2014.pdf) 

[Instituto Nacional De Câncer - Atlas da Mortalidade](https://mortalidade.inca.gov.br/MortalidadeWeb/) 

[Instituto Nacional do Câncer - Controle do Câncer de Colo do Útero](https://www.inca.gov.br/controle-do-cancer-do-colo-do-utero/conceito-e-magnitude)

[Instituto Nacional do Câncer - Para que Servem as Vacinas Contra o HPV?](https://www.inca.gov.br/perguntas-frequentes/para-que-servem-vacinas-contra-o-hpv)

[PNI- Programa Nacional de Imunizações, Boletim Informativo: Vacinação contra HPV](https://portalarquivos2.saude.gov.br/images/pdf/2017/julho/28/Boletim-informativo.pdf)

[Tabnet - DATASUS, Cobertura Vacinal](http://tabnet.datasus.gov.br/tabdata/livroidb/Com2007/Com_F13.pdf)

[Tabnet - DATASUS,  Imunizações: Cobertura -  Notas Técnicas](http://tabnet.datasus.gov.br/cgi/pni/%5Ccpnidescr.htm)
 
[World Health Organization -  International Agency for Research on Cancer](https://www.iarc.who.int/)

<a name="doc"></a>
# Documentação

- [Matplotlib](https://matplotlib.org/)
 
- [Numpy](https://numpy.org/)
	
- [Pandas](https://pandas.pydata.org/)
 
- [Seaborn](https://seaborn.pydata.org/)

<a name="agra"></a>
# Agradecimentos

Gostaria de deixar meu agradecimento aos instrutores do módulo 2: Thiago Gonçalves e Guilherme Silveira.
	
Ao pessoal do Scuba team e do Discord, que sempre trazem excelentes discussões e ideia

Também gostaria de agradecer ao Junior Torres e Carolina Dias, que sempre têm ideias inspiradoras, 
e me deram muitas dicas de como melhorar as visualizações gráficas.

<p align="center"><img src="https://media.giphy.com/media/M9NbzZjAcxq9jS9LZJ/giphy.gif"</p>




