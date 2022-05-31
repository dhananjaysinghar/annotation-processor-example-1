# annotation-processors: Part 1 Maven

An example on how to use Java Annotation Processors for with **Maven**. To test the example, you will need an installed JDK 11 and Maven >= 3.

Compile the Project:

```
mvn clean install
```

During the compilation, you should see an output from the Annotation Processor like the following:

```
[INFO] found @Log at .....
```


## This is an util library , Use below dependency and plugin in pom.xml , and use @Log in class level of your class
~~~
    <dependencies>
        <dependency>
            <groupId>com.annotation.processor</groupId>
            <artifactId>annotation-processor-example-1</artifactId>
            <version>0.0.1-SNAPSHOT</version>
        </dependency>
    </dependencies>   
        
    <plugins>    
      <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-compiler-plugin</artifactId>
         <version>3.6.1</version>
         <configuration>
            <showWarnings>true</showWarnings>
         </configuration>
      </plugin>
    </plugins>  
~~~