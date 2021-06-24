# TechLabsProject_PsiData
![Python](https://img.shields.io/badge/Python-v3.8-blue.svg?logo=python&longCache=true&logoColor=white&style=flat-square&colorA=4c566a&colorB=5e81ac)
![Plotly](https://img.shields.io/badge/Plotly-v4.9.0-blue.svg?logo=python&longCache=true&logoColor=white&style=flat-square&colorA=4c566a&colorB=5e81ac)
![Pandas](https://img.shields.io/badge/Pandas-v1.1.1-blue.svg?logo=pandas&longCache=true&logoColor=white&style=flat-square&colorA=4c566a&colorB=B48EAD)

Análise de dados relacionados à saúde mental em Curitiba, no Brasil e no mundo. 
Feito com Python e Google Colaboratory de maio a julho de 2021.

<p align="center">
   <img src="/logo psidata.png" >
</p>


## Dashboard
https://chart-studio.plotly.com/dashboard/psidata:6/view#/

## Autores

- [Vitória Stavis de Araujo](https://vitoriastavis.github.io/vitoriastavis/)
-
-
-

## Base de dados

- Data SUS ([PySUS](https://pypi.org/project/PySUS))
- [E-Saúde - Curitiba](https://www.curitiba.pr.gov.br/dadosabertos/busca/?pagina=8)
- [OMS 1](https://apps.who.int/gho/data/node.main.MENTALHEALTH?lang=en)
[OMS 2](https://apps.who.int/gho/data/node.sdg.3-4-data?lang=en)
[OMS 3](https://www.who.int/teams/mental-health-and-substance-use/suicide-data)


## Documentação do projeto

- [Documentação API PySUS](https://pysus.readthedocs.io/_/downloads/en/latest/pdf/)
- [Documentação Plotly](https://plotly.com/python/)

## Sobre o projeto

[Houve um pico histórico nas pesquisas sobre transtornos mentais: buscas tiveram uma alta de 98% ante a média dos dez últimos anos.](https://saude.estadao.com.br/noticias/geral,com-pandemia-buscas-relacionadas-a-transtornos-mentais-no-google-batem-recorde,70003445996)

Entre as perguntas mais pesquisadas está ”como lidar com a ansiedade”. 

[Estima-se que 62 mil adolescentes morreram em 2016 como resultado de autolesão. O suicídio é a 3ª principal causa de morte entre adolescentes mais velhos (15 a 19 anos).](https://www.paho.org/pt/topicos/saude-mental-dos-adolescentes)

[Perto de 800 000 pessoas se vão por conta do suicídio cada ano, ou seja, *uma pessoa a cada 40 segundos*. Existem indicações de que para cada adulto que se suicida, podem ter havido mais de 20 que tentaram se suicidar.](https://www.who.int/teams/mental-health-and-substance-use/suicide-data)

Em 2021, com um ano e meio da pandemia da COVID-19, todos já sentiram pelo menos uma vez algum sintoma relacionado à saúde mental. Ansiedade, depressão, mudanças de humor repentinas, crises de pânico.[As pessoas reagem de maneira diferente a situações estressantes. Como cada um responde à pandemia pode depender de sua formação, da sua história de vida, das suas características particulares e da comunidade em que vive.](http://bvsms.saude.gov.br/ultimas-noticias/3427-saude-mental-e-a-pandemia-de-covid-19)

Isso é mais do que inspiração para este projeto. Esses dados são um sinal e uma oportunidade de nos conscientizarmos. 

O PsiData faz a análise da saúde mental em diferentes níveis: local (Curitiba), nacional e global.

Veja a análise gráfica no [Chart Studio](https://chart-studio.plotly.com/dashboard/psidata:6)

## Sobre Curitiba

[De acordo com o Ministério da Saúde,](https://www.bemparana.com.br/noticia/pr-bate-recorde-de-mortes-relacionadas-a-transtornos-mentais-diz-ministerio-da-saude) o estado do Paraná bate recorde de mortes relacionadas a transtornos mentais em 2020.

Foram analisados os dados do [sistema informatizado E-Saúde](http://esaude.curitiba.pr.gov.br/PortalSaude/). Foi criado em 2020 para **automatização de agendamento de consultas e realização de teleconsultas**, organização e remanejamento da agenda de profissionais e cadastro de medicamentos. O sistema registra atendimentos prestados pela **Secretaria Municipal de Saúde** em sua rede composta por Unidades Básicas de Saúde, Unidades de Pronto Atendimento, Centros de Especialidades Médicas e Odontológicas, entre outros. 

[Nos dados disponibilizados pela Prefeitura Municipal de Curitiba](https://www.curitiba.pr.gov.br/dadosabertos/busca/?pagina=8), podemos encontrar as seguintes informações sobre pessoas que requisitaram atendimento entre dezembro de 2020 e maio de 2021:
[Clique aqui para ver a tabela de informações.](https://imgur.com/a/DJyoQ9Y)

Nesse estudo, foi feita uma análise focando nas variáveis:
* Idade
* Sexo
* Tratamento no Domícilio (qual é o tratamento da água no domicílio)
* Energia Elétrica (se há energia elétrica na casa do cliente)
* Destino Lixo (para onde é encaminhado o lixo no domicílio)
* Fezes/Urina (destino das fezes e da urina no domicílio)
* Bairro

Foi usada a biblioteca pandas e numpy para análise, matplotlib e seaborn para os primeiros gráficos e plotly para os gráficos finais, passados para o [Chart Studio](https://chart-studio.plotly.com/dashboard/psidata:6).

A tabela geral possui 39813 amostras e 44 colunas. Os profissionais requisitados são: psicólogo clínico, farmacêutico, fisioterapeuta, fonoaudiólogo, nutricionista e educador físico. Dos requerimentos,  48,2% são por psicólogo. A partir da data de nascimento, foi gerada a idade dos pacientes. Os valores nulos foram substituídos pelo valor mais frequente.

Ao final, foi feita uma classificação com as classes 'fez consulta de psicologia' e 'não fez consulta de psicologia'. Foi usado o modelo de Random Forest tanto para seleção de características quanto para a classificação em si. As variáveis selecionadas foram: -.
O modelo foi feito com 80% dos dados para treino e 20% para teste. 

## Brasil
<img src="/SuícidiosBrasil(2017-2019).png" >

## Mundo
Segundo estimativas da [Organização Mundial de Saúde](https://www.who.int/teams/mental-health-and-substance-use/suicide-data) (OMS), ocorre um suicídio no mundo a cada 40 segundos.
### **Dados apontam que o suicídio em 2016 foi responsável por 1,4% das mortes no mundo, tornando-se a 18ª maior causa de mortes ([OMS](https://www.who.int/teams/mental-health-and-substance-use/suicide-data), 2021).**

Diante deste lamentável fato, é necessário apresentar e compreender os dados sobre este tipo de morte em diferentes países, para assim, fornecer ferramentas para análise e elaboração de ações voltadas a promover a saúde mental da população.

A partir dos dados disponíveis, é realizado um estudo com ênfase nos países da América Latina em comparação com alguns países ricos selecionados.
1.  A [primeira base de dados](https://apps.who.int/gho/data/node.main.MHSUICIDE?lang=en) trata da taxa de suicídios por 100 mil habitantes, para os países, no seu valor médio geral e também para cada sexo:
          a) Primeiramente é realizada um observação da evolução do percentual de suicídios de 2000, 2010 até 2019 e;
          b) Numa segunda perspectiva, se observam os dados a partir dos três anos recentes disponíveis, 2017, 2018 e 2019. 
2.  A [segunda base de dados](https://apps.who.int/gho/data/node.main.MHFAC?lang=en) refere-se a dados sobre infraestruturas e serviços voltados a promover a saúde mental nos países para o ano de 2016.


A amostra de dados levantados, busca realizar comparações entre a América Latina, o Brasil e países ricos selecionados.
## Conclusões



## Organizadores
<img src="/tech.png" >
- [TechLabs](https://www.techlabs.org/)

## Suporte

* Encontrou algum problema? Tem alguma sugestão?

Envie um email para: 
vitoriastavisa@gmail.com


