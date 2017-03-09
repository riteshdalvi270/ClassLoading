# ClassLoading
Class loading using java

Compile:
javac -d classes fileName (src/main/java/helper/Helper.java) : moves the class file Helper.class under /classes

javac -cp classes/ src/main/java/helper/Main.java (gives the classpath to find Helper class)


Run:

1. java application.Main (you have to be directory above application in classes folder) [You always run class files in java]

Set the classpath using
Main.class lies under the same folder, where other classes lies
1. set CLASSPATH=classes -- Global class path (not prefered, might affect other java application)

If you Main.class lies somewhere else
1. java -cp classes/ application.Main

Jar file
1. jar cvf helper.jar classes/helper/Helper.class
2. java -cp classes;helper.jar application.Main
