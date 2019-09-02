### protobuf
---
.go
https://github.com/gogo/protobuf

.js

.java
https://github.com/protocolbuffers/protobuf


```
```

```
```

```java
// java/core/src/test/java/com/google/protobuf/Proto2SchemaTest.java

@RunWith(JUnit4.class)
public class Proto2SchemaTest extends AbstractProto2SchemaTest {
  
  @Override
  proteted Schema<Proto2Message> schema() {
    return TestSchemas.genericProto2Schema;
  }
  
  @Override
  protected void registerSchemas() {
    TestSchemas.registerGenericProto2Schemas();
  }
}
```


