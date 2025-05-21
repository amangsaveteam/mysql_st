# 条件查询

# 条件查询

# 1. 查询年龄等于 88 的员工
select * from emp where age = 88;
# 2. 查询年龄小于 20 的员工信息
select * from emp where age < 20;
# 3. 查询年龄小于等于 20 的员工信息
select * from emp where age <= 20;
# 4. 查询没有身份证号的员工信息
select * from emp where idcard is null;
# 5. 查询有身份证号的员工信息
select * from emp where idcard is not null;
# 6. 查询年龄不等于 88 的员工信息
select * from emp where age != 88;
select * from emp where age <> 88;
# 7. 查询年龄在 15 岁（包含）到 20 岁（包含）之间的员工信息
select * from emp where age >= 15 and age <= 20;
select * from emp where age >= 15 && age <= 20;
select * from emp where age between 15 and 20;
# 8. 查询性别为 女 且年龄小于 25 岁的员工信息
select * from emp where age < 25 && gender = '女';
# 9. 查询年龄等于 18 或 20 或 40 的员工信息
select * from emp where age = 18 or age = 20 or age = 40;
select * from emp where age in(18,20,40);
# 10. 查询姓名为两个字的员工信息--使用模糊匹配 单个字符_,任意字符%
select * from emp where name like '__';
# 11. 查询身份证最后一位是X的员工信息
select * from emp where idcard like '%X';