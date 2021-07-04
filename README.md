# Docker Big Data Tools
:information_source: **This docker-compose file is configured to run multiple nodes.**


This is a Hadoop Cluster that contains the necessary tools that can be used in the BigData domain, It's a collection of docker containers that you can use directly to have the maximum of tools like :


* **Hive** 
* **Hue**
* **MySql**
* **Zookeeper**
* **Kafka**
* **Hbase**
* **Mongo**
* **Metabase**
* **Streamsets**
* **Sqoop**
* **Storm**



## Docker Images Used 
- **namenode** : [fjardim/namenode_sqoop ](https://hub.docker.com/r/fjardim/namenode_sqoop)
- **datanode** : [fjardim/datanode ](https://hub.docker.com/r/fjardim/datanode)
- **hive-server** : [fjardim/hive](https://hub.docker.com/r/fjardim/hive)
- **hive-metastore** : [fjardim/hive](https://hub.docker.com/r/fjardim/hive)
- **hive-metastore-postgresql** : [fjardim/hive-metastore](https://hub.docker.com/r/fjardim/hive-metastore)
- **hue** : [fjardim/hue](https://hub.docker.com/r/fjardim/hue)
- **mysql** : [fjardim/mysql](https://hub.docker.com/r/fjardim/mysql/)
- **zookeeper** : [fjardim/zookeeper](https://hub.docker.com/r/fjardim/zookeeper)
- **kafka** : [fjardim/kafka](https://hub.docker.com/r/fjardim/kafka)
- **presto-coordinator** : [fjardim/prestodb](https://hub.docker.com/r/fjardim/prestodb)
- **hbase-master** : [fjardim/hbase-master](https://hub.docker.com/r/fjardim/hbase-master)
- **mongo** : [fjardim/mongo](https://hub.docker.com/r/fjardim/mongo)
- **mongo-express** : [fjardim/mongo-express](https://hub.docker.com/r/fjardim/mongo-express)
- **kafkamanager** : [fjardim/kafkamanager](https://hub.docker.com/r/fjardim/kafkamanager)
- **metabase** : [fjardim/metabase](https://hub.docker.com/r/fjardim/metabase)
- **streamsets** : [streamsets/datacollector:3.13.0-latest](https://hub.docker.com/layers/streamsets/datacollector/3.13.0-latest/)
- **storm** : [fmantuano/apache-storm:develop](https://hub.docker.com/layers/fmantuano/apache-storm/develop/)
- **jupyter-spark** : [fjardim/jupyter-spark](https://hub.docker.com/r/fjardim/jupyter-spark)
---
## Instalations
```bash=
git clone https://gitlab.com/ZakariaMahmoud/docker-bigdata-tools.git

cd docker-bigdata-tools

sudo docker-compose up -d
```
> ⚠️ **It takes some time for launch and configure all the images**

## Screenshots
### **Namenode**
- **URL** : http://localhost:50070/

![](https://i.imgur.com/0suoN0k.png)


> 👁️ You can see here 3 Live Nodes**

![](https://i.imgur.com/Hhf9K3A.png)

![](https://i.imgur.com/aZFGqB2.png)

![](https://i.imgur.com/2O98bq8.png)


### **Datanode 1**
- **URL** : http://localhost:50075/

![](https://i.imgur.com/SgBYFNO.png)


### **Datanode 2**
- **URL** : http://localhost:50080/

![](https://i.imgur.com/AEaSjTH.png)


### **Datanode 3**
- **URL** : http://localhost:50085/

![](https://i.imgur.com/uxjs1nf.png)

### **Hue**
- **URL** : http://localhost:8888/

**Username : admin**
**Password : admin**

![](https://i.imgur.com/XX7tyum.png)

**After click in Sign In**


![](https://i.imgur.com/gjrohHE.png)


**Now you can use Hive**

 - Simple Query for test
```sql=
CREATE TABLE IF NOT EXISTS users(id INT, name VARCHAR(45), website VARCHAR(45));

INSERT INTO users VALUES(1,"mahmoud zakaria","www.mahmoud.ma");
```
![](https://i.imgur.com/CtcgKOx.png)

- After insert data you can execute select query. 

```sql=
SELECT *FROM users;
```
![](https://i.imgur.com/wFId19M.png)

* Hue Dashboard

![](https://i.imgur.com/mPxPSwQ.png)


## kafka Manager
- **URL** : http://localhost:9000/


![](https://i.imgur.com/ODSOhp1.png)

## Cluster Overview
- **URL** : http://localhost:8080/

![](https://i.imgur.com/71L8GJH.png)

## Hbase
- **URL** : http://localhost:16010/

![](https://i.imgur.com/QXix2Za.png)

![](https://i.imgur.com/8YdxLxu.png)


## Storm UI
- **URL** : http://localhost:8090/

![](https://i.imgur.com/Uz4kLG1.png)
![](https://i.imgur.com/qAAa8uo.png)

## Jupyter
- **URL** : http://localhost:8889/

![](https://i.imgur.com/b7zOYtX.png)

## Mongo Express
- **URL** : http://localhost:8081/
![](https://i.imgur.com/aHqGu7Q.png)

## StreamSets
- **URL** : http://localhost:18630/

**Username : admin**
**Password : admin**

![](https://i.imgur.com/zY9jqhv.png)
---
## Created by

* 🇲🇦 **Mahmoud Zakaria** 
* 🌐 [www.mahmoud.ma](https://www.mahmoud.ma/)