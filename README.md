CS15L-LabReport-4
========
  
**Log into ieng6**
  ````
    $ssh cs15lsp23nz@ieng6.ucsd.edu
  ````
 ![Image](LoginToIeng6.jpg)
  The command above log into my ieng6 account because I have generated the public and private key pair in lab. This allows me to skip the password input to the ieng6 server. Once the terminal detects the login attempt, the server will find the public key as approved. Then, my local computer will prove ownership to the corresponding private key. Therefore, I could login to ieng6 without manual authentication.

**Clone your fork of the repository from your Github account**
  ````
    $git clone git@github.com:leftPathGoat/lab7.git
  ````
 ![Image](LoginToIeng6.jpg)
  -The git command clone the repository using ssh key at `git@github.com:leftPathGoat/lab7.git`.The previous setup from lab allows me to use SSH and HTTPS.
  
**Run the tests, demonstrating that they fail**
  ````
    $cd lab7 
    $ls
    $bash test.sh
  ````
 ![Image](testFail.jpg)
 -The `$cd lab7` command change my directory to the lab7 folder. Then `$ls` shows all the files in the lab7 folder. When I run bash script `$bash test.sh`, the script compiles all the java file, and execute the jUnit test `ListExampleTest.class`. 
 -By using `$cat test.sh`, we can look at the content from `test.sh`.  
 ![Image](catTest.jpg)
  
**Edit the code file to fix the failing test**
 ![Image](vimOpen.jpg)
```
$vim ListExamples.java
```
-The command vim open the file `istExamples.java` and allows me to edit the file.
>/cha <enter>
><down> <right> <right> r 2 <enter>
>:wq <enter>
  
**Run the tests, demonstrating that they now succeed**
  
Commit and push the resulting change to your Github account (you can pick any commit message!)
For example, when you run the tests, you might want to use the up arrow or Ctrl-R to access your bash history rather than typing in the full command with classpath, etc. You might say something like this accompanying the screenshot for running the tests:

Keys pressed: <up><up><up><up><enter>, <up><up><up><up><enter> The javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java command was 4 up in the search history, so I used up arrow to access it. Then the java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ... command was 4 up in the history, so I accessed and ran it in the same way.
