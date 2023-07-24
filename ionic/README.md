# Ionic (Cordova)
## ionic serve
```
ionic serve
```
## cordova build debug for android
```
ionic cordova build --debug/--release android
```
## You can check if Java JDK, Android SDK, Gradle are properly installed before building an app.
```
cordova requirements android --verbose 
```
## Remove platform : android
```
ionic cordova platform rm android
```
## Add ionic platform  (cordova platform add <platform>)
```
ionic cordova platform add android
```
## 
```
npm i -g native-run
```
## Build android 
```
ionic cordova build android
```
## Build android
```
ionic cordova run android -l
```
 ## Build android and run in external device
```
ionic cordova run android -l --external
```
##  add cordova plugin androidx
```
ionic cordova plugin add cordova-plugin-androidx
```
## cordova plugin androidx adapter
```
ionic cordova plugin add cordova-plugin-androidx-adapter
```
## Ionic command list 
```
Ionic command
```
## Ionic generate (page moduel and all)
```
Ionic generate
```
## Generate ionic page by folder
```
Ionic generate page recepis/recepis-deatails
```

# Ionic Capacitor
Ionic, Capacitor and Android Studio | DigitalOcean Android Development - [Ionic Documentation](ionicframework.com)
## Build android and run in external device
```
ionic capacitor run android -l --external
```
## Build android 
```
ionic capacitor build android
```
## ionic integrations enable capacitor
```
ionic integrations enable capacitor
```
## remove android folder
```
rm -rf android/
```
## Add capacitor android
```
npx cap add android
```
## Cpacitor sync android
```
npx cap sync android
```
## Add package id and app name 
```
npx cap init ? App name: CapApp ? App Package ID:com.mydomain.myappname
```

## Steps for ionic capacitor andtroid build : 
1. ```ionic build```
2. ```ionic cap add ios```
3. ```ionic cap add android```
4. ```ionic cap copy``` (Every time you perform a build (e.g. ionic build) that updates your web directory (default: www),
 you'll need to copy those changes into your native projects:)
5. ```ionic cap sync``` (Note: After making updates to the native portion of the code (such as adding a new plugin), use the sync command:)
6. ```ionic cap open android```

## APK without capacitor
1. ```ionic capacitor add android ```
2. ```ionic capacitor copy android && cd android && ./gradlew assembleDebug && cd``` 
Then your apk will be at:
android/app/build/outputs/apk/debug/app-debug.apk


## ReferenceError: globalThis is not defined
```
npm install globalthis
```
## Capacitor can’t build due to AndroidX conflicts, at a total loss on how to fix

1. ```npm install jetifier```
2. ```npx jetify ```
3. ```npx cap sync android```
which changed the import reference from: `import android.support.v4.app.ActivityCompat;`

# Add java home and android home path
## if you are using WINDOWS follow these steps to change JAVA_HOME path.

1. go to my computer properties.
2. click on Advanced system settings (A new window will be open).
3. click on Environment Variables Button.
4. in System variables panel. find JAVA_HOME variable, add new or click on EDIT.
5. Example 'C:\Program Files\Java\jdk-17' 


## Chrome dev list 
   
```
    chrome://inspect/#devices
```

## Android emulator cannot acces api use IP 10.0.2.2 
10.0.2.2	Special alias to your host loopback interface (127.0.0.1 on your development machine)

## Errors 
### “Webpage not available… The webpage http://localhost:8100/ 17 could not be loaded because: net::ERR_CLEARTEXT_NOT_PERMITTED”

just try
```
npm i -g native-run
```
then
```
ionic capacitor run android -lc --host=0.0.0.0 -native-run
```
for live-reload


 
