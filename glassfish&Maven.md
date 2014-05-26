
#### glassfishのインストールとは設定

環境変数の設定なら：

GLASSFISH_HOME:C:\glassfish3

path:%GLASSFISH_HOME%\bin

====================================
 
cd C:\glassfish3\bin

asadmin stop-domain domain1

asadmin delete-domain domain1

asadmin create-domain domain1
 
asadmin start-domain domain1

asadmin add-resources D:\NetBeansProjects\trunk\xxx\src\main\webapp\WEB-INF\glassfish-resources.xml
 

====================================


asadmin change-admin-password
 
asadmin enable-secure-admin
 
asadmin diaable-secure-admin
 
asadmin create-service domain1

====================================

#### Maven CMD命令

cd D:\NetBeansProjects\trunk\xxx

d:

mvn clean install

cd D:\NetBeansProjects\trunk\xxx

d:

mvn clean install

====================================

#### JDBC接続プール新規追加  

JDBC接続プール名：　mysql\_timeline\_timelinePool  
リソースタイプ：　javax.sql.DataSource  
ドライバのベンダー：　MySQL  
URL： jdbc:mysql://localhost:3306/xxx?zeroDateTimeBehavior=convertToNull  
driverClass： com.mysql.jdbc.Driver  
Password： xxx  
portNumber： 3306  
databaseName： xxx  
User： xxx  
serverName： localhost  

**JDBCリソース新規追加**  

JNDI名： jdbc/xxx 
プール名： mysql_timeline_timelinePool  

====================================

#### ログ

C:\glassfish3\glassfish\domains\domain1\logs\server.log
