CREATE TABLE ValueTable (id int);  
BEGIN TRANSACTION;              -- aqui começa a transação
       INSERT INTO ValueTable VALUES(1);  
       INSERT INTO ValueTable VALUES(2);  
COMMIT;                         -- aqui termina e "grava" tudo


--Enquanto não dá o COMMIT essas inserções não constam de fato no banco de dados. Um ROLLBACK descartaria tudo feito antes.
