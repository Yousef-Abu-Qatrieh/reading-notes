#SQl Summary   
we use select query to return specific  Columns from table   
we use where condition to determine  column values that should be include or not    
we use between to determine the range of two Values and Not between to check the value doesn't include in this range   
we use And/Or operator to determine if some data exist or not also we use IN (…) NOT IN (…) to determine the data in the list or not   
we use = or != to search on string  = for exact same string and != same string inequality comparison    
we use LIKE and Not LIKE to search on string if exist or not also we use % to search on part of string if exist   
we use DISTINCT to remove dublicate data   
we use ORDER BY to sort our data asc or desc   
we use limit to reduce the row numbers that we want to search on also we use OFFSET  will specify where to begin counting the number rows from    
we use Join to combine row data across two separate tables using this unique key   
we use Insert to add new data to our table use this query (INSERT INTO mytable VALUES (value_or_expr, another_value_or_expr, …); )      
we use Update to update our table data use this query (UPDATE mytable SET column = value_or_expr,  other_column = another_value_or_expr, WHERE condition);
we use Delete to delete row from our table using  this query (DELETE FROM mytable WHERE condition;)   
we use CREATE TABLE to create a new tabele and we use IF NOT EXISTS to check if we didn't create a table have the same name 
we use this query to create table :   
CREATE TABLE IF NOT EXISTS mytable (  column DataType TableConstraint DEFAULT default_value, another_column DataType TableConstraint DEFAULT default_value);    
we use ALTER TABLE to update our table data like change name add  delete      
we use Drop to delete table that we  create using this query (DROP TABLE IF EXISTS mytable;) 
