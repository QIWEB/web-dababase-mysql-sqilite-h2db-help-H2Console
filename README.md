# web-dababase-mysql-sqilite-h2db-help-H2Console
全能java数据库管理web网页版 支持mysql sqlite等几乎主流数据库方便 by qiweb 20240702

# 快速开始：
安装Java jdk*+
# cmd 运行 
java -cp "h2-2.1.214.jar;sqlite-jdbc-3.34.0.jar;mysql-connector-java-5.1.32.jar" org.h2.tools.Server -web -webAllowOthers -webAdminPassword yourSecurePassword

# 支持22种数据库：
SQLite              
MySQL               
H2 (Embedded)       
H2 (Server)         
Derby (Embedded)    
Derby (Server)      
HSQLDB              
MariaDB             
PostgreSQL          
MS SQL Server 2005  
MS SQL Server 2000  
Oracle              
DB2                 
Firebird Server     
Azure SQL           
Hive                
Hive 2              
Impala              
Redshift            
Snowflake           
Teradata            
JNDI Data Source    


# 不到5mb大小的jar 支持 20多种语言：
"cs">Čeština 
"de">Deutsch 
"en" selected="">English 
"es">Español 
"fr">Français 
"hi">Hindi हिंदी 
"hu">Magyar 
"ko">한국어 
"in">Indonesia 
"it">Italiano 
"ja">日本語 
"nl">Nederlands 
"pl">Polski 
"pt_BR">Português (Brasil) 
"pt_PT">Português (Europeu) 
"ru">русский 
"sk">Slovensky 
"tr">Türkçe 
"uk">Українська 
"zh_CN">中文 (简体) 
"zh_TW">中文 (繁體) 


# mysql8需要关闭ssl
关闭ssl
由于容器默认可能没有安装vi或vim，你需要使用包管理器（如apt-get，假设容器基于Debian或Ubuntu）来安装。先更新软件包列表，然后安装vim：
Bash
apt-get update && apt-get install -y vim
ssl=0

/etc/mysql/my.cnf 

登录到SHOW VARIABLES LIKE '%ssl%';
[mysqld]
ssl=0
skip_ssl


echo ssl=0 >> my.cnf
echo skip_ssl >> my.cnf

驱动使用 com.mysql.cj.jdbc.Driver
mysql5使用
