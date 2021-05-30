# Dados relativos aos casos de violência doméstica em Portugal

Este projeto foi criado no âmbito da unidade curricular de Programação e Algoritmos II do 1º ano de Licenciatura em Comunicação e Design Multimédia, com o objetivo de analisar e desenvolver o tratamento de dados relativos aos casos de Violência Doméstica em Portugal.
O ficheiro csv utilizado foi retirado de https://github.com/dssg-pt/mp-violencia-domestica , focando a análise no distrito de Coimbra. Na mesma, comparamos os casos de violência doméstica em Coimbra com os números referentes às duas principais cidades portuguesas, Lisboa e Porto; permite-nos ter uma noção relativa à sua evolução ao longo do tempo, comparando os números nestes três distritos. Posto isto, foram também comparados os casos de Coimbra entre vítimas do sexo feminino, masculino e intersexo.

# Fontes de dados e API´s utilizados 

Ficheiro [data.csv](https://github.com/dssg-pt/mp-violencia-domestica/tree/main/data) utilizado para análise.

##### Os dados que se encontram no ficheiro **data.csv** provém dos seguintes endereços:

[Estatísticas fornecidas pela APAV relativas ao período 2013-2018](https://apav.pt/apav_v3/images/pdf/Estatisticas_APAV_Violencia_Domestica_2013_2018.pdf)

[Dados trimestrais fornecidos pelo Governo](https://www.cig.gov.pt/area-portal-da-violencia/violencia-no-namoro/documentacao/)

[Dados anuais por concelho fornecidos pelo INE](https://www.ine.pt/xportal/xmain?xpid=INE&xpgid=ine_main)

[Dados anuais por concelho fornecidos pelo PORDATA](https://www.pordata.pt/DB/Ambiente+de+Consulta/Nova+Consulta)

[Dados anuiais de monitorização forneciddos pelo Ministério da Administração Interna](https://www.sg.mai.gov.pt/paginas/violenciadomesticarelatorios.aspx)

###### Todos os endereços acima listados são referentes aos dados de casos de violênia doméstica a nível nacional. 

# Estrutura 

O repositório está organizado da seguinte forma: 

**data.csv**: Ficheiro que contém os dados relativos aos casos de violência doméstica em Portugal (número de crimes e vítimas, sexo e faixa etária das mesmas e casos em que o crime foi ou não descontinuado) durante o período 2009-2019.

**violencia_domestica.ipynb**: [Tratamento/limpeza de dados e comparação dos números relativos aos distritos de Coimbra, Porto e Lisboa, juntamente com a comparação dos números referentes aos diferentes sexos no distrito de Coimbra.](https://github.com/martabarroso4/Dados-Violencia-Domestica/blob/main/violencia_domestica.ipynb)  

# Dicionário de dados 

| Nome da coluna | Significado | Possíveis valores | 
| -------------- | ----------- | ----------------- |
| ano            | ano referente aos dados | Inteiro >= 0
| municipio      | município referente aos dados | String 
| codigo_municipio | código do município | Inteiro >= 0
| num_habitantes | número de habitantes referente ao município naquele ano | Inteiro >= 0
| num_crimes     | número de crimes ocorridos naquele município e ano | Inteiro >= 0
| num_vitimas    | número de vítimas referente àquele município e ano | Inteiro >= 0
| num_vitima_feminina | número de vítimas do sexo feminino referente àquele município e ano | Inteiro >= 0 
num_vitima_masculina | número de vítimas do sexo masculino referente àquele município e ano | Inteiro >= 0
num_vitima_intersexo | número de vítimas intersexo referente àquele município e ano | Inteiro >= 0 
num_vitima_idade_3 | | Inteiro >= 0
num_vitima_idade_5 | | Inteiro >= 0
num_vitima_idade_10 | | Inteiro >= 0
num_vitima_idade_17 | | Inteiro >= 0
num_vitima_idade_24 | | Inteiro >= 0
num_vitima_idade_34 | | Inteiro >= 0
num_vitima_idade_44 | | Inteiro >= 0
num_vitima_idade_54 | | Inteiro >= 0
num_vitima_idade_64 | | Inteiro >= 0
num_vitima_idade_mais_65 | número de vítimas com idade superior a 65 anos referente àquele municípo e ano | Inteiro >= 0
num_crimes_vitimacao_continuada | | Inteiro >= 0
num_crimes_vitimacao_nao_continuada | | Inteiro >= 0


