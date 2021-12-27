# AetherialMist Logging

[![](https://jitpack.io/v/AetherialMist/Log4jLogging.svg)](https://jitpack.io/#AetherialMist/Log4jLogging)


Basic logging support using Log4j2

Designed to look similar to Spring Boot without actually using Spring Boot

## How to include in your project

Add the following to your POM

```xml
<project>
    <repositories>
        <!-- Pull GitHub releases as a dependency -->
        <repository>
            <id>jitpack.io</id>
            <url>https://jitpack.io</url>
        </repository>
    </repositories>
    
    <dependencies>
        <!-- Basic Logging Support -->
        <dependency>
            <groupId>com.github.AetherialMist</groupId>
            <artifactId>Log4jLogging</artifactId>
            <version>RELEASE_VERSION</version>
        </dependency>
    </dependencies>
</project>
```

---

IMPORTANT

You may need to include `-Dlog4j.skipJansi=false` as a VM option.

---

Recommended to use with Lombok

```xml
<project>
    <dependencies>
        <!-- https://mvnrepository.com/artifact/org.projectlombok/lombok -->
        <!-- Use the '@Slf4j' annotation on the class to auto-generate the Logger 'log' -->
        <dependency>
            <groupId>org.projectlombok</groupId>
            <artifactId>lombok</artifactId>
            <version>1.18.22</version>
            <!-- <version>OR_NEWER_VERSION</version> -->
            <scope>provided</scope>
        </dependency>
    </dependencies>
</project>
```