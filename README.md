# JavaAppiumCucumber

Mobile automation using java with Appium and Cucumber.

### Prerequisites

* Appium Server
* Java_JDK_8
* Maven
* IDE Editor (Eclipst, InteliJCE, VSCode)
* Real Device / Emulator

#For some how to installation, you can find here ["Conflence Jira"](https://tcashsquad.atlassian.net/l/c/Rc5nB2Bt "Conflence Jira")

### Tested ON
* Node version `17.6.0`
* Npm version `8.5.1`
* Java version `1.8.0_202`
* Maven version `3.8.4`
* Appium version `1.22.2`
* Android SDK Platform-tools `32.0.0`
* MacOS BigSur `11.5.1`
* Emulator Android `Pixel_5_API_30`

### This is directory structure ###

    .
    ├── src
    │   ├── test
    │   │   ├── resources
    │   │   │   └── features
    │   │   │       ├── 2_Login.feature
    │   │   │       └── 1_Register.feature
    │   │   └── java
    │   │       ├── utility
    │   │       │   └── Hook.java
    │   │       ├── stepdefination
    │   │       │   ├── RegisterStep.java
    │   │       │   └── LoginStep.java
    │   │       ├── runner
    │   │       │   └── TestRunner.java
    │   │       └── page
    │   │           ├── RegisterPage.java
    │   │           └── LoginPage.java
    │   └── app
    │       └── Android_WebDriverio.apk
    ├── pom.xml
    ├── env.properties
    └── README.md

### How to Getting Started

* Start AppiumServer port 4723
* Start emulator / connect real device, and attach with "adb device"
* Open file env.properties, and changes with your emulator / real device

    ```bash
    deviceName=emulator-5554
    udid=emulator-5554
    platformName=11
    appPackage=com.wdiodemoapp
    appActivity=com.wdiodemoapp.MainActivity
    ```
* Run Maven

    ```bash
    mvn verify
    ```
