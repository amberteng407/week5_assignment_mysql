# 第五週作業 MySQL

## 要求三
mysql > insert into user (id,name,username,password)
<br /> -> values (1,"ply","ply","ply");
<br /> -> values (2,"a","abc","123");
<br /> -> values (3,"b","def","456");
<br /> -> values (4,"c","ghi","789");
<br /> -> values (5,"d","jkl","000");
<br /> ![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Insert.png)

mysql > select * from user;
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%20all.png)
 
mysql > select count(*) from user;
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BCount.png)

mysql > select * from user order by time desc;
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BOrder%20by%20time.png)

mysql > select * from user order by time desc limit 1,3;
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BOrder%20by%20time%2BLimit.png)

mysql > select * from user where username="ply";
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BWhere%20username.png)

mysql > select * from user where username="ply" and password="ply";
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BWhere%20username%2Cpassword.png)

mysql > update user set name="丁滿" where username="ply";
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Update%20name.png)

mysql > delete from user;
<br />![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Delete%20all.png)

 
## 要求四
mysql > select * from message;
<br /> ![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Insert%20message.png)

mysql > select user.name, message.content
<br />  -> from message Inner join user
<br />  -> on user.id = message.user_id;
<br />  ![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Join%20name.png)
<br /> 
mysql > select user.name, user.username, message.content
<br />  -> from message Inner join user
<br />  -> on user.id = message.user_id;
<br />  -> where user.username = "ply";
<br />  ![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Join%20username.png)
