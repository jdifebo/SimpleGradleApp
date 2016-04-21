**Hello Simple Gradle**

The simplest Gradle+Java app that you can make.  We apply the ```application``` plugin, which implicitly
 applies the ```java``` plugin in our ```build.gradle``` file, and this allows us to build Java projects without dependencies, as long as they
use the default settings.  In other words, we want our source files to be in src/main/java.

There is one source file, ```HelloSimpleGradle.java```.  We can run our main method two different ways:
1. Use ```gradle run```.  This utilizes our ```application``` plugin, which builds
the code and then runs the class specified in the build file.
2. First build the project with ```gradle build``` and then run the jar file like you would normally:```java -cp build/libs/SimpleGradleApp.jar HelloSimpleGradle```



```
Hello Simple Gradle!
```

You can also import this project into Intellij IDEA or Eclipse, although with Eclipse you'll need a gradle plugin to do
so.  But if you use the plugin within Eclipse, then you won't need to worry about using the eclipse plugin in your
```build.gradle``` file.