# docker-android
[![Apache 2.0 License](https://img.shields.io/badge/license-Apache%202.0-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0.html)

Docker image for Android builds.

## Base Image

It use CentOS 7 as default base image. But you have another choice base on Ubuntu 14.04. [ubuntu/Dockerfile](ubuntu/Dockerfile).

## What's Included

- Oracle Java 8
- Android SDK
 - Build Tools 23.0.3 & 24.0.3
 - Platform SDK 23 & 24
- Pre-installed Gradle version 3.1

## Usage

You can pull the image form DaoCloud's image repository by using `docker pull` or [`dao pull`](https://dashboard.daocloud.io/mirror).

```sh
docker pull daocloud.io/nekocode/docker-android:<lastest-verion>
dao pull daocloud.io/nekocode/docker-android:<lastest-verion>
```

You can get the `<lastest-verion>` [here](https://dashboard.daocloud.io/packages/4c0f5468-9623-4ffb-8dd2-e2680ba9ab9d).

In CI enviroment, you can use `gradle app:assembleRelease` instead of `./gradlew app:assembleRelease` to speed up your build.