# Part2

## SQL Server to Postgres **fullload and cdc** task
1. For source EC2 SQL Server rdp (remote desktop) using login **\administrator** and password **pAsswOrd12**
2. from the documentation https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Source.SQLServer.html find out the prerequisites for the EC2 SQL Server to use as CDC source.
3. Make the necessary changes to source sql server using rdp session and client ssms (SQLServer Management Studio)
4. Setup a new fullload and cdc task to migrate table **mytable** from sqlserver to aurora postgres.
5. run sample inserts on source sql server and verify data is being migrated to aurora postgres
6. additionally you can create update/delete statements to test the cdc.

```
--sample inserts
INSERT INTO mytable([fname],[lname]) VALUES('Ferris','Mccoy'),('Bradley','Britt'),('Raphael','Sampson'),('Lane','Gallagher'),('Jin','Marks'),('Marshall','Houston'),('Mannix','Mullen'),('Harper','Alvarez'),('Fuller','Mcneil'),('Denton','Petty');
INSERT INTO mytable([fname],[lname]) VALUES('Blake','Farley'),('Vladimir','Davenport'),('Roth','Rhodes'),('Yardley','Vazquez'),('Wang','Maldonado'),('Josiah','Colon'),('Mark','Head'),('Hilel','Koch'),('Linus','Hull'),('Solomon','Wells');
```
