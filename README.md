
# walkbase-sdk-android

## Getting started

`$ npm install git+https://github.com/conexusTech/walkbase-sdk-android.git --save`

### Mostly automatic installation

`$ react-native link react-native-walkbase-engage`

### Manual installation


#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNWalkbaseEngagePackage;` to the imports at the top of the file
  - Add `new RNWalkbaseEngagePackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-walkbase-engage'
  	project(':react-native-walkbase-engage').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-walkbase-engage/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-walkbase-engage')
  	```

  
