# ![](01_docs/logo_48x48.png) IBPM Mercury DB (HgDB) for Docker

> IBPM Mercury DB (HgDB) is a service server (SOAP and REST) that allows you to manage any objects, also called cases. Its engine is based on the relational SQL model (data is stored in a relational database). The combination of objects and relationships allows you to use Mercury DB as an object database supporting ACID (Atomicity, Consistency, Isolation, Durability) transactions as well as integrating it with traditional BI (Business Intelligence) systems for business data analysis. It connects the world of NoSQL databases (such as ElasticSearch, Mongo DB) with the world of relational databases (Oracle, DB2, PostgreSQL, MySQL). The commercial version of the server is distributed by  IBPM. The website was created to promote awareness of the solution among mobile and web application developers. The articles will include API descriptions, good practices of using the system and news, development plans and interesting facts related to the implementation of both the server and its clients.

| Project name | Akronym | Last version | Code inspection | 
|--------------|--------------|--------------|--------------|
| Mercury DB (HgDB) 3.0 | HgDB | 3.0.3.2.11 | ![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=io.hgdb%3Amercury&metric=alert_status) | 

:point_right: IBPM Mercury DB (HgDB) was created out of the need to effectively register, search, compare and audit data that is used during the operation of process applications in the company.

:point_right: IBPM Mercury DB (HgDB) can act as a data repository for process applications (in particular IBM Business Process Manager ), a repository independent of the systems existing in the organization, a unified data repository for applications internally created in the organization (e.g. when we want to manage any data, we do not have a dedicated system and we create a solution within the organization, and we want the data to be safe and stored in a uniform manner for each application). 

:point_right: IBPM Mercury DB (HgDB) is applicable wherever the data model changes dynamically as a result of application development. It provides constant access to data in all implemented models. It does not require data migration to new versions of data storage structures. The engine for identifying the types of stored objects performs the task of building ontologies, creates their new versions and links between them. The ability to define alternative field nomenclature allows you to create universal relationships between data from different systems.

:point_right: IBPM Mercury DB (HgDB) data repository stores metadata about the types of objects as well as the method of their presentation on  web forms and mobile applications. Therefore, it is an ideal solution for the implementation of the mechanisms of their automatic generation, dynamic presentation of data to the end user.

:point_right: More about project and product you can read on [Mercury DB (HgDB) 3.0](https://hgdb-org.translate.goog/?_x_tr_sl=pl&_x_tr_tl=en&_x_tr_hl=pl&_x_tr_pto=wapp) page.

## Prerequisites

- Installed Docker Engine
- Installed Docker Compose

### Docker Engine

[Docker Engine](https://docs.docker.com/engine/) is an open source containerization technology for building and containerizing your applications. Docker Engine acts as a client-server application with:

- A server with a long-running daemon process dockerd.
- APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon.
- A command line interface (CLI) client docker.

The CLI uses Docker APIs to control or interact with the Docker daemon through scripting or direct CLI commands. Many other Docker applications use the underlying API and CLI. The daemon creates and manage Docker objects, such as images, containers, networks, and volumes.

Go to [Docker Engine installation overview](https://docs.docker.com/engine/install/) page to learn how to install it on various system platforms.

### Docker Compose

[Compose](https://docs.docker.com/compose/) is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration.

Go to [Docker Compose installation overview](https://docs.docker.com/compose/install/) page to learn how to install it on various system platforms.


## Download images from dockerhub

The composition consists of the following images:
- the [PostgreSQL](https://hub.docker.com/repository/docker/ibpm/postgres) container.
```
docker push ibpm/postgres:mercury-hgdb-3.0
```
- the [Apache ActiveMQ](https://hub.docker.com/repository/docker/ibpm/activemq) container.
```
docker push ibpm/activemq:mercury-hgdb-3.0
```
- the [OpenLDAP](https://hub.docker.com/repository/docker/ibpm/openldap) container.
```
docker push ibpm/openldap:mercury-hgdb-3.0
```
- the [Iron - POI Excel Serwer](https://hub.docker.com/repository/docker/ibpm/poi-server) container.
```
docker push ibpm/poi-server:mercury-hgdb-3.0
```
- the [Clustered Cache](https://hub.docker.com/repository/docker/ibpm/ehcache) container.
```
docker push ibpm/ehcache:mercury-hgdb-3.0
```
- the [IBPM Mercury (HgDB)](https://hub.docker.com/repository/docker/ibpm/mercury) container.
```
docker push ibpm/mercury:mercury-hgdb-3.0.3.2.11
```
- the [IBPM Mercury (HgDB) LoadBalancer](https://hub.docker.com/repository/docker/ibpm/mercury-lb) container.
```
docker push ibpm/mercury-lb:mercury-hgdb-3.0
```

## Up docker compose


## License types

## License key request





