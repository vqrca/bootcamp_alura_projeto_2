[![Badge](https://img.shields.io/badge/Author-Valquíria_Alencar-%237159c1?style=flat-square&logo=ghost)](https://github.com/vqrca/)
[![Gmail Badge](https://img.shields.io/badge/-valquiria.c.alencar@gmail.com-6633cc?style=flat-square&logo=Gmail&logoColor=white&link=mailto:valquiria.c.alencar@gmail.com)](mailto:valquiria.c.alencar@gmail.com)
[![Linkedin Badge](https://img.shields.io/badge/-Valquíria_Alencar-6633cc?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/valquiria-alencar/)](https://www.linkedin.com/in/valquiria-alencar/) 

<p align="center">
  <img src="https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/cover_hpv.png" />
</p>


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

O Notebook com a análise completa e código pode ser encontrado [aqui](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Bootcamp_Projeto_2_Valquiria_Alencar.ipynb)
> Recomendo que seja aberto pelo colab para melhorar a visualização :wink:	

Um PDF sumarizando as análises, sem conter os códigos e etapas de tratamento dos dados, pode ser encontrado [aqui](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Resultados_Projeto_2_Valquiria.pdf)

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

O projeto aqui apresentado teve por objetivo analisar a cobertura da vacinação nas Unidades da Federação por ano, no período disponibilizado pelo DATASUS (1994-2019) e verificar a cobertura dos imunobiológicos aplicados em cada uma das Unidades da Federação.
Além disso, como a vacinação contra HPV não está incluída nos dados de cobertura vacinal, outros datasets foram obtidos, como os seguintes objetivos:

- Verificar se houve aumento na aplicação de doses após o período que a vacina foi incluída no calendário de vacinação;
- Comparar a aplicação de doses nos sexos feminino e masculino e verificar se houve aumento de adesão no sexo masculino ao longo do tempo;
- Analisar a proporcionalidade da vacinação de acordo com o número de habitantes e verificar se há consistência nessas proporções nas Unidades da Federação;
- Analisar o número de doses aplicadas por faixa etária

<p align="center"><img src="https://media.giphy.com/media/BpGWitbFZflfSUYuZ9/giphy.gif"</p>	

<a name="met"></a>
# Métodos

## Coleta dos dados:

Os dados utilizados neste projeto foram obtidos do [Tabnet - DATASUS](http://www2.datasus.gov.br/DATASUS/index.php?area=0202&id=11637), um banco de dados que disponibiliza dados relacionados à saúde. Entre os dados disponibilizados, podemos encontrar  Imunizações - desde 1994, na opção Assistência à saúde. Em imunizações há dados sobre cobertura vacinal, número de doses aplicadas e taxas de abandono.
Neste projeto os seguintes datasets foram obtidos:

### Coberturas Vacinais por Ano segundo Unidade da Federação
Aplicando os seguintes filtros:
- Linha: Unidade da Federação
- Coluna: Ano
- Conteúdo: Coberturas Vacinais
- Período disponível: 1994 - 2019

O arquivo *.csv* desse dataset pode ser encontrado [aqui](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/cobertura_vacinas_1994-2021_por_ano.csv)

### Coberturas Vacinais por Imunobiológico segundo Unidade da Federação
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
- Período disponível:  2009-2019 (feminino), 2013-2019 (masculino)

Os arquivos *.csv* desse datasets podem ser encontrados aqui:

[Feminino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_ano_feminino.csv)

[Masculino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_ano_masculino.csv)

por faixa etária:
- Linha: Unidade da Federação
- Coluna: Faixa etária 
- Conteúdo: Doses aplicadas 
- Período disponível:  2009-2019 (feminino), 2013-2019 (masculino)

Os arquivos *.csv* desse datasets podem ser encontrados aqui:

[Feminino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_faixa_etaria_feminino.csv)

[Masculino](https://github.com/vqrca/bootcamp_alura_projeto_2/blob/main/Dados/HPV_doses_faixa_etaria_feminino.csv) 

## Bibliotecas utilizadas 

- bs4: para extração de dados de arquivos HTML
	
- Pandas: para realizar a manipulação dos datasets

- Numpy: para realizar de cálculos numéricos 
	
- Matplotlib: para plotar os gráficos

- Requests: para extração de dados de arquivos HTML

- Seaborn: para plotar os gráficos

O notebook *.ipynb* foi construído no google colab usando Python 3.7.10. 

<a name="conclusoes"></a>
# Conclusões
## Parte I
- Como podemos observar, as coberturas vacinais estavam em torno de 40% no ano inicial (1994) e foram subindo gradativamente até 1999. **Entre  2000-2012 há uma estabilização e as médias das coberturas vacinais ficam próximas de 80%**. Após 2012 vemos um aumento na cobertura (com valores médios acima de 80%), porém, há uma **queda em 2016 para uma cobertura média de 52.64%**. Os valores voltam a subir tendo uma média de 72.65% em 2018. 
 
- Esse tipo de informação é preocupante, pois **baixas coberturas** alcançadas para as principais vacinas do Calendário Nacional de Vacinação representam uma **ameaça real de retorno de doenças comuns no passado**, como o sarampo e a poliomielite (paralisia infantil).
 
- Inclusive, **em 2018 tivemos o retorno do Sarampo**, com o registro de 10.274 casos no País. O País enfrentou dois surtos da doença: no Amazonas e em Roraima. Além disso, casos isolados foram notificados em outros Estados. E nós, claramente, tivemos esses casos de sarampo no Brasil porque não tínhamos cobertura de vacinação adequada. 
 
- Em relação à **Febre Amarela**, a **cobertura vacinal só é alta na Região Norte, na Região Nordeste no Maranhão, Bahia e na Região Centro-Oeste, em todos os Estados exceto no Distrito Federal**.
 
  Considerando essas recomendações do Ministério da saúde, por serem áreas endêmicas, **A cobertura não é ideal no Espírito Santo e no Distrito Federal, onde as coberturas não chegam a 50%.**

- No caso do **Sarampo**, a situação é preocupante no **Distrito Federal**, que teve **cobertura vacinal de 5.74%**. 
 
- **São Paulo, Ceará e Pernambuco são os Estados com maior cobertura vacinal contra o sarampo, chegando perto de 100%.**
Na **Vacinação contra Poliomelite (4 anos)**, as **coberturas vacinais são péssimas em grande parte do País**, com **cobertura mínima de 27.98% e cobertura média de 60.37%**. Os **piores cenários são vistos em Amapá, Pará, Maranhão, Acre, Bahia e Rio Grande do Norte, onde a vacinação não chega nem a 50% de cobertura.** 
 
- A **Tetra Viral (SRC + VZ: contra sarampo, caxumba, rubéola e varicela) não alcançou ao menos 80% de cobertura vacinal em nenhuma das Unidades da Federação**. Os melhores valores de cobertura se concentram nas Regiões Sul e Centro-Oeste e na  Região Norte nos Estados: Rondônia, Roraima, Tocantins, Amazonas e Amapá.
 
- Quando analisamos os valores de média vemos que os Imunobiológicos com maiores % de cobertura vacinal são:

  BCG

  Tríplice Viral D1

  Poliomielite

  DTP
 
- Quando analisamos os valores de média vemos que os Imunobiológicos com % de Cobertura vacinal abaixo de 50% são:

  Febre Amarela

  Dupla adulto e tríplice acelular gestante

  dTpa gestante

  DTP REF (4 e 6 anos)

  Haemophilus influenzae b
 
- A **vacina BCG**, que previne a tuberculose, apresenta a maior cobertura vacinal, que é ótima em todas as Unidades da Federação. 
Dados apresentados pelo [Ministério da Saúde](https://agenciabrasil.ebc.com.br/saude/noticia/2019-09/bcg-e-unica-vacina-atingir-meta-de-imunizacao-desde-2017)  mostram que a BCG **foi a única vacina a alcançar a cobertura vacinal pretendida nos anos de 2017 e 2018**. 
 
- Em segundo lugar temos a **vacina contra poliomielite**, **porém a cobertura não chega a 100% em todos os Estados**. A maioria dos Estados da Região Norte (exceto Tocantins) não atinge os 100% de cobertura e alguns Estados do Nordeste se encontram em uma situação similar: Maranhão, Piauí, Ceará, Alagoas e Bahia.
 
- Enquanto isso, a vacina **Tríplice viral apresenta ótima cobertura na primeira dose, mas quando olhamos a segunda dose vemos que o cenário muda completamente**, principalmente na região Norte, onde a melhor cobertura é em Rondônia com 82.36%. No Acre, por exemplo, a cobertura cai para 54.31%.
 
- A queda da cobertura vacinal pode estar relacionada com a hesitação à vacinação, definida como atraso na aceitação ou recusa das vacinas recomendadas, apesar da sua disponibilidade nos serviços de saúde.Os  **principais motivos da hesitação à vacinação são falta de confiança quanto à eficácia/segurança da vacina e preocupações com eventos adversos**. 
 

 ## Parte II
- O **papilomavírus humano** (HPV) é **uma das infecções sexualmente transmissíveis mais frequentes no mundo**. A persistência da infecção por alguns tipos de HPV pode evoluir para o **câncer do colo do útero**, doença que registra milhares de  novos casos por ano. **Uma das principais estratégias para prevenção desse tipo de câncer é a vacinação.**

- Quando analisamos a vacinação contra o HPV é possível observar que no caso da vacinação no **sexo feminino os valores mais altos de doses aplicadas se concentram no ano inicial da campanha de vacinação (2014)** e as **doses aplicadas foram caindo ao longo do tempo, apresentando uma queda abrupta em 2016**. Em 2017 houve um pequeno aumento, mas as doses voltaram novamente a cair. Enquanto isso, **no caso das doses aplicadas no sexo masculino, as doses parecem ter começado a ser aplicadas somente em 2017, porém em 2018 as doses começam a declinar**.
 
- **No período de 2014 a 2016 a vacinação estava ocorrendo de fato somente sexo feminino e que a vacinação era relacionada ao tamanho crescente da população**.
Portanto, **quanto maior o número de habitantes, maior o número de doses aplicadas,** exceto em poucos pontos que ficariam fora de uma reta, caso fosse inserida uma reta nesses gráficos. 
 
- **Em 2017, vemos que a vacinação estava ocorrendo nos sexos feminino e masculino, de forma proporcional à população**, porém nos **anos seguintes vemos que começa a ocorrer uma dispersão nos pontos, indicando que a aplicação de doses começou a não estar tão relacionada.** 
Ao analisar a proporcionalidade de doses aplicadas pela população, de cada Unidade da Federação, é possível observar que **em 2017 havia uma proporção mais homogênea.**
 
- **Em 2018 há uma série de discrepâncias, principalmente no sexo feminino, onde temos mais doses sendo aplicadas em Roraima, Amazonas e Paraná. Nos dados do sexo masculino há mais doses sendo aplicadas no Paraná, Roraima, Amazonas e Maranhão.**
 
- Essas **heterogeneidades na proporção** de doses aplicadas podem estar associadas a **políticas públicas estaduais distintas**, que **afetam a disponibilidade de vacinas para a população**. 
 
 
- A análise de doses aplicadas por faixas etárias mostra que a **vacinação foi maior na faixa etária de 9 e 11 anos no sexo femino**, e que **abrangeu a faixa etária entre 9-14 anos**.
 
 
- No caso do **sexo masculino a vacinação abrangeu a faixa etária entre 11-14 anos, porém foi maior aos 11 e 12 anos de idade.**
 
 
- As **doses acima de 14 anos**, provavelmente, estão relacionadas ao fato da **vacina ter sido disponibilizada para as mulheres e homens até 26 anos de idade** vivendo com HIV/AIDS, transplantados de órgãos sólidos, de medula óssea e pacientes oncológicos.
 
- A **discrepância entre vacinação nos sexos femino de masculino e a queda na aplicação de doses** mostra que a mídia social tem importante papel na disseminação das informações e é uma das maneiras de divulgar recomendações de saúde. Mas destaca-se que a **falta de informações e/ou as informações falsas sobre a vacina HPV ampliam a dificuldade de adesão à vacinação**.

- Apesar da distribuição gratuita da vacina contra HPV, os resultados mostrados neste projeto e em estudos anteriores indicam que existe uma dificuldade na adesão nessa campanha de vacinação, principalmente no sexo masculino. **Os resultados mostram que os  gestores estaduais precisam planejar estratégias específicas para cada território e tentar de alguma forma ampliar essa vacinação.** 

- A vacina mais utilizada atualmente é a quadrivalente, que hoje é recomendada para meninas e mulheres de nove a 45 anos e meninos e homens de nove a 26 anos de idade. Porém, **além das fake news, diversos fatores para baixa vacinação têm sido associados ao baixo nível educacional, baixa renda, residência em zona rural, baixo acesso à informação e aos serviços de saúde e barreiras interpostas por dogmas religiosos**.

- Apesar da queda na resposta imunológica com o passar dos anos, **adultos que não foram expostos ao vírus podem se vacinar**. Por esse motivo, o **Ministério da Saúde chegou a ofertar a vacina para adultos até os 26 anos.**
Para aqueles **acima dessa idade, é necessário se vacinar na rede privada**. Devido ao alto preço das doses na rede privada, a vacina se torna acessível apenas para uma pequena parcela da população brasileira. 
- **Em conclusão, seria pertinente ampliar a vacinação contra HPV para adultos, já que a maior parte da população não tem acesso à rede privada.**

<a name="final"></a>
# Considerações finais

O que pode explicar a diminuição na cobertura vacinal nos últimos anos?
Essa cobertura não é simplesmente um número. Sem cobertura vacinal, nós estamos suscetíveis a todas essas doenças.
Nós sabemos que nosso país oferece diversos imunobiológicos gratuitamente no calendário nacional e que essa distribuição abrange recém-nascidos, crianças, adolescentes, adultos, idosos e povos indígenas.
	
Minha opinião como Bióloga e Cientista é que a circulação crescente de notícias falsas sobre vacinas, que têm ocorrido nas redes sociais e aplicativos como WhatsApp, trouxe um enorme obscurantismo, que vem assolando nossa sociedade.
	
Mesmo com evidências científicas de que as vacinas são seguras, alguns pais e responsáveis simplesmente optam por não levarem seus filhos para serem vacinados. 
Essa questão se tornou ainda mais evidente desde 2020, com o surgimento da pandemia de SARS-CoV-2, onde ocorreu uma disseminação massiva de fake news, sobre medicações e vacinação. 

Entramos num momento extremamente crítico e preocupante, onde o próprio presidente do Brasil, faz propaganda contra a vacinação. 
		
<p align="center"><img src="https://media.giphy.com/media/2RrKN8LIzvluQXOffg/giphy.gif"</p>

É necessária uma comunicação efetiva dos órgãos de saúde com a população. Não podemos permitir que doenças que foram erradicadas anos atrás retornem.
	
**Todos precisam entender que Vacinas Salvam Vidas!** 


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

- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)

- [Matplotlib](https://matplotlib.org/)
 
- [Numpy](https://numpy.org/)
 
- [Pandas](https://pandas.pydata.org/)
 
- [Requests](https://docs.python-requests.org/en/master/)
 
- [Seaborn](https://seaborn.pydata.org/)


<a name="agra"></a>
# Agradecimentos

Gostaria de deixar meu agradecimento aos instrutores do módulo 2: Thiago Gonçalves e Guilherme Silveira.
	
Ao pessoal do Scuba team e do Discord, que sempre trazem excelentes discussões e ideias.

Também gostaria de agradecer ao Junior Torres e à Carolina Dias, que sempre têm ideias inspiradoras, 
e me deram muitas dicas de como melhorar as visualizações gráficas.

<p align="center"><img src="https://media.giphy.com/media/M9NbzZjAcxq9jS9LZJ/giphy.gif"</p>




