# Jenkins

## Install
Following tools required to be installed for Jenkins to work

### 1. Java

<br><code> brew cask install caskroom/versions/java8 </code></br>

### 2. Maven
Open the terminal and type
<br><code> brew install maven </code></br>

### 3. Apache Tomcat
Download Apache Tomcat from http://tomcat.org tar.gz file
Extract it and add the bin folder to the PATH variable in .bash_profile
To test, go the bin directory and run 
<br><code> ./catalina.sh run </code></br>

Then go to the browser and connect to localhost:8080

### 4. Jenkins

<br><code> brew install jenkins </code></br>

## Post-build setup

### Unlock the Jenkins software
1. Start the jenkins server. This will run on port 8080 and you can access it using browser.
<br><code> brew services start jenkins </br></code>

2. Using the browser http://localhost:8080
   Install custom plugins, remove Ant, Gradle and Subversion
   Click on Install Plugin

3. Add JDK to the global environment variable
   http://localhost:8080 
   Login as admin username and password
   Configure -> Manage Jenkins -> Global Tool Configuration
   Add JDK, name it and add the path for JDK home. (you can find it using /usr/libexec/java_home -V)
   

