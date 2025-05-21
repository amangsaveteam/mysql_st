# 1.查询年龄为20,21,22,23岁的女性员工信息。
select * from emp where age in(20,21,22,23) and gender = '女';

# 2.查询性别为 男，并且年龄在20-40 岁(含)以内的姓名为三个字的员工
select * from emp where age between 20 and 40 and gender = '男' and name like '___';
# 3.统计员工表中，年龄小于60岁的，男性员工和女性员工的人数。
select gender,count(*) from emp where age < 60 group by gender ;
# 4.查询所有年龄小于等于35岁员工的姓名和年龄，并对查询结果按年龄升序排序，如果年龄相同按入职时间降序排序。
select name,age from emp where age <= 35 order by age asc , entrydate desc ;
# 5.查询性别为男，且年龄在20-40 岁（含）以内的前5个员工信息。对查询的结果按年龄升序排序，年龄相同按入职时间升序排序。
select * from emp where age between 20 and 40 and gender = '男' order by age asc , entrydate asc limit 0,5;