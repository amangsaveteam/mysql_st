# 插入指定字段
insert into employee(id, workno, name, gender, age, idcard, entrydate) values (1,'1','Itcast','男',10,'123456789012345678','2000-01-01');
# 查询表
select * from employee;
# 插入全部字段
insert into employee values (2,'2','张无忌','男',18,'123456789012345670','2005-01-01');
# 添加多条字段
insert into employee values (3,'3','韦一笑','男',18,'123456789012345671','2005-01-01'),(4,'4','赵敏','女',18,'123456789012345672','2005-01-01');
# 修改指定字段
update employee set name = 'itheima' where id = 1;
# 同时修改多个指定字段
update employee set name = '小昭',gender = '女' where id = 1;
# 修改所有的指定字段
update employee set entrydate = '2008-01-01' ;
# 删除指定字段
delete from employee where gender = '女';
# 删除全部字段
delete from employee;