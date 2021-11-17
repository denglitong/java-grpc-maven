# Grpc Java demo

## 生成/更新protobuf文件

    mvn clean package

## 编译运行

编译

    mvn clean compile

启动server:
    
    mvn exec:java -Dexec.mainClass="com.example.myproject.grpc.HelloServer"

启动client:

    mvn exec:java -Dexec.mainClass="com.example.myproject.grpc.HelloClient"

