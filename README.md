
# react-native-broadcast

## Getting started

`$ npm install react-native-broadcast --save`

### Mostly automatic installation

`$ react-native link react-native-broadcast`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-broadcast` and add `RNBroadcast.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNBroadcast.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<
5. Need to add Link binary to `libz` & `libstdc++` into final project

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNBroadcastPackage;` to the imports at the top of the file
  - Add `new RNBroadcastPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-broadcast'
  	project(':react-native-broadcast').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-broadcast/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-broadcast')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNBroadcast.sln` in `node_modules/react-native-broadcast/windows/RNBroadcast.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Com.Reactlibrary.RNBroadcast;` to the usings at the top of the file
  - Add `new RNBroadcastPackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNBroadcast from 'react-native-broadcast';

// TODO: What to do with the module?
RNBroadcast;
```
