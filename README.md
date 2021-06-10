# TechLabsProject_PsiData

Análise de dados relacionados à saúde mental em Curitiba, no Brasil e no mundo. 
Feito com Python e Google Colaboratory de maio a julho de 2021.

<p align="center">
  <img src="/tech.png" >
</p>

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

[Houve um pico histórico nas pesquisas sobre transtornos mentais: buscas sobre o tema tiveram uma alta de 98% ante a média dos dez últimos anos.](https://saude.estadao.com.br/noticias/geral,com-pandemia-buscas-relacionadas-a-transtornos-mentais-no-google-batem-recorde,70003445996)

Entre as perguntas mais pesquisadas está ”como lidar com a ansiedade”. Em junho, a pergunta ”o que é felicidade” teve o maior volume de buscas dos últimos oito anos.

[Estima-se que 62 mil adolescentes morreram em 2016 como resultado de autolesão. O suicídio é a 3ª principal causa de morte entre adolescentes mais velhos (15 a 19 anos).](https://www.paho.org/pt/topicos/saude-mental-dos-adolescentes)

[Perto de 800 000 pessoas se vão por conta do suicídio cada ano, ou seja, *uma pessoa a cada 40 segundos*. Existem indicações de que para cada adulto que se suicida, podem ter havido mais de 20 que tentaram se suicidar.](https://www.who.int/teams/mental-health-and-substance-use/suicide-data)

Em 2021, com um ano e meio da pandemia da COVID-19, todos já sentiram pelo menos uma vez algum sintoma relacionado à saúde mental. Ansiedade, depressão, mudanças de humor repentinas, crises de pânico.[As pessoas reagem de maneira diferente a situações estressantes. Como cada um responde à pandemia pode depender de sua formação, da sua história de vida, das suas características particulares e da comunidade em que vive.](http://bvsms.saude.gov.br/ultimas-noticias/3427-saude-mental-e-a-pandemia-de-covid-19)

Isso é mais do que inspiração para este projeto. Esses dados são um sinal e uma oportunidade de nos conscientizarmos. 

O PsiData faz a análise da saúde mental em diferentes níveis: local (Curitiba), nacional e global.

Veja a análise gráfica no [Chart Studio](https://chart-studio.plotly.com/dashboard/psidata:6)

# Sobre Curitiba

[De acordo com o Ministério da Saúde,](https://www.bemparana.com.br/noticia/pr-bate-recorde-de-mortes-relacionadas-a-transtornos-mentais-diz-ministerio-da-saude) o estado do Paraná bate recorde de mortes relacionadas a transtornos mentais em 2020.

Foram analisados os dados do [sistema informatizado E-Saúde](http://esaude.curitiba.pr.gov.br/PortalSaude/). Foi criado em 2020 para **automatização de agendamento de consultas e realização de teleconsultas**, organização e remanejamento da agenda de profissionais e cadastro de medicamentos. O sistema registra atendimentos prestados pela **Secretaria Municipal de Saúde de Curitiba** em sua rede de atenção. Esta rede é composta por Unidades Básicas de Saúde, Unidades de Pronto Atendimento, Centros de Especialidades Médicas e Odontológicas, entre outros. 

[Nos dados disponibilizados pela Prefeitura Municipal de Curitiba](https://www.curitiba.pr.gov.br/dadosabertos/busca/?pagina=8), podemos encontrar as seguintes informações sobre pessoas que requisitaram atendimento de Psicologia:
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


## Organizadores

- [TechLabs](https://www.techlabs.org/)

## Suporte

* Encontrou algum problema? Tem alguma sugestão?

Envie um email para: 



