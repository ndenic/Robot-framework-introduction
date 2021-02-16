# Robot framework - Project setup

Before you start the installation, make sure that you already have some of the below installed.
In command line write :

```
python --version
robot --version
pip --version-
chromedriver --version
```

## Install Tools:
- [Install python 3+](https://www.python.org/downloads/)
- [Install pip](https://pip.pypa.io/en/stable/installing/)
- [Install Robot Framework](https://pypi.org/project/robotframework/)
- [Install SeleniumLibrary and WebDrivers](http://robotframework.org/SeleniumLibrary/)

## Create virtual environment for Python(robot framework)
There are many tools available for creating and managing virtual Python environments
 - The venv module, that comes shipped with Python (i.e., is part of the standard library).
 - The virtualenv module.
 - The pipenv module.
 - The anaconda module.
 
I recommend you to follow next link for instruction to create virtual environment for Robot framework.
https://michaelhallik.github.io/blog/2021/02/04/Running-Robot-Framework-in-a-virtual-environment-pt-4

## Integrated Development Environment

You can use a text editor such as Atom to write tests in Robot
- [Install Atom](https://atom.io/)

I recommend installing the following plugin if you are going to use Atom
or any other 'text editor'

```
gitlab-integration
language-robot-framework
autocomplete-robot-framework
```

We can write tests in Robot anywhere , in PyCharm and in Eclipse IDE, VSCode, etc.
Within these IDE we need to integrate some plugins as well as for Atom text editor
- [Install VSCode](https://code.visualstudio.com/download)
- [Install PyCharm](https://www.jetbrains.com/pycharm/)
- [Install Eclipse](https://www.eclipse.org/downloads/)

#### Robocorp Lab
This is special IDE only for Robot framework that adjusts the environment for us (Python , robot ...)
- [Robocorp lab](https://robocorp.com/freedevtools)

## Official documentation
- [Robot framework user guide](http://robotframework.org/robotframework/#user-guide)
- [Standard libraries](http://robotframework.org/robotframework/#standard-libraries)

## Recommendation
To make this framework easier to understand, I recommend the following tutorials and documentation 
- [Robocorp beginner course](https://robocorp.com/docs/courses/beginners-course) Short course in Robocorp lab (introduction to framework and IDE)
- [Test Automation University - Robot framework](https://testautomationu.applitools.com/robot-framework-tutorial/) Also a course that goes through the installation and writing of tests in Visual Studio.
- [Micheal Hallik blog](https://michaelhallik.github.io/tag/robotframework) I found this blog very useful for understanding the key things about robot framework and why we should use it in our project.

## Project structure
For easier project management, I suggest using the following structure when creating an automation test project in Robot framework

- Libraries (some our custom Libraries stored here)
- Sample files (sample testing files like images,documents etc.)
- Results (generated html xml results and screenshots etc)
- Setup (setup files like test suite , configurating selenium etc.)
- Tests (Tests folder where all tests are separated in Page folders where they have their robot test file and robot resource file 
  - LoginPage
      - loginTest.robot  (here we have some specific keywords for Login page and Test Cases)
      - loginResources.robot ( in resource we place selectors and store them in variables)

This is just my suggestion, there is no specific set of rules on how to write a project in a Robot framework such as Page Object Model or something like that in Java ,but it remains to us, to organize the easiest way to navigate through the project.
 ![Project structure](https://i.ibb.co/9vtsmKY/project-Structure.png)
