
### follow https://github.com/react-native-community/react-native-maps/blob/master/docs/installation.md 

1. create google map api key

2. add three lines to android/build.gradle

buildscript {
    ext {
        buildToolsVersion = "28.0.3"
        minSdkVersion = 16
        compileSdkVersion = 28
        targetSdkVersion = 28

///////////////////////////////////////
        supportLibVersion = '28.0.0'
        playServicesVersion = '16.1.0'
        androidMapsUtilsVersion = "0.5+"
///////////////////////////////////////



3. add this to android/app/src/main/AndroidManifest.xml

 <meta-data
        android:name="com.google.android.geo.API_KEY"
        android:value="google map api key"
      />


4. run this from root
cd android && gradlew clean
cd .. && react-native run-android


5. Ensure also that the relevant Google APIs have been enabled for your project

6. 
Run:
npm start --clear-cache
react-native run-android
In Case Of Error
cd android
gradlew clean
cd ..
react-native run-android
	










