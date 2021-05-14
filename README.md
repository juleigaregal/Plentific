/****** Script for SelectTopNRows command from SSMS  ******/
SELECT [TYPE],
LEFT(transferdate, 7) as DATES, -- TRANSFORMS DATE TO YYYY-MM FORMAT
AVG(price) as AVG_PRICE
,[PostCode]
   
  
 FROM [Càiniǎo].[dbo].[pp-complete2]
 GROUP BY
 PostCode, 
 TYPE, 
 left(transferdate, 7)
 
