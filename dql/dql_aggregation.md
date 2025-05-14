# 聚合函数
# 将一列数据作为一个整体，进行纵向计算

# 1.统计企业员工数量--null不参与聚合函数
select count(*) from emp;
select count(id) from emp;
# 2.统计企业员工平均年龄
select avg(age) from emp;
# 3.统计企业员工最大年龄
select max(age) from emp;
# 4.最小年龄
select min(age) from emp;
# 5.统计西安地区员工年龄之和
select sum(age) from emp where workaddress = '西安';