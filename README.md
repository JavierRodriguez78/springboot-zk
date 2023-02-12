# springboot-zk
*Spring Boot configuration for ZK framework*

A continuación se detalla los pasos para añadir ZK en SpringBoot:

1º Añadimos el repositorio de ZK.

```xml
 <repositories>
    <repository>
        <id>ZK CE</id>
        <name>ZK CE Repository</name>
        <url>https://mavensync.zkoss.org/maven2</url>
    </repository>
 </repositories>
```
2º Añadimos la libreía para la configuración de zk en springboot denominado *zkspringboot-starter*
también le indicamos la versión de la librería puedes buscarlo [aquí](http://mavensync.zkoss.org/maven2/org/zkoss/zkspringboot/zkspringboot-starter/)
```xml
<dependency>
    <groupId>org.zkoss.zkspringboot</groupId>
    <artifactId>zkspringboot-starter</artifactId>
    <type>pom</type>
    <version>3.0.0</version>
</dependency>
```
3º Todos los recursos de las páginas se guardarán en la carpeta web dentro de resources.
4º Añadimos las págnas y la configuración dentro del application.properties
```properties
zk.homepage=hello
```
5º Ejecutamos 
```mvn
mvn install
```
6º Nos dirigimos a **localhost:8080** donde podemos ver nuestro componente.
