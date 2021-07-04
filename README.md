# Docker Big Data Tools
:information_source: **This docker-compose file is configured to run multiple nodes.**


This is a Hadoop Cluster that contains the necessary tools that can be used in the BigData domain, It's a collection of docker containers that you can use directly to have the maximum of tools like :


* **Hive** 
* **Hue**
* **MySql**
* **Zookeeper**
* **Kafka**
* **Hbase**
* **NiFi**
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
- **Apachi NiFi** : [apache/nifi:latest](https://hub.docker.com/r/apache/nifi)
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



> 👁️ You can see here 3 Live Nodes**


### **Datanode 1**
- **URL** : http://localhost:50075/


### **Datanode 2**
- **URL** : http://localhost:50080/


### **Datanode 3**
- **URL** : http://localhost:50085/


### **Hue**
- **URL** : http://localhost:8888/

**Username : admin**
**Password : admin**


**After click in Sign In**


**Now you can use Hive**

 - Simple Query for test
```sql=
CREATE TABLE IF NOT EXISTS users(id INT, name VARCHAR(45), website VARCHAR(45));

INSERT INTO users VALUES(1,"mahmoud zakaria","www.mahmoud.ma");
```

- After insert data you can execute select query. 

```sql=
SELECT *FROM users;
```

* Hue Dashboard


## kafka Manager
- **URL** : http://localhost:9000/


## Cluster Overview
- **URL** : http://localhost:8080/


## Hbase
- **URL** : http://localhost:16010/


## Storm UI
- **URL** : http://localhost:8090/


## Jupyter
- **URL** : http://localhost:8889/


## Mongo Express
- **URL** : http://localhost:8081/


## StreamSets
- **URL** : http://localhost:18630/

**Username : admin**
**Password : admin**

---
Modified By ven2day


