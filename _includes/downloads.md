<!-- Lists WireMock download options -->

* Maven
  * | "pom.xml"
    ```
    <dependency>
      <groupId>org.wiremock</groupId>
      <artifactId>wiremock</artifactId>
      <version>{{ site.wiremock_version }}</version>
      <scope>test</scope>
    </dependency>
    ```
  * see [JUnit 5](/_docs/junit-jupiter.md) or [plain Java](/_docs/java-usage.md)  
* Gradle Groovy
  * | "build.gradle"
    ```
    testImplementation "org.wiremock:wiremock:{{ site.wiremock_version }}"
    ```
  * see [JUnit 5](/_docs/junit-jupiter.md) or [plain Java](/_docs/java-usage.md)  
* Gradle Kotlin
  * | "build.gradle.kts"
    ```
    testImplementation("org.wiremock:wiremock:{{ site.wiremock_version }}")
    ```
  * see [JUnit 5](/_docs/junit-jupiter.md) or [plain Java](/_docs/java-usage.md)
* Scala SBT
  * | "build.sbt"
    ```
    libraryDependencies +=
      "org.wiremock" % "wiremock" % "{{ site.wiremock_version }}" % Test
    ```
* Standalone
  * [download latest standalone JAR](https://repo1.maven.org/maven2/org/wiremock/wiremock-standalone/X.Y.Z/wiremock-standalone-X.Y.Z.jar)
  * `java -jar wiremock-standalone-X.Y.Z.jar`
  * follow [here](/_docs/standalone/java-jar.md)
* Docker
  * `docker run -it --rm -p 8080:8080 --name wiremock wiremock/wiremock:X.Y.Z`
  * follow [here](/_docs/standalone/docker.md)
