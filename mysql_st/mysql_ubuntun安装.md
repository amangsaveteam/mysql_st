
、、、
sudo apt  update
sudo apt install mysql-server
、、、
-- 查看mysql是否正常运行
sudo systemctl status mysql
-- 查看mysql的配置文件
sudo cat /etc/mysql/debian.cnf
-- 登录mysql
mysql -udebian-sys-maint -pK4nA1PkvVpzRLi2n

use mysql

-- 查看rooto用户
select user,plugin from user;
update user set plugin='mysql_native_password'  where user = 'root';
select user,plugin from user;
# 一定要更新权限
flush privileges;
# 更新密码
alter user 'root'@'localhost' identified by 'py12345';
exit;

# 登陆mysql
mysql -uroot -ppy12345
