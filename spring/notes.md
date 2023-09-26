# Notes

If using regular spring-context, to force Spring to obey your logging framework (e.g. logback), make sure that you exclude the Apache Commons Logging transitive dependency.
```xml
<dependency>
  <groupId>org.springframework</groupId>
  <artifactId>spring-context</artifactId>
  <version>6.0.12</version>
  <exclusions>
    <exclusion>
      <groupId>commons-logging</groupId>
      <artifactId>commons-logging</artifactId>
    </exclusion>
  </exclusions>
</dependency>
```
