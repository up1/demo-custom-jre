## How to run ?

```
$javac -d outDir --module-source-path . $(find demo.module -name "*.java")
$java --module-path outDir -m demo.module/demo.Hello
$java --list-modules
```

## Create custom JRE

```
$jlink --module-path outDir --add-modules demo.module,java.base --output custom-jre

$java -m demo.module/demo.Hello
```
