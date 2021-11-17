# Grpc Java demo

## 项目结构

    ├── pom.xml
    ├── src
    │   ├── main
    │   │   ├── java
    │   │   │   └── com
    │   │   │       └── example
    │   │   │           └── myproject
    │   │   │               ├── gencode
    │   │   │               │   └── helloworld
    │   │   │               │       ├── HelloRequest.java
    │   │   │               │       ├── HelloRequestOrBuilder.java
    │   │   │               │       ├── HelloResponse.java
    │   │   │               │       ├── HelloResponseOrBuilder.java
    │   │   │               │       ├── HelloServiceGrpc.java
    │   │   │               │       └── HelloServiceOuterClass.java
    │   │   │               └── grpc
    │   │   │                   ├── HelloClient.java
    │   │   │                   ├── HelloServer.java
    │   │   │                   └── HelloServiceImpl.java
    │   │   ├── proto
    │   │   │   └── HelloService.proto

## 生成/更新protobuf文件

    mvn clean package

## 编译运行

编译

    mvn clean compile

启动server:
    
    mvn exec:java -Dexec.mainClass="com.example.myproject.grpc.HelloServer"

启动client:

    mvn exec:java -Dexec.mainClass="com.example.myproject.grpc.HelloClient"

