
# Basic commands 

  start sbt shell 
    => sbt
 
  compile a project 
    => compile

  start continuous compilation 
    => ~compile
 
  get help in the console 
    => help

  get specific help 
    => help <command>
 
  run program ( continuous ~ ) 
    => run
 
  set Scala version from the shell 
    => set ThisBuild / scalaVersion := "2.12.7"

  get Scala version 
    => scalaVersion
 
  reload the build 
    => rebuild

  name the project: 
      ThisBuild / scalaVersion := "2.12.7"
      ThisBuild / organization := "com.example"

      lazy val hello = (project in file("."))
      .settings(
        name := "Hello"
      )

   save set given in a sbt session 
     => save session




