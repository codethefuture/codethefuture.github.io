---
layout: post
title: IntelliJ IDEA で Android 開発環境を整えたメモ
description: ""
category : development
tags : [IntelliJ IDEA, Android]
---
{% include JB/setup %}

### Download
* http://developer.android.com/sdk/index.html
* http://www.oracle.com/technetwork/java/javase/downloads/index.html

### Android SDK setting
* Android SDK Manager start
    1. terminal.app
    2. $ cd [Android SDK]/sdk/tools/android
    3. tools and SDK Platform install
    4. Quit

* AVD Manager start
    1. $ android avd
    2. Android Vertical Devices
    3. New button
    4. create android vm
    5. Quit

### Intellij IDEA setting
* Quick Start
  1. Configure
  2. Project Defaults
  3. Project Structure
  4. Project Settings - Project
  5. Project SDK - New button
  6. JDK
  7. select for JDK Path
  8. Project SDK - New button
  9. Android SDK
  10. select for AndroidSDK Path
  11. OK button


