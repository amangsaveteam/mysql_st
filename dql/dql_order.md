# 排序查询
# 1.根据年龄进行升序排序(默认是升序)
select * from emp order by  age asc;
# 2.根据入职时间进行降序排序
select * from emp order by  entrydate desc ;
# 3.根据年龄进行升序排序，年龄相同在根据入职时间进行降序排序
select * from emp order by  age asc,entrydate desc;