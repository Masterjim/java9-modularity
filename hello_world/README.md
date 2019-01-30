# Java 9 Modularity Hello World
## How to compile the project
```javac -d out/helloworld src/helloworld/com/javamodularity/helloworld/HelloWorld.java src/helloworld/module-info.java```
## How to package the project
```jar -cfe mods/helloworld.jar com.javamodularity.helloworld.HelloWorld -C out/helloworld .```
## How to run the project
* The exploded module format
```java --module-path out --module helloworld/com.javamodularity.helloworld.HelloWorld```
* The module jar format
```java --module-path mods --module helloworld```
