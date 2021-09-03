# Project 0
Due: 09/10, 11:59pm EST (Late 09/13, 09/17)
Survey Soft Deadline: 09/07, 11:59pm

## Class Survey

Take the class survey to give us your information and class preferences [here](https://forms.gle/ZEkNzA9qPKvHWQRp6). You must be signed in to your terpmail email to access the link AND provide your FULL NAME (First and Last) to receive credit for this. Submit this survey ASAP (we will need the information to add you to your team).

## Team Formation

Sign up for a team on [this google sheet](https://docs.google.com/spreadsheets/d/1Vpk3ItHD1IkxlZtybxKcOvl4k_ZeH98llw5K6LoltDs/edit?usp=sharing). You must be signed in to your terpmail email to access the link AND provide your FULL NAME (First and Last) to receive credit for this.
Your assigned TA will add you to your team on Github. 

## Set Up Your Local Git Environment
Once you have been added to your team on Github, take the following steps to set up your Local Git Environment in your command line:

1. Generate your ssh-keys with ```ssh-keygen```
2. Configure your local environment with your name and email
      - ```git config --global user.name "your_name_here"```
      - ```git config --global user.email your_email_here```
3. Add your ssh-keys to your GitHub account 
4. Clone your repository using ssh ```git clone git@...```

If you don't already have git installed on your command line, follow the directions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

Once you have cloned the remote repository, checkout the setup branch

```bash
git checkout setup
git pull
```

edit the main README and add your name as one of the lines. Then add, commit, and push your changes:

```bash
git add README.md
git commit -m "your_name git setup"
git push -u origin setup
```

## Checking Your Java Installation

Once you have cloned the repository, test your Java installation:

If you don't already already have java installed, you can install it through [OpenJDK](https://openjdk.java.net/install/).

```bash
cd path_to_repo/Projects/P0
javac HelloWorld.java
java HelloWorld
```

We will also be using JUnit Tests in this class. Run the following commands to test that you can run and compile JUnit tests:

```bash
cd path_to_repo/Projects/P0
javac -cp "junit-4.10.jar:." TestHelloWorld.java 
java -cp "junit-4.10.jar:." org.junit.runner.JUnitCore TestHelloWorld
```

If you are using a Windows machine, you may need to modify the classpath to use semicolons instead of colons:

```
cd path_to_repo\Projects\P0
javac -cp "junit-4.10.jar;." TestHelloWorld.java
java -cp "junit-4.10.jar;." org.junit.runner.JUnitCore TestHelloWorld
```

On ELMS, submit the output of the TestHelloWorld JUnit test.

## Academic Integrity

Please **carefully read** the academic honesty section of the course syllabus. **Any evidence** of impermissible cooperation on projects, use of disallowed materials or resources, or unauthorized use of computer accounts, **will be** submitted to the Student Honor Council, which could result in an XF for the course, or suspension or expulsion from the University. Be sure you understand what you are and what you are not permitted to do in regards to academic integrity when it comes to project assignments. These policies apply to all students, and the Student Honor Council does not consider lack of knowledge of the policies to be a defense for violating them. Full information is found in the course syllabus, which you should review before starting.
