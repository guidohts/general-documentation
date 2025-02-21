# Setup Java Development Environment

You have various options to create a new dev environment on yout machine.

At first, create a folder to contain all new projects in the future.

If you are on Mac, you may create a folder in your home directory, e.g. `/Users/school/src`.

On Windows, you may create a folder like `c:\users\school\src`.

If you want to work on an USB drive, you can use it. You may create a folder on the USB drive or just use the root folder.

## Setup a New Project With Eclipse

If you start Eclips you are asked to specify a workplace folder. Please specify the folder created in the step before, e.g. `/Users/school/src` or `c:\users\school\src`.

If Eclipse was previously open with another workplace, then use File -> Switch Workplace.

Now, when you get a new task to work on, create a new Java project for every task you work on. If you want
to create HelloWorld, the go to the package explorer, right click and create a new Java Project!

As "project name" specify `HelloWorld`! Leave the other settings with their defaults!

Now, your project should have a `src` folder.

Next step, is to create a package in the `src` folder. Right click on the `src` folder and add a package.
The package name should be all lowercase characters and it may contains dots. E.g. you could create a package `de.hts.helloworld`.

Now, right click on the package and create a new class. The name should start with an uppercase letter. E.g. you could name the class `App`. Before you click Finish, check the option to create the `public static void main(String[] args)`! If you need to add a second class, there is no more `public static void main(String[] args)` in the additional classes needed, since the is only one class in the project, that should be started.

Do not include other tasks you work on in this project. Just create a new project in your workspace!

## Setup a New Project With JetBrains IDE

T.B.D.

## Setup a New Project Without any IDE

Create a new folder to contain the project.
  - Go to your workplace folder, e.g. `/Users/school/src` or `c:\users\school\src`.
  - Create folders for the new project, e.g. `mkdir -p HelloWorld/src/de/hts/helloworld` on Mac. If you work on Windows you need to create each folder one after another. Also create a folder `HelloWorld/bin`.
  - Create a text file `App.java` in this folder and add your content:

```
package de.hts.helloworld;

public class App {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

	}

}
```

To compile the class, run inside `/Users/school/src/HelloWorld`

    javac -d bin src/de/hts/helloworld/App.java

After this, you should have a file `bin/de/hts/helloworld/App.class`.

Now, you could run your compiled class file inside `/Users/school/src/HelloWorld`:

    java -cp bin de.hts.helloworld.App

or

    java -cp bin de/hts/helloworld/App










