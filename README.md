SolrSqlBatchEntityProcessor
===========================

Used for Sor DIH, optimization for org.apache.solr.handler.dataimport.SqlEntityProcessor;
This class will help us to resolve OutOfMemory Problems - it optimizes the SQL, adding ID and LIMIT strategies, 
      for examples: 'select c1,c2,c3 from table_1  where id > 10000 limit 500';

Additionally, it will be better if DIH support multiple threads strategy.
