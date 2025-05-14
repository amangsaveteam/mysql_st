# 分页查询
# 1.查询第1页员工数据，每页展示10条记录 limit 起始索引，索引记录
select * from emp limit  0,10;
# 2.查询第2页员工数据，每页展示10条记录--------》（页码-1）*页展示记录数
select * from emp limit  10,10;