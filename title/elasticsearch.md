---
description: install elasticSearch
---

# Install ElasticSearch

## Add user

show users

```
$ cut -d: -f1 /etc/passwd
```

add user

```text
$ adduser  essearch
```

password user

```text
passwd  essearch
```



delete user

```text
userdel  essearch
```

login user

```text
su essearch
```

Install ES 

[https://www.elastic.co/guide/en/elasticsearch/reference/current/targz.html](https://www.elastic.co/guide/en/elasticsearch/reference/current/targz.html)

```text
wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-7.8.1-linux-x86_64.tar.gz
wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-7.8.1-linux-x86_64.tar.gz.sha512
shasum -a 512 -c elasticsearch-7.8.1-linux-x86_64.tar.gz.sha512 
tar -xzf elasticsearch-7.8.1-linux-x86_64.tar.gz
cd elasticsearch-7.8.1/
./bin/elasticsearch
```

Testing

```text
curl 'http://localhost:9200/?pretty'
```

