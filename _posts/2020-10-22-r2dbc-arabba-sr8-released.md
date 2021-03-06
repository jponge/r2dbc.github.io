---
layout: post
title:  "R2DBC Arabba-SR8 released"
date:   2020-10-22 17:15:00 +0200
tags: [release]
author: Mark Paluch
---

On behalf of the community and everyone who contributed, we're delighted to announce availability of R2DBC `Arabba-SR8` available from Maven Central!

This service release ships the following modules:

* [R2DBC MariaDB connector - 0.8.4-rc](https://github.com/mariadb-corporation/mariadb-connector-r2dbc/releases/tag/0.8.4) (`org.mariadb:r2dbc-mariadb`)
* [R2DBC SQL Server driver - 0.8.5.RELEASE](https://github.com/r2dbc/r2dbc-mssql/milestone/11?closed=1) (`io.r2dbc:r2dbc-mssql`)
* [R2DBC PostgreSQL driver - 0.8.6.RELEASE](https://github.com/pgjdbc/r2dbc-postgresql/milestone/15?closed=1)  (`io.r2dbc:r2dbc-postgresql`)
* [R2DBC Pool - 0.8.5.RELEASE](https://github.com/r2dbc/r2dbc-pool/milestone/10?closed=1) (`io.r2dbc:r2dbc-pool`)
* [R2DBC Proxy - 0.8.5.RELEASE](https://github.com/r2dbc/r2dbc-proxy/milestone/8?closed=1)  (`io.r2dbc:r2dbc-proxy`)

This is a maintenance release shipping with mostly bugfixes fixes, selected enhancements, and dependency upgrades. Check out the changelogs associated with each component.

We recommend version management by using R2DBC BOM as individual modules follow their own version number schedule.

If you use Maven, you can add the following lines to your `pom.xml`:

```xml
<dependencyManagement>
  <dependencies>
    <dependency>
      <groupId>io.r2dbc</groupId>
      <artifactId>r2dbc-bom</artifactId>
      <version>Arabba-SR8</version>
      <type>pom</type>
      <scope>import</scope>
    </dependency>
  </dependencies>
</dependencyManagement>

<dependencies>
  <dependency>
    <groupId>org.mariadb</groupId>
    <artifactId>r2dbc-mariadb</artifactId>
  </dependency>
</dependencies>
```
