# Lab 01: Hello World

Java basics lesson using a Paper Minecraft plugin. The plugin sends `Hello World!` to the player each time they join.

## Requirements

- JDK 25
- VS Code with Microsoft's Extension Pack for Java
- Git
- Paper 1.21.11 running with Java 25
- Minecraft Java Edition 1.21.11

The project includes Maven Wrapper; a separate Maven installation is not required. Internet access is needed for the first build to download dependencies.

## Open the project

```powershell
git clone https://github.com/gumidnight/lab-01-hello-world.git
cd lab-01-hello-world
code .
```

Check `java -version` and `javac -version` report Java 25. Open the whole repository folder in VS Code.

## Build on Windows

```powershell
.\build-plugin.bat
```

The resulting plugin is `target/HelloWorld-1.0.1.jar`. For Maven diagnostic output, use `.\mvnw.cmd package`.

Stop your local Paper server, copy the JAR into its `plugins` folder, then start the server and join to see the greeting. After a code change, save, build, replace the JAR while the server is stopped, restart, and reconnect.

The Maven artifact version is 1.0.1; the plugin metadata in `plugin.yml` is 1.0.0. The existing tested source and build files are preserved unchanged.