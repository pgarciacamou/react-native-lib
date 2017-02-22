
# react-native-lib

## Getting started

`$ npm install react-native-lib --save`

### Mostly automatic installation

`$ react-native link react-native-lib`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-lib` and add `RNLib.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNLib.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNLibPackage;` to the imports at the top of the file
  - Add `new RNLibPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-lib'
  	project(':react-native-lib').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-lib/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-lib')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNLib.sln` in `node_modules/react-native-lib/windows/RNLib.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Cl.Json.RNLib;` to the usings at the top of the file
  - Add `new RNLibPackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNLib from 'react-native-lib';

// TODO: What do with the module?
RNLib;
```
  