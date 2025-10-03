# hello-java-maven
Simple Java Maven "Hello, Jenkins + Maven!" project for TASK 8 DEV.

## Files
- `src/main/java/HelloWorld.java` — simple main class that prints a message.
- `pom.xml` — Maven project file (Java 1.8 target).

## To build locally (Windows PowerShell)
1. Install JDK 8 or 11 and Maven, ensure `java` and `mvn` are on PATH.
2. Open PowerShell in the project folder and run:
   ```powershell
   mvn clean package
   ```
3. JAR will be in `target/` (example: `target/hello-1.0-SNAPSHOT.jar`).

## For Jenkins (quick steps)
1. Push this repo to GitHub.
2. In Jenkins create a Freestyle project.
3. Under "Source Code Management" add the Git repo URL.
4. Under "Build" choose "Invoke top-level Maven targets" and set `Goals` to `clean package`.
5. Run the build and check console output for `BUILD SUCCESS`.

## Purpose
This project is ready to upload to GitHub and connect to your Jenkins job for the TASK 8 DEV.
