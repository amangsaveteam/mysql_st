# 数据控制语言，用来管理数据库用户，控制数据库的访问权限

# 用户管理
# 1.创建用户 itcast ，只能够在当前主机localhost访问，密码123456;
create user 'itcast'@'localhost' identified by '123456';

# 2.创建用户 heima ，可以在任意主机访问该数据库，密码123456;
create user 'heima'@'%' identified by '123456';

# 3.修改用户 heima 的访问密码为 1234;
alter user 'heima'@'%'  identified with mysql_native_password by '1234';

# 4.删除itcast@localhost用户
drop user 'itcast'@'localhost';

# 权限控制
# 1.查询权限
show grants for 'heima'@'%';
# 2.授予权限,多个权限之间用逗号分割
grant all on itcast.* to 'heima'@'%';
# 3.撤销权限
revoke all on itcast.* from 'heima'@'%';