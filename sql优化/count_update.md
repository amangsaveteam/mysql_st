![alt text](1e490fd3-d1cf-45f5-86dc-caefed97cb3d.png)
![alt text](6aa1d5d8-68fe-49cd-92c0-03a12ddd851a.png)
# update更新字段要根据索引进行更新，索引更新是行锁，如果不根据索引更新会出发表锁，无法同时更新；
![alt text](efa6b9ae-c806-4420-808d-93e3e8e53ab6.png) 
--升级为表锁会降低并发