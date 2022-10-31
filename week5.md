# Using the Find Command

## fd ./technical
       fd .government
       fd .biomed
       fd -tm biomed
       fd .plos
       download/plos.md
## *./technical
        * .government
        * .biomed
        * .plos
## grep "./technical" find-results.txt
        grep ".government" find-results.txt
        grep ".biomed" find-results.txt
        grep ".plos" find-results.txt
## Running Script Files
        javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
        java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore DocSearchTest
## Java is not recognizing my commands. I will go to office hours to fix this. 