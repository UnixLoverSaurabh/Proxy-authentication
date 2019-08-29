### Method 1
In the Ubuntu 16.04 and later default repositories JavaFX is packaged as a separate package named openjfx. To install it in Ubuntu 18.04, open the terminal and type:

`sudo apt install openjdk-8-jdk openjfx`


### Method 2
Step 1:
  Download latest jdk from oracle (Linux x64)
  https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

Step 2:
  Extract downloaded tar.gz in /usr/java/
  e.g /usr/java/java/jdk1.8.0_221/
  
Step 3:
  Launch your favourite ide https://www.jetbrains.com/idea/download/
  The ide will automatically detect path.
  If not then :
      For IntelliJ idea
          File --> Project Structure --> Project --> new Project SDK
          Give the path /usr/java/java/jdk1.8.0_221/
          
          
 ### Doing this both java and javafx will work fine
