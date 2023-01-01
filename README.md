# 🏦 SmartContract RestAPI project using Spring Boot and web3j

## Initial Project
### Create prj
> [Project URL](https://start.spring.io/#!type=gradle-project&language=java&platformVersion=3.0.1&packaging=jar&jvmVersion=17&groupId=com.hibuz.ethereum&artifactId=contract&name=contract&description=SmartContract%20RestAPI%20project%20using%20Spring%20Boot%20and%20web3j&packageName=com.hibuz.ethereum.contract&dependencies=web,lombok)

### Add additional depenancy
```groovy
dependencies {
	implementation 'org.springframework.boot:spring-boot-starter-web'
	implementation 'org.springdoc:springdoc-openapi-starter-webmvc-ui:2.0.2'
	implementation 'org.web3j:core:4.9.5'
	compileOnly 'org.projectlombok:lombok'
	annotationProcessor 'org.projectlombok:lombok'
	testImplementation 'org.springframework.boot:spring-boot-starter-test'
}
```


## Building for production

### Packaging as jar

To build the final jar and optimize the example application for production, run:

```
./gradlew clean bootJar
```

To ensure everything worked, run:

```
java -jar build/libs/*.jar
```

Then navigate to http://localhost:8080/swagger-ui/index.html in your browser.
