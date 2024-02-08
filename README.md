https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#getting-started.first-application


![01.png](img/01.png)

![02.png](img/02.png)

- Maven

![03.png](img/03.png)

```xml
<parent>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-parent</artifactId>
    <version>3.2.2</version>
</parent>
```

![04.png](img/04.png)

- Starters
- https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#using.build-systems.starters

```xml
<dependencies>
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>
</dependencies>
```

![05.png](img/05.png)

---

![06.png](img/06.png)

```java
@SpringBootApplication
public class MainApplication {
    public static void main(String[] args) {
        SpringApplication.run(MainApplication.class, args);
    }
}
```

![07.png](img/07.png)

![08.png](img/08.png)

![09.png](img/09.png)

---

![10.png](img/10.png)

```java
@RestController
public class HomeController {

    @ResponseBody
    @GetMapping("/")
    public String index() {
        return "Hello World";
    }
}
```


![12.png](img/11.png)