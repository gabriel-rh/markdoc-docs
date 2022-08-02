# Code


{% sidebyside %}

{% item %}

~~~
```yaml
    commands:
    - id: build
        exec:
            component: mysql
            commandLine: mvn clean
            workingDir: /projects/spring-petclinic
```
~~~

{% /item %}

{% item %}

```yaml
    commands:
    - id: build
        exec:
        component: mysql
        commandLine: mvn clean
        workingDir: /projects/spring-petclinic
```

{% /item %}

{% /sidebyside %}
