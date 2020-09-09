# uuid example React Native

```
yarn
npx pod-install

// For iOS:
yarn run ios

// Or for Android:
yarn run android
```

This example was created with the following steps:

1. Create new React Native App:

   ```
   npx react-native init reactnative
   cd reactnative
   ```

1. Install uuid and `crypto.getRandomValues()` Polyfill:

   ```
   yarn add uuid react-native-get-random-values
   npx pod-install
   ```

1. Add the polyfill as [first import in index.js](./index.js#L5):

   ```js
   import 'react-native-get-random-values';
   ```

1. Make use of [`uuid` in App.js](./App.js).
