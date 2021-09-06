# SketchUpdate
[![](https://jitpack.io/v/Knight-Fiury/SketchUpdate.svg)](https://jitpack.io/#Knight-Fiury/SketchUpdate)
![GitHub last commit](https://img.shields.io/github/last-commit/Knight-Fiury/SketchUpdate)
[![API](https://img.shields.io/badge/API-21%2B-blue.svg?style=flat)](https://android-arsenal.com/api?level=21)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/Knight-Fiury/SketchUpdate/blob/main/LICENSE)
![Website](https://img.shields.io/website?down_color=lightgray&down_message=Server%20Down&up_color=blue&up_message=Up%20%26%20Running&url=https%3A%2F%2Fsketchupdate.tk)
[![Users](https://img.shields.io/endpoint?url=https://sketchupdate.tk/statistics/user.php)](https://sketchupdate.tk/#download)

This is an app to add In-App-Update system in your app in minutes... 

You can notify specific users or all of them at once. Besides you can schedule the msg whatever you are going to send with this app. Furthermore you can use this app to Ban, Send Reward news or Warn the user

# Features 
 - [x] Full Free
 - [x] Simple Api Response 
 - [x] Easy To Use
 - [x] Realtime UI Change
 - [x] Supports Specific User Update 
 - [x] Schedule Updates 
 - [x] Force or Unforce App Update
 - [x] Supports OneTime Message Send
 - [x] Fully Customizable 
 - [x] No Branding or Watermark 
 - [x] Send Pop-up Notifications

## Download SketchUpdate
You can download SketchUpdate from our website
visit us https://sketchupdate.tk

### Step 1 : Account Creation
Download & complete registration. After that simply login. You have to verify yourself every time you login...

### Step 2 : Creating Project
After completing verification you can create a project. Simply click on "Add New Project" to start. Give a name of your project for easy recognition and for the api. 

![Image 1](https://user-images.githubusercontent.com/86944710/129434900-af79acbb-0667-41fe-9ed4-c75210e9e981.jpg)

### Step 3 : Copying Api
An api will be created automatically when you create a new project. You can simply copy the api of a project just by swipe that left or right...

![Image 2](https://user-images.githubusercontent.com/86944710/129434944-3bfce963-f242-4601-a2d3-5c9eca6a1e3f.jpg)

Your copied API should look like this
```https://sketchupdate.tk/data.php/?appId=[PROJECT_NAME]```

i.e. In this case the API is ```https://sketchupdate.tk/data.php/?appId=testing_4620```

### Step 4 : Understanding Api Response
A successful ```GET``` response will be like below... 
```json
{
 "Server_Response":
     [
         {
          "sendTo":"all",
          "alertType":"sheet2",
          "newVersion":"1.2",
          "title":"Update App?",
          "titleColor":"#000000",
          "isSubtitle":"true",
          "subtitle":"Download Size 10MB",
          "description":"We recommend that you update to the latest version. You can keep using this app while downloading the update",
          "descriptionColor":"#000000",
          "appIcon":"https:\/\/sketchupdate.tk\/assets\/images\/favicon.png",
          "appName":"Sketchupdate",
          "mainBtnTxt":"Update",
          "mainBtnTxtColor":"#FFFFFF",
          "mainBtnBackColor":"#000000",
          "mainBtn":"https:\/\/sketchupdate.tk",
          "isExtraBtn":"true",
          "extraBtnTxt":"dismiss",
          "extraBtnTxtColor":"#000000",
          "extraBtnBackColor":"#FFFFFF",
          "extraBtn":"dismiss",
          "isCancelable":"false",
          "isOneTime":"false",
          "backColor":"#FFFFFF",
          "radius":"25",
          "btnRadius":"25",
          "isHeader":"true",
          "time":"2021\/8\/7\/11\/10"
         }
     ]
}
```
### Step 5 : Add Dependency
```groovy
dependencies {
    implementation 'com.github.Knight-Fiury:SketchUpdate:1.0-alpha'
}
```

### Step 6 : Usage
Call SketchUpdate Dialog Through This Code
```java
//Store The API Response in a String//
//Here Response is The String//
sketchupdate.callDialog(Response, MainActivity.this);
//sketchupdate.callDialog(String, Activity);//
```
Call SketchUpdate Notification Through This Code
```java
//Store The API Response in a String//
//Here Response is The String//
sketchupdate.callNotification(Response, getApplicationContext());
//sketchupdate.callNotification(String, Context);//
```

## Schedule The Update
Using SketchUpdate you can set the time of your app updates just by clicking on the button next to "Send Update". After setting the time click on "Send Update" and you are done

![Image 3](https://user-images.githubusercontent.com/86944710/129435210-45946179-c355-4f47-8cab-7b5d570dea32.jpg)

# Donate
[![Donate](https://s2.svgbox.net/payments.svg?ic=paypal)](https://paypal.me/safinrazoan) 
