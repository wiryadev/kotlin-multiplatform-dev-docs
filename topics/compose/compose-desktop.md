[//]: # (title: Compose Multiplatform for desktop)

With Compose Multiplatform, you can create desktop applications for macOS, Linux, and Windows.

In this tutorial, you'll create, configure, and run a simple desktop application using Kotlin Multiplatform wizard
and the Compose Multiplatform UI framework.

## Create the project

To begin, create a sample project. This is best achieved with the Kotlin Multiplatform web wizard:

1. Open the [Kotlin Multiplatform wizard](https://kmp.jetbrains.com).
2. Select the **Desktop** option, clear the others.
3. Click the **Download** button and unpack the resulting archive.

![Kotlin Multiplatform wizard](multiplatform-web-wizard-desktop.png){width=450}

## Examine the project structure

1. Launch Android Studio.
2. On the welcome screen, click **Open** or select **File | Open** in the editor.
3. Navigate to the unpacked project folder and click **Open**.

   Android Studio detects that the folder contains a Gradle build file and opens the folder as a new project.

The project includes the _composeApp_ Kotlin module. It uses [Gradle](https://kotlinlang.org/docs/gradle.html) as the build system that helps
you automate your build process.

The module has the `desktopMain` _source set_. In Gradle, source sets group files together where each group has its own
dependencies.

![Compose Multiplatform project structure](compose-desktop-project-structure.png){width=350}

## Run your application

### In the editor

You can run the application on desktop right from the editor:

1. Go to `composeApp/src/desktopMain/kotlin`.
2. Open the `main.kt` file and find the `main()` function:

   ![Compose Multiplatform desktop app](first-compose-project-on-desktop-main.png){width=350}

3. Click the green run icon in the gutter next to the `main()` function:

   ![First Compose Multiplatform app on desktop](first-compose-project-on-desktop-1.png){width=400}

4. Click the button in the application to see how it reacts and updates the UI.

Once you run your desktop application, a new **Run Configuration** is created. You can use it from now on to run the
desktop application:

![Run Compose Multiplatform app on desktop](compose-new-run-desktop.png){width=300}

### Using Gradle tasks

Alternatively, you run your desktop app using Gradle tasks:

* In the [Gradle tool window](https://www.jetbrains.com/help/idea/jetgradle-tool-window.html), select `KotlinProject/Tasks/compose desktop/run`:

  ![Gradle run tasks for desktop](compose-gradle-run-desktop.png){width=350}

  The first run may take some time.

* You can also run Gradle tasks in the terminal:

  * `./gradlew run` to run the application
  * `./gradlew package` to store native distribution into `build/compose/binaries`

## Next steps

We encourage you to explore Compose Multiplatform further and try out more projects:

* [Create an application targeting iOS and Android with Compose Multiplatform](compose-multiplatform-getting-started.md)
* [See how to create and run tests for multiplatform projects](multiplatform-run-tests.md).
* [Learn more about the project structure](https://kotlinlang.org/docs/multiplatform-discover-project.html).