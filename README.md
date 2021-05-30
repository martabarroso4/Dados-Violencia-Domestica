# Dados relativos aos casos de violência doméstica em Portugal

Este projeto foi criado no âmbito da unidade curricular de Programação e Algoritmos II, com o objetivo de analisar e desenvolver o tratamento de dados. 
O ficheiro csv utilizado foi retirado de https://github.com/dssg-pt/mp-violencia-domestica , focando a análise no distrito de Coimbra. Na mesma, comparamos os casos de violência doméstica em Coimbra com os números referentes às duas principais cidades portuguesas, Lisboa e Porto; permite-nos ter uma noção relativa à sua evolução ao longo do tempo, comparando os números nestes três distritos. Posto isto, foram também comparados os casos de Coimbra entre vítimas do sexo feminino, masculino e intersexo. As colunas presentes no ficheiro continham objetos que foram transformados em 

# 📖 Contexto 

A violência doméstica é um crime que, ao contrário do que é acreditado, não diz respeito a idades, estatuto social, sexo, religião, cultura, orientação sexual, estado civil ou formação. Este crime é praticado por alguém que inflige maus tratos físicos ou psicológicos, uma vez ou de forma consistente, a outra pessoa (conjugue/ex-conjugue; namorado/a ou ex-namorado/a) que co-habitem, ou não e, também, a sujeitos que, de algum modo, não tem capacidades para se defender (idosos, grávidas, crianças, pessoas com algum tipo de deficiência). 

Neste projeto, a análise dos dados referentes a um tema como a Violência Doméstica surge num contexto de sensibilização, com o objetivo de trazer mais consciência e exposição quanto à gravidade desta situação e para mostrar os elevados números associados a este crime. 

As estatísticas presentes neste projeto permitiram que retirássemos várias conclusões sobre este assunto. Em primeiro lugar, refuta-se o estereótipo da inexistência de vítimas masculinas, uma vez que o número de casos sobre este sexo mostra-se bastante elevado. Relativamente às idades, percebe-se que há um aumento significativo de acordo com a idade, ou seja, o número de pessoas mais velhas que são vítimas deste crime é mais elevado que o número de jovens. 

Segundo o relatório anual da APAV, 79% dos crimes contra pessoas assinalados estavam associados à Violência Doméstica.

# 👁️ Questões abordadas 

Média de casos em Coimbra, Lisboa e Porto, por ano.

Média de casos dos diferentes sexos em Coimbra, por ano.

Evolução dos casos em Coimbra, ao longo do tempo, discriminada por sexo.   

Evolução dos casos em Coimbra, Lisboa e Porto, ao longo do tempo e respetiva comparação. 

Taxa (em percentagem) de casos entre sexos, em Coimbra, nos diferentes anos (2009-2019).

Taxa (em percentagem) de casos por 1000 habitantes, em Coimbra, Lisboa e Porto, nos diferentes anos (2009-2019).  


# 📉 Fontes de dados e API´s utilizados 

Ficheiro [data.csv](https://github.com/dssg-pt/mp-violencia-domestica/tree/main/data) utilizado. 

##### Os dados que se encontram no ficheiro **data.csv** provém dos seguintes endereços:

[Estatísticas fornecidas pela APAV relativas ao período 2013-2018](https://apav.pt/apav_v3/images/pdf/Estatisticas_APAV_Violencia_Domestica_2013_2018.pdf)

[Dados trimestrais fornecidos pelo Governo](https://www.cig.gov.pt/area-portal-é-da-violencia/violencia-no-namoro/documentacao/)

[Dados anuais por concelho fornecidos pelo INE](https://www.ine.pt/xportal/xmain?xpid=INE&xpgid=ine_main)

[Dados anuais por concelho fornecidos pelo PORDATA](https://www.pordata.pt/DB/Ambiente+de+Consulta/Nova+Consulta)

[Dados anuiais de monitorização forneciddos pelo Ministério da Administração Interna](https://www.sg.mai.gov.pt/paginas/violenciadomesticarelatorios.aspx)

###### Todos os dados acima listados são referentes aos casos de violênia doméstica a nível nacional. 

# 🧱 Estrutura 

O repositório está organizado da seguinte forma: 

**data.csv**: Ficheiro que contém os dados relativos aos casos de violência doméstica em Portugal.

**violencia_domestica.ipynb**: [Tratamento/limpeza de dados e comparação dos números relativos aos distritos de Coimbra, Porto e Lisboa, juntamente com a comparação dos números referentes aos diferentes sexos.](https://github.com/martabarroso4/Dados-Violencia-Domestica/blob/main/violencia_domestica.ipynb)  

# 📔 Dicionário de dados 

| Nome da coluna | Significado | Tipo de dado |  
| -------------- | ----------- | ----------------- |
| ano            | Ano referente aos dados. | object
| municipio      | Município referente aos dados. | string 
| codigo_municipio | Código do município. | object
| num_habitantes | Número de habitantes referente ao município naquele ano. | object
| num_crimes     | Número de crimes ocorridos naquele município e ano. | object
| num_vitimas    | Número de vítimas referente àquele município e ano. | object
| num_vitima_feminina | Número de vítimas do sexo feminino referente àquele município e ano. | object
num_vitima_masculina | Número de vítimas do sexo masculino referente àquele município e ano. | object
num_vitima_intersexo | Número de vítimas intersexo referente àquele município e ano. | object
num_vitima_idade_3 | Número de vítimas com idade até aos 3 anos. | object
num_vitima_idade_5 | Número de vítimas com idade entre os 3 e 5 anos. | object
num_vitima_idade_10 | Número de vítimas com idade entre os 5 e 10 anos. | object
num_vitima_idade_17 | Número de vítimas com idade entre os 10 e 17 anos. | object
num_vitima_idade_24 | Número de vítimas com idade entre os 17 e 24 anos. | object
num_vitima_idade_34 | Número de vítimas com idade entre os 24 e 34 anos. | object
num_vitima_idade_44 | Número de vítimas com idade entre os 34 e 44 anos. | object
num_vitima_idade_54 | Número de vítimas com idade entre os 44 e 54 anos. | object
num_vitima_idade_64 | Número de vítimas com idade entre os 54 e 64 anos. | object
num_vitima_idade_mais_65 | Número de vítimas com idade superior a 65 anos. | object
num_crimes_vitimacao_continuada | Número de casos em que a a vítimação persistiu. | object  
num_crimes_vitimacao_nao_continuada | Número de casos em que a vitimação não persistiu. | object


