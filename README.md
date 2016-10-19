Docker container: CentOS 7 + Java 8 + Tomcat 8

## Build the image

```sh
git clone https://github.com/blav/centos-tomcat.git
cd centos-tomcat
docker build -t blav/centos-tomcat .
```

## How to use
Put your war under the `/opt/tomcat/webapps` directory.

```sh
docker run -v /opt/tomcat/webapps:/opt/tomcat/webapps -i -t --name centos-tomcat blav/centos-tomcat
```

## Versions

|Software|Version|Note|
|:-----------|:------------|:------------|
|CentOS|7||
|Java|8u102||
|Apache Tomcat|8.5.6||
