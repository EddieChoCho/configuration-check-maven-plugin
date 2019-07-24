# A Maven plugin to check your customized configuration file

### Introduction for Maven plugin

* [How to build a Maven plugin](https://dzone.com/articles/a-simple-maven-3-plugin)
* [Naming convention for customize Maven plugin](https://maven.apache.org/guides/plugin/guide-java-plugin-development.html)

### How to use this Maven plugin

* Maven Phase: A Maven phase represents a stage in the Maven build lifecycle.
* Maven Goal: Each phase is a sequence of goals, and each goal is responsible for a specific task.
* Please configure the plugin with the phase and goals. For example:

```$xslt
    <build>
        <plugins>
            <plugin>
                <groupId>eddie.com</groupId>
                <artifactId>configuration-check-maven-plugin</artifactId>
                <version>1.0-SNAPSHOT</version>
                <executions>
                    <execution>
                        <phase>compile</phase>
                        <goals>
                            <goal>check-configuration</goal>
                        </goals>
                    </execution>
                </executions>
            </plugin>
        </plugins>
    </build>
```

