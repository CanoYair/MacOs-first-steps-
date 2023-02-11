### React Native Install Config  

---------------------
## Getting Started 

Homebrew is a type of platform dependency installation software which would allow us to install all the download and install all the required files. To install Homebrew, open your terminal prompt and type the below command :

```sh 
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Brew 

A few examples of useful commands and/or tasks.

```sh
brew install wget 
```


# Node & Watchman

## Installing dependencies

You will need Node, Watchman, the React Native command line interface, a Ruby version manager, Xcode and CocoaPods.

While you can use any editor of your choice to develop your app, you will need to install Xcode in order to set up the necessary tooling to build your React Native app for iOS.

> nodejs watchamn 

```sh
brew install node
brew install watchman
```

>Yarn 

```
npm install --global yarn
```

> Cocopods 

```sh
brew install cocoapods
```


## Utilities & Tools  Extra 

```
sudo gem install ffi
```

## nvm 

``` sh
brew install nvm 
```

## > nvm install  npm version 
 
* nvm ls-remote 
* nvm install  10..2.1
* nvm use  10.2.1
* node --version 

-----------------

# Android

### Installing JDK

With Homebrew, this is pretty straightforward.

```sh
brew tap AdoptOpenJDK/openjdk
brew install --cask adoptopenjdk8
```


Install Java Development Kit (JDK) using Homebrew with the following command:

```
brew install --cask adoptopenjdk/openjdk/adoptopenjdk8

```

>Java Version 

```
java -version
``` 


-----------
# Android

### Configure the ANDROID_HOME environment variable

What we want to do is to open `$HOME/.zshrc`to add environmental variables. If you're using `bash`, it should be `$HOME/.bash_profile` or `$HOME/.bashrc` . To open`$HOME/.zshrc` or `$HOME/.bashrc`, go to the terminal and type


```
nano ~/.zshrc
```

or

```
nano ~/.bashrc
```


```
npm install -g expo-cli
```


## Configure ANDROID_HOME environment variable

Open your Terminal and navigate to your computer’s root directory (usually it’s the default directory).

Now you need to open your `.bashrc` or `.bash_profile` file if you have any. If you don’t have either, create one by running this command:

```text
touch .zshrc
```

Now you can open this `.bashrc` file in your preferred editor. To open it directly in your Terminal via nano, run this command:

```text
nano ~/.zshrc
```

Now you need to add your environment variables to this file. This part can be a little tricky to get right, but I'll try my best to explain.

The official React Native docs tell you to add these variables to your bash file:

```bash
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

But they don’t mention that you need to edit the first line so it matches your exact location path to your Android SDK folder.

This line:

```bash
export ANDROID_HOME=$HOME/Library/Android/sdk
```

Remember I told you this earlier when setting up Android Studio:

> Take note of the **Android SDK Location** path at the top of this screen. You’ll need this path value to define environment variables shortly.

If you didn't, you can just go to Android **Preferences > Appearance & Behavior > System Settings > Android SDK** and here you’ll see the location you need to add to the ANDROID_HOME variable. In my case it’s this:

```bash
/Users/david/Library/Android/sdk
```

So I changed this line:

```bash
export ANDROID_HOME=$HOME/Library/Android/sdk
```

To this:

```bash
export ANDROID_HOME=/Users/david/Library/Android/sdk
```

So now my `.bashrc` file looks like this:

```bash
export ANDROID_HOME=/Users/david/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

You only need to change the _first line_ (because the other lines get the path referenced via the `$ANDROID_HOME` variable) to match the Android SDK location from _your_ Android Studio. Then copy-paste it all into your `.bashrc` file and save it by pressing CTRL + X, Y, Enter, to save changes.

Now restart your terminal to make the changes take effect.

Enter this command to load your configurations into your current shell:

```bash
source $HOME/.zshrc
```

And verify that `ANDROID_HOME` has been added to your path by running this command:

```bash
 echo $PATH.
```

Your output should look similar to this:

```bash
Users/david/Library/Android/sdk/emulator:/Users/david/Library/Android/sdk/tools:/Users/david/Library/Android/sdk/tools/bin:/Users/david/Library/Android/sdk/platform-tools
```

If it does, you should be set up and ready to run React Native apps via the Android Studio Emulator!

--------------

# React Native: How to Setup React Native CLI for iOS on macOS

![[react 3.png]]

-   **Node:** a cross-platform runtime environment that allows you to run JavaScript on the server-side.
-   **Watchman:** a performance-boosting tool that watches for changes in the filesystem.
-   **React Native CLI:** the Command Line Interface
-   **Xcode:** a suite of software tools for developing Apple/iOS software
-   **CocoaPods:** an app dependency manager built with Ruby and used for Objective-C and Swift. We use it to manage external libraries.
----------



### Expo Go Quickstar

Run the following command to create a new React Native project called "AwesomeProject":

> npm  

```
npx create-expo-app AwesomeProject
```

```
cd AwesomeProject
npx expo start
```

or 

>yarn

```
yarn create expo-app AwesomeProject
```

```
cd AwesomeProject
yarn expo start
```

------

### React Native CLI Quickastart  

#### Development OS
mac os 

#### Target OS
ios 


```
npx react-native init AwesomeProject
```

```
npx react-native start
```

```
npx react-native run-ios
```

```
react-native run-ios --simulator "iPhone 5s
```

![[GettingStartediOSSuccess-e6dd7fc2baa303d1f30373d996a6e51d.png]]


### Java


```
brew tap homebrew/cask-versionsb
rew install --cask zulu11
```

>`source ~/.zshrc`

```
export ANDROID_HOME=$HOME/Library/Android/sdkexport PATH=$PATH:$ANDROID_HOME/emulatorexport PATH=$PATH:$ANDROID_HOME/platform-tools
```

>`source ~/.zshrc` 


```
npx react-native init AwesomeProject
```

```
npx react-native start
```


```
npx react-native run-android
```


-----------
