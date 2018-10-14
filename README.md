# sonar-cobertura-plugin

[![pipeline status](https://gitlab.com/raatiniemi/sonar-cobertura-plugin/badges/master/pipeline.svg)](https://gitlab.com/raatiniemi/sonar-cobertura-plugin/commits/master)
[![quality gate](https://sonarcloud.io/api/project_badges/measure?project=me.raatiniemi.sonar%3Acobertura&metric=alert_status)](https://sonarcloud.io/dashboard?id=me.raatiniemi.sonar%3Acobertura)
[![code test coverage](https://sonarcloud.io/api/project_badges/measure?project=me.raatiniemi.sonar%3Acobertura&metric=coverage)](https://sonarcloud.io/dashboard?id=me.raatiniemi.sonar%3Acobertura)
[![technical dept](https://sonarcloud.io/api/project_badges/measure?project=me.raatiniemi.sonar%3Acobertura&metric=sqale_index)](https://sonarcloud.io/dashboard?id=me.raatiniemi.sonar%3Acobertura)

The repository is a SonarQube plugin for parsing reports from [cobertura](http://cobertura.github.io/cobertura/).
*This is not a standalone plugin yet, i.e. it needs to be [embedded within another plugin](https://gitlab.com/raatiniemi/sonar-objective-c).*

## Usage

In order to include the code from this repository, you'll first need to add the
repository.

```gradle
repositories {
    maven {
        url  "https://dl.bintray.com/raatiniemi/maven"
    }
}
```

And, then you need to declare it as a dependency using `compile 'me.raatiniemi.sonar:cobertura:$latestVersion'`.

*Dependency examples are using Gradle, for additional dependency options you can
checkout [sonar-cobertura-plugin at bintray](https://bintray.com/raatiniemi/maven/sonar-cobertura-plugin).*
