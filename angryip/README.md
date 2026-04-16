Angry IP Scanner
Fast and friendly network scanner

The source code is available on Github, and licensed under the terms of GPL v2.

You need to clone the following URL: https://github.com/angryip/ipscan.git

In order to get the source code, the following command must be run (make sure you have git installed):

git clone git://github.com/angryip/ipscan.git
This command will fetch the current source code of the program with full history into local directory named ‘ipscan’. Or just browse the code repository on Github.

If the source of particular release is required, then you can later switch to particular tag using:

git checkout tag-name
where tag-name is the released version number (eg 3.9.3), for full list of available tags use:

git tag
Building
In order to build the binaries, you need only to run ‘./gradlew’ in the ‘ipscan’ directory. Gradle will use the standard build.gradle script there and compile, test, and package the program for all platforms. Note: some packaging features were tested only on Linux.

The source code tree also includes the preconfigured Intellij IDEA project for convenience. Then, it can be run using the net.azib.ipscan.Main class.
