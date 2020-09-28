# bigdatawithscala

install scala in ubuntu 16.4

# Scala
sudo apt-get remove scala-library scala
sudo wget http://scala-lang.org/files/archive/scala-2.12.1.deb
sudo dpkg -i scala-2.12.1.deb
sudo apt-get update
sudo apt-get install scala

# SBT
echo "deb https://dl.bintray.com/sbt/debian /" | sudo tee -a /etc/apt/sources.list.d/sbt.list
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2EE0EA64E40A89B84B2DF73499E82A75642AC823
sudo apt-get update
sudo apt-get install sbt



1) JDK 8 or newer (latest stable version is 10)
2) Scala
3) SBT - it is the build-tool
4) git clone 

SBT

# show all sub-projects
sbt> projects

# switch to a sub-project
sbt> project <name of sub-project>

# compile
sbt> compile

# compile on every file change
sbt> ~compile

# run test
sbt> test

# run a certain test
sbt> test:testOnly <name of test>
  
  Build the project

To build a project go through the following steps:

$> cd /path/to/repo
$> sbt
# select one of the project
sbt> projects
sbt> project <project name>

# minimum JS optimizations
sbt> fastCompile

# maximum JS optimizations (Github page)
sbt> fullCompile
sbt> exit

# opens project in the default browser
$> open project_name/index.html
