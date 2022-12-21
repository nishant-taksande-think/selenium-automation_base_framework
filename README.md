# selenium-automation_base_framework

This framework is developed in order to provide the features of selenium webdriver to the user with simplicity. Framework is organised and comprehensive.
It follows the page object model and is compatible with java language. 
The structure is divided properly:
* Library package - This package contains the important classes like App library, Test base and Configuration.
* PageObject package - This package consists of the page object classes i.e for each web page there will be one class.
* Test package - This package will contain all the test classes.


To get a better understanding of the workflow and architecture, Refer the below links :

**Framework Architecture:**

<img width="435" alt="Framework_Archi" src="https://user-images.githubusercontent.com/119481896/208860540-13da9d72-5385-4637-ae5e-993b5f4acd1f.png">

**Framework Workflow:**

<img width="522" alt="workflow" src="https://user-images.githubusercontent.com/119481896/208861064-f087f484-4fe9-4a41-bd72-ca18f16337ac.png">


## Installation
Before setting up the workspace we must first download the git for your respective Operating System if you don't already have it.

Execute this `git --version` in your respective Bash/Command Prompt to validate the existence of git on the local system.

https://docs.google.com/document/d/1zawm7Dkn8Gw1zhXyS8l1IJYSavow6UAJOlnmTbybYaU/edit?usp=sharing


## Setting the workspace

Before directly taking the repository clone anywhere on your file system follow the good practice of creating a separate directory for this project.

```bash
# Commands are the same irrespective of Operating System.

mkdir seleniumBaseFramework
cd seleniumBaseFramework
``

## SSH key setup
There are 2 ways by which you can clone this repository:

    1. Using Http 
    2. Using Ssh
But in Ssh, you don't have to write the passphrase every time and is much more secure compared to HTTP.

GitLab and SSH keys:
https://docs.gitlab.com/ee/ssh/index.html#generate-an-ssh-key-pair

Execute this:
```bash
cat *.pub 
```
And copy the contents.

Inside GitLab click on Profile --> Setting --> SSH Keys (Present on Left Panel), by default no ssh key exists there, so we need to add one.
Paste the content of the .pub file inside the text area and click add key.

After this just clone the repository inside the seleniumBaseFramework directory.
``` bash
git clone <ssh of the repository>
```

But to be able to execute git commands like add, commit, push, etc we must need to set up the email and username. And for this execute
:
```bash
git config --global user.email "testemail@test.com"
git config --global user.name "Test Name"

```

Now we are ready to execute any git command.

## IDE Configuration

**Eclipse**

Download and install Eclipse from [here](https://www.eclipse.org/downloads/).

Eclipse plugins:
    1. TestNG
    2. Git(Installed by default in eclipse version 4.21.0 and after).


**TestNG Installation**

    1. Java 1.7+ is required for running the TestNG for Eclipse plugin.
    2. Eclipse 4.2 and above is required. Eclipse 3.x is NOT supported any more.
    3. You can use either the Eclipse Marketplace or the update site.
    * Eclipse Marketplace: Go to the TestNG page on the Eclipse Marketplace and drag the icon called "Install" onto your workspace.
    * Update site: Select Help / Install New Software Enter the update site URL in "Work with:" field: https://testng.org/testng-eclipse-update-site. Make sure the check box next to the URL is checked and click Next. Eclipse will then guide you through the process.


## Import Project into Eclipse

Since this is a Gradle project we need to use Import as Gradle.

* On the top menu bar go to File --> Import.
* Then select **Existing Gradle Project**.
* And choose the project location and click Finish.

The eclipse will then take some time to build the project.

Now we are ready to make changes, edit the code and execute the existing scripts.

## Debug and Run Tests

* To run test in eclipse go to test.java  right click and select Run As --> TestNG Test.
* To debug test in eclipse right click on test.java and select Debug As --> TestNG Test.

## Run TestNG.xml 

* To run test in eclipse go to  right click and select Run As --> TestNG Suite.


