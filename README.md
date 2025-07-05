dolick [just a fork of paper]

The most widely used, high-performance Minecraft server that aims to fix gameplay and mechanics inconsistencies.




How To (Server Admins)
------
1.21.7 dolick
Download Dolick from our [downloads page]([https://www.mediafire.com/file/o6xn46000rj0ojg/Dolick.1.21.7.jar/file]).

Run the Dolick jar directly from your server. Just like old times



```xml
<repository>
    <id>papermc</id>
    <url>https://repo.papermc.io/repository/maven-public/</url>
</repository>
```

```xml
<dependency>
    <groupId>io.papermc.paper</groupId>
    <artifactId>paper-api</artifactId>
    <version>1.21.7-R0.1-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
```
##### Gradle
```kotlin
repositories {
    maven {
        url = uri("https://repo.papermc.io/repository/maven-public/")
    }
}

dependencies {
    compileOnly("io.papermc.paper:paper-api:1.21.7-R0.1-SNAPSHOT")
}

java {
    toolchain.languageVersion.set(JavaLanguageVersion.of(21))
}
```

How To (Compiling Jar From Source)
------
To compile Paper, you need JDK 21 and an internet connection.

Clone this repo, run `./gradlew applyPatches`, then `./gradlew createMojmapBundlerJar` from your terminal. You can find the compiled jar in the `paper-server/build/libs` directory.

To get a full list of tasks, run `./gradlew tasks`.

How To (Pull Request)
------
See [Contributing](CONTRIBUTING.md)

Old Versions (1.21.3 and below)
------
For branches of versions 1.8-1.21.3, please see our [archive repository](https://github.com/PaperMC/Paper-archive).

Support Us
------
First of all, thank you for considering helping out, we really appreciate that!

PaperMC has various recurring expenses, mostly related to infrastructure. Paper uses [Open Collective](https://opencollective.com/) via the [Open Source Collective fiscal host](https://opencollective.com/opensource) to manage expenses. Open Collective allows us to be extremely transparent, so you can always see how your donations are used. You can read more about financially supporting PaperMC [on our website](https://papermc.io/sponsors).

You can find our collective [here](https://opencollective.com/papermc), or you can donate via GitHub Sponsors [here](https://github.com/sponsors/PaperMC), which will also go towards the collective.

Special Thanks To:
-------------

[![YourKit-Logo](https://www.yourkit.com/images/yklogo.png)](https://www.yourkit.com/)

[YourKit](https://www.yourkit.com/), makers of the outstanding java profiler, support open source projects of all kinds with their full featured [Java](https://www.yourkit.com/java/profiler) and [.NET](https://www.yourkit.com/.net/profiler) application profilers. We thank them for granting Paper an OSS license so that we can make our software the best it can be.

[<img src="https://user-images.githubusercontent.com/21148213/121807008-8ffc6700-cc52-11eb-96a7-2f6f260f8fda.png" alt="" width="150">](https://www.jetbrains.com)

[JetBrains](https://www.jetbrains.com/), creators of the IntelliJ IDEA, supports Paper with one of their [Open Source Licenses](https://www.jetbrains.com/opensource/). IntelliJ IDEA is the recommended IDE for working with Paper, and most of the Paper team uses it.

All our sponsors!  
[![Sponsor Image](https://raw.githubusercontent.com/PaperMC/papermc.io/data/sponsors.png)](https://papermc.io/sponsors)
