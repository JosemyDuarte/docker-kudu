# **docker-kudu**
___

### Description
___

This image runs [*Apache Kudu*](https://kudu.apache.org/) included in the Cloudera CDH distribution.

You can pull it with:

    docker pull josemyd/kudu

You can also find other images based on different Apache Kudu releases, using a different tag in the following form:

    docker pull josemyd/kudu:[kudu-release]-[cdh-release]

Stop with Docker Compose:

    docker-compose up

**IMPORTANT**: You need the **ntpd** daemon running on the host. To install it:

    apt-get install ntp (Debian, Ubuntu)
    yum install ntp     (RedHat, Centos)

Once started you'll be able to access to the following UIs:

| **Kudu Web UIs**           |**URL**                    |
|:----------------------------|:--------------------------|
| *Kudu Master*               | http://localhost:8051     |
| *Kudu Tablet Server*        | http://localhost:8050     |

### Available tags

- Kudu 1.7.0 ([1.7.0-cdh5.15.1](https://github.com/josemyduarte/docker-kudu/blob/1.7.0-cdh5.15.1/Dockerfile), [latest](https://github.com/josemyduarte/docker-kudu/blob/latest/Dockerfile))

### Copyright

This image is based on the work of [Parrot Stream](https://github.com/parrot-stream/docker-kudu). With the difference that this image is smaller.