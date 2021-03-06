---

title: "Web applications"
weight: 40

menu:
  main:
    name: "Web Applications"
    identifier: "user-guide-spring-boot-webapps"
    parent: "user-guide-spring-boot-integration"

---

To enable [Web Applications]({{<relref "webapps/index.md">}}) you can use following starter in your `pom.xml`:

```xml
<dependency>
  <groupId>org.camunda.bpm.springboot</groupId>
  <artifactId>camunda-bpm-spring-boot-starter-webapp</artifactId>
  <version>{project-version}</version>
</dependency>
```

By default the starter registers a controller to redirect `/` to camundas bundled `index.html`.
To disable this you have to add to your application properties:
```properties
camunda.bpm.webapp.index-redirect-enabled=false
```