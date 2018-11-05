# Testing_AKKA_on_Evosuite
We attempt to produce AKKA tests automatically using evosuite
On ubuntu, get into the project directory (Testing_AKKA_on_Evosuite) and run the following commands:
1: -$ export EVOSUITE="java -jar $(pwd)/evosuite-1.0.6.jar"
2: -$  $EVOSUITE -prefix com.lightbend.akka.sample -projectCP target/classes:library_dependencies/akka-actor_2.12-2.5.12.jar:library_dependencies/akka-testkit_2.12-2.5.12.jar:library_dependencies/config-1.3.2.jar:library_dependencies/scala-java8-compat_2.12-0.8.0.jar:library_dependencies/scala-library-2.12.5.jar
The commands should generate test suites for the AKKA project. The application merely has AKKA actors sending greetings to each other in a distrubted setting
