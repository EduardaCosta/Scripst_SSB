# Scripst_SSB
Scripts utilizadas para execução dos testes presentes na Dissertação. 

As scripts para o cenário A correspondem aos ficheiros com o seguinte nome: 
    hive_queries.sh - Esquema em Estrela (com o Hive)
    presto_queries.sh - Esquema em Estrela (com o Presto, utilizando Distributed Join)
    presto_queries_BJ.sh - Esquema em Estrela (com o Presto, utilizando Broadcast Join)
    hive_queries.sh - Tabela Desnormalizada (com o Hive)
    presto_queries_D.sh - Tabela Desnormalizada (com o Presto)

Para o cenário B1 os ficheiros foram adaptados de acordo com o atributo de particionamento e, sendo variações dos ficheiros anteriores, apresentam a seguinte notação: 
    ..._part - Particionamento por "Od_Year"
    ..._part2 - Particionamento por "S_Region"
    ..._part3 - Particionamento por "P_MFGR"
    ..._mpart1 - Particionamento por "Od_Year" e "Od_Monthnuminyear"
    ..._mpart2 - Particionamento por "Od_Year" e "S_Region"
    ..._mpart3 - Particionamento por "S_Region", "S_Nation" e "S_City"

As scripts utilizadas no cenário B2 são variações das scripts utilizados para o cenário A, alterando-se apenas os nomes das tabelas, pelo que não estão aqui apresentados. Na dissertação foi utilizada a seguinte notação:
    ..._mbuckets - Bucketing por "Orderdate", "Suppkey", "Custkey" e "Partkey"
    ..._buckets1 - Bucketing por "Custkey"
    ..._buckets2 - Bucketing por "Orderkey"
    ..._buckets3 - Bucketing por "Year" Sorted by "P_Brand1"
    ..._buckets4 - Bucketing por "Suppkey" (normalizada) e Bucketing por "
    ..._buckets41 - Bucketing por "P_Brand1" Sorted by "Od_Year"
  
As scripts utilizadas no cenário B3 são variações das scripts utilizadas para o cenário B1, de acordo com a configuração de Particionamento pretendida, pelo que nao estão aqui apresentadas. Na dissertação foi utilizada a seguinte notação: 
    ..._p_b2 - Particionamento por "Od_Year" e Bucketing por "Orderkey"
    ..._p2_b4 - Particionamento por "S_Region" e Bucketing por "Suppkey"
    ..._mpart2_b4 - Particionamento por "Od_Year" e "S_Region" e Bucketing por "Suppkey"
