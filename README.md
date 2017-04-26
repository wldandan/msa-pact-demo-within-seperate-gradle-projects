## 基于Pact构建的契约测试

#### 简介

* order-consumer作为消费者，使用order-service提供的数据
* order-service作为提供者，提供数据给order-consumer

#### 使用Pact，先生成Pact的契约文件
```
$  cd order-consumer
$  ./gradlew test
```

#### 使用Pact的契约文件，验证提供者

```
$ cd order-service
$ ./run_pact_verify.sh
```

