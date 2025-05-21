![alt text](c164d3d0-e088-4be2-8162-6cec977e1a8d.png)
![alt text](da6a2239-41c8-4207-8f4d-8321c5ab9999.png)
select id  from tb_sku order by id limit 9000000,10;
# 多表查询思路
select s.* from tb_sku s ,(select id from tb_sku order by id limit 9000000,10) a where s.id = a.id;
