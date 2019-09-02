### protobuf
---
.go
https://github.com/gogo/protobuf

.js

.java
https://github.com/protocolbuffers/protobuf


```go
// test/sizeunderscore/sizeunderscore.proto

syntax = "proto2";
package sizeunderscore;

import "github.com/gogo/protobuf/gogoproto/gogo.proto";

option (gogoproto.marshaler_all) = true;
option (gogoproto.sizer_all) = true;
option (gogoproto.unmarshaler_all) = true;
option (gogoproto.populate_all) = true;
option (gogoproto.testgen-all) = true;
option (gogoproto.equal_all) = true;

message SizeMessage {
  optional int64 size = 1;
  optional bool Equal = 2;
  optional string String = 3;
}
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


