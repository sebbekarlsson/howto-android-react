# Getting started on MacOS

## Installing the Android SDK using `Homebrew`
    
    brew tap caskroom/cask
    brew cask install android-sdk

> This will place the `Android SDK` at /usr/local/Caskroom/android-sdk/\<version\>

## Updating the SDK and installing requirements

    sdkmanager --update
    sdkmanager "platforms;android-25" "build-tools;25.0.2" "extras;google;m2repository" "extras;android;m2repository"
    sdkmanager --licenses

## Making sure your computer knows where the SDK is located

    export ANDROID_HOME=/usr/local/Caskroom/android-sdk/\<version\>

# Android Emulator

## Launching an emulator

    emulator -avd my_android

> I have already created an AVD, here's how to do that:
> [stackoverflow](https://stackoverflow.com/questions/3552218/android-create-avd-size-on-windows-command-prompt)

> Make sure this is running before starting your react-native app

# React Native

## Installing React Native
    
    nom install -g yarn
    npm install -g react-native 

## Creating your first application

    react-native init myapp

    cd myapp
    react-native run-android
