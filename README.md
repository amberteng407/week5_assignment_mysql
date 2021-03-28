# 第五週作業 MySQL

## 要求三
mysql > insert into user (id,name,username,password)
<br />  -> values (1,"ply","ply","ply");
<br />  -> values (2,"a","abc","123");
<br />  -> values (3,"b","def","456");
<br />  -> values (4,"c","ghi","789");
<br />  -> values (5,"d","jkl","000");
<br />  ![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Insert.png)
<br /> 
mysql > select * from user;
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%20all.png)
<br /> 
mysql > select count(*) from user;
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BCount.png)
<br /> 
mysql > select * from user order by time desc;
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BOrder%20by%20time.png)
<br /> 
mysql > select * from user order by time desc limit 1,3;
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BOrder%20by%20time%2BLimit.png)
<br /> 
mysql > select * from user where username="ply";
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BWhere%20username.png)
<br /> 
mysql > select * from user where username="ply" and password="ply";
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Select%2BWhere%20username%2Cpassword.png)
<br /> 
mysql > update user set name="丁滿" where username="ply";
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Update%20name.png)
<br /> 
mysql > delete from user;
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Delete%20all.png)
<br /> 
<br /> 
## 要求四
mysql > select * from message;
![image](https://github.com/amberteng407/week5_assignment_mysql/blob/main/image/Insert%20message.png)
<br /> 
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
