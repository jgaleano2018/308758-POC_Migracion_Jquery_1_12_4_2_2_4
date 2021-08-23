# Introduction 

NewUX is a project for the digital transformation of Avianca. 

# Getting Started
This project is based on AEM, so you have to do a few of installations and configurations before to start:
1.	Installation process
2.	Software dependencies
3.	Latest releases
4.	API references

# Installation Process

You have to dowload and install the next packages:

1. Download [Java JDK 1.8 (o mayor)](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

2. Configuration of environment variables: 

For Windows:
Go to menu and search: `Edit the system environment variables`, click on `environment variables` and add `JAVA_HOME` with the path `C:\Program Files\Java\jdk1.8.0_171`(Be sure to validate the installation path of the JDK)
For more info visit:  [Config JAVA_HOME](https://www.mkyong.com/java/how-to-set-java_home-on-windows-10/)

3. Create in your root path a folder with the name "apps": 

For example: `C:\apps`

4. Download the binary zip archive of [Maven 3.3.x or major](https://maven.apache.org/download.cgi)
and extract the content on `C:\apps`:

Example: `C:\apps\apache-maven-3.5.3-bin`

5. Copy the content of this folder and replace the `apache-maven-3.5.3-bin` folder:

Example: `C:\appsn\apache-maven-3.5.3`

You must to see inside this folder the next packages: bin, boot, conf, lib, etc.

6. Now you have to config the environment variables for Maven:

Go to menu and search: `Edit the system environment variables`, click on `environment variables` and add `M2_HOME` with the path `C:\apps\apache-maven-3.5.3`(Be sure to validate the installation path of the Maven).

Add `M2_HMAVEN_HOMEOME` with the same path `C:\apps\apache-maven-3.5.3`. Be sure to add to `path` the next paths: 

- `%JAVA_HOME%\bin`
- `%M2_HOME%\bin`
- `%MAVEN_HOME%\bin`


7. Restart your system and go to the `CMD` and eject:

```
java -version
mvn -v
```

If neither of them exists, please repeat steps one through 6.

8. Download [Git](https://git-scm.com/downloads) 
5. Clone the repository (The repository is private so you'll have to ask for access to your leader)

For the Features Team:
```
git clone https://aviancavsts.visualstudio.com/DigitalChannels/_git/NewUX -b NEWUX
```

For the BugFixes Team:
```
git clone https://aviancavsts.visualstudio.com/DigitalChannels/_git/NewUX -b 0.2.X
```

6. Config your `Git Flow`:

```
git flow init -f

```

For the Features Team:

Release Branch: `master`
Pre-release Branch: `NEWUX`

```
Which branch should be used for bringing forth production releases?
   - 0.2.X
   - NEWUX
Branch name for production releases: [] master

Which branch should be used for integration of the "next release"?
   - 0.2.X
Branch name for "next release" development: [] NEWUX

```

For the BugFixes Team:

Release Branch: `NEWUX`
Pre-release Branch: `0.2.X`

```
Which branch should be used for bringing forth production releases?
   - 0.2.X
   - NEWUX
Branch name for production releases: [] NEWUX

Which branch should be used for integration of the "next release"?
   - 0.2.X
Branch name for "next release" development: [] 0.2.X

```

Note: You should never commit to master!!.

For more info about [GitFlow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow).


6.	Download [NodeJS](https://nodejs.org/en/download/) and verify the installation with the command:
```
node -v
```
7.	Download and Install [AEM 6.3.jar](https://drive.google.com/drive/folders/1NTl-Nz1RuGjU4jLc-qsPvN8gnTH1883U)
8. Download and Install AEM License Property (you must validate with your leader to provide you this license)
9. Avianca VPN Connection - Checkpoint: 

Once again you must validate with your leader to provide you with the credentials to connect to the Avianca VPN (in this way you can connect to the list of airports, among others).

You must to have an Username and a Password.


To be continued...