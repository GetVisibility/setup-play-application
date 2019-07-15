# Setup Play Application
Instructions for setting up a Scala development environment with the [Play Framework](https://www.playframework.com/) and an IDE.

---

## Building the starter project 
1. Install a Java Development Kit (JDK) from [Oracle](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (this is a link to Java 8, but you can install anything up to 11)
2. Install the Scala Built Tools (SBT), instructions for Mac, Linux and Window can be found [here](https://www.scala-sbt.org/release/docs/Setup.html)
3. Open a terminal/command prompt in the location you want to create your project.
4. Run the following command `sbt new playframework/play-scala-seed.g8` This instruction can be found on the play framework [getting started](https://www.playframework.com/getting-started) site.
5. Navigate to the top level directory of the project. (the one with **build.sbt**) In the case of the example this is play-scala-seed.
6. Run `sbt run` and open a browser and navigate to [localhost:9000](http://localhost:9000/)
7. If everything works, you should see a **Welcome to Play!** message.

---

## Working with the IntelliJ IDE
1. Download the Intellij community edition (free) IDE for your operating system. Instructions can be found on the jetbrains website [here](https://www.jetbrains.com/idea/)

2. Open the preferences and install the scala plugin (screenshot below)

![screenshot of scala-plugin](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/scala-plugin.png)

3. Click on File > Open... and navigate to the project folder. Click on the **build.sbt** file and then open. You will be given 3 options:

![screenshot of open-project](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/open-project.png)

4. Choose Open as Project (this is critical to get the IDE to recognise this as a Scala project and have intelli-sense work correctly)

5. You will be given an option to Import Project from sbt. Leave the options at default and click OK.

![screenshot of import-project](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/import-project.png)

6. At the top of the IDE there is an option to Add Configuration (this is for building and running).

![screenshot of add-configuration](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/add-configuration.png)

7. Click the **+** symbol and choose **sbt Task** from the list.

![screenshot of add-sbt-task](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/add-sbt-task.png)

8. For the **Name:** and **Tasks:** type in `run`

![screenshot of configure-sbt-task](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/configure-sbt-task.png)

9. You can now click on the play button to run the application from the IDE.

![screenshot of run-application](https://github.com/GetVisibility/setup-play-application/raw/master/images/idea/run-application.png)
