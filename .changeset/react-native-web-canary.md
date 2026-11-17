---
'expo': patch
'expo-template-default': patch
'expo-template-tabs': patch
'babel-preset-expo': patch
'@expo/metro-config': patch
'@expo/cli': patch
'@expo/html-elements': patch
'expo-system-ui': patch
'expo-camera': patch
'expo-gl': patch
'expo-router': patch
'expo-symbols': patch
---

Upgrade `react-native-web` and `babel-plugin-react-native-web` to 0.22.0-canary-20261119-0cbcdde. This version is ESM only, so imports of its internal modules now use explicit `.js` file paths.

`expo/types` now loads the types that `react-native-web` includes, in place of its own copy. React Native props and styles get the web values that `react-native-web` supports, on all platforms. For example, `fontSize` and `lineHeight` accept strings, and `View` accepts `href`. The `className` props stay.
