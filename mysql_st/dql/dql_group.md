# 分组查询
# 1.根据性别分组，分别统计男女员工数量
select gender,count(*) from emp group by gender ;
# 2.根据性别分组，分别统计男女员工平均年龄
select gender,avg(age) from emp group by gender ;
# 3.查询年龄小于45的员工，并根据工作地址分组，获取员工数量大于等于3的工作地址
select workaddress,count(*) as countaddress from emp where age < 45 group by workaddress having count(*) >= 3;