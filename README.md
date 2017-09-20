# ojdbc8
Oracle JDBC Driver for java oracle.jdbc.driver.OracleDriver ojdbc8

# How deploy to sonatype
mvn clean install

unzip .m2\repository\com\oracle\jdbc\ojdbc8\12.2.0.1\ojdbc8-12.2.0.1.jar -d .m2\repository\com\oracle\jdbc\ojdbc8\12.2.0.1\ojdbc8-12.2.0.1

cd ojdbc  (this project directory)

cp .m2\repository\com\oracle\jdbc\ojdbc8\12.2.0.1\ojdbc8-12.2.0.1\oracle target\classes\oracle

cp .m2\repository\com\oracle\jdbc\ojdbc8\12.2.0.1\ojdbc8-12.2.0.1\META-INF target\classes\META-INF

mvn deploy -Pdeploy -Dmaven.main.skip=true -Dmaven.install.skip=true  (configure your Maven setting.xml)

# How use

[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.github.noraui/ojdbc8/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.github.noraui/ojdbc8)

```xml
<dependency>
    <groupId>com.github.noraui</groupId>
    <artifactId>ojdbc8</artifactId>
    <version>12.2.0.1</version>
</dependency>
```

# License

[![license](https://img.shields.io/github/license/NoraUi/ojdbc8.svg)](https://github.com/NoraUi/ojdbc8/blob/master/LICENSE)
BSD, See LICENSE for details

# Contributors

[![GitHub contributors](https://img.shields.io/github/contributors/NoraUi/ojdbc8.svg)](https://github.com/NoraUi/ojdbc8/graphs/contributors)
[![GitHub closed pull requests](https://img.shields.io/github/issues-pr/NoraUi/ojdbc8.svg)](https://github.com/NoraUi/ojdbc8/pulls)
[![GitHub issues](https://img.shields.io/github/issues/NoraUi/ojdbc8.svg)](https://github.com/NoraUi/ojdbc8/issues)
