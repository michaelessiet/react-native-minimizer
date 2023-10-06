# react-native-minimizer
Minimize React Native app, works on Android And iOS.
## Installation

```sh
npm install react-native-minimizer
```

### Mostly automatic installation

Add this to your `android/build.gradle` file, under `allprojects.repositories`:

```
allprojects {
  repositories {
    // ...
    maven {
      url("${project(':react-native-minimizer').projectDir}/libs")
    }
  }
}
```

## Usage
```javascript
import Minimizer from 'react-native-minimizer';

// exits the aplication
Minimizer.exit();
// goes back to previously openned app if there was such
Minimizer.goBack();
// just minimizes the app
Minimizer.minimize();
```
