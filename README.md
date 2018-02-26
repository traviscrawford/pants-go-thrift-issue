*FIXED IN https://github.com/pantsbuild/pants/issues/5453*

# pants-go-thrift-issue
Repo to help troubleshoot using thrift with go.

```
$ ./pants binary src/go/cgo/

17:29:06 00:00 [main]
               (To run a reporting server: ./pants server)
17:29:06 00:00   [setup]
17:29:07 00:01     [parse]
               Executing tasks in goals: jvm-platform-validate -> bootstrap -> imports -> unpack-jars -> deferred-sources -> gen -> pyprep -> resolve -> resources -> compile -> binary
17:29:07 00:01   [jvm-platform-validate]
17:29:07 00:01     [jvm-platform-validate]
17:29:07 00:01   [bootstrap]
17:29:07 00:01     [substitute-aliased-targets]
17:29:07 00:01     [jar-dependency-management]
17:29:07 00:01     [bootstrap-jvm-tools]
17:29:07 00:01     [provide-tools-jar]
17:29:07 00:01   [imports]
17:29:07 00:01     [ivy-imports]
17:29:07 00:01   [unpack-jars]
17:29:07 00:01     [unpack-jars]
17:29:07 00:01   [deferred-sources]
17:29:07 00:01     [deferred-sources]
17:29:07 00:01   [gen]
17:29:07 00:01     [antlr-java]
17:29:07 00:01     [antlr-py]
17:29:07 00:01     [jaxb]
17:29:07 00:01     [protoc]
17:29:07 00:01     [ragel]
17:29:07 00:01     [thrift-java]
17:29:07 00:01     [thrift-py]
17:29:07 00:01     [wire]
17:29:07 00:01     [go-thrift]
17:29:07 00:01       [execute]
17:29:07 00:01   [complete]
               FAILURE
Exception caught: (<type 'exceptions.AttributeError'>)

Exception message: 'NoneType' object has no attribute 'rsplit'
```
