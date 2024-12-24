# UpdateReactnative0.6xto0.7x
Update Existing React Native App from react-native version 0.6x to 0.7x

# Steps for update react-native version 0.6x to 0.7x
Here we will take an example to update react-native version from 0.69.4 to 0.75.0

# Step 1:
Remove node_modules, package-lock.json and Podfile.lock

# Step 2:
Now go to package.json and update "react" :"^x.x.x" to "react" :"^18.3.1" and "react-native" :"^0.69.4" to "react-native" :"^0.75.0" 

# Step 3:
Use https://microsoft.github.io/rnx-kit/docs/tools/align-deps#:~:text=%40rnx%2Dkit%2Falign%2D,are%20curated%20from%20real%20apps to check that your packages are using compatible dependencies and versions and update accordingly.

# Step 4:
Use https://react-native-community.github.io/upgrade-helper/?from=0.69.4&to=0.75.4&package=com.test&name=test and get the diff and change the files accordingly.

# Step 5:
Now run "npm i"

# Step 6:
Now open the android folder in Android Studio and proceed to Sync Project File with Gradle.

# Step 7:
After completion run the app using "cd android && react-native run-android"

# Step 8:
Open projectname.xcworkspace in Xcode and wait for sync to be completed.

# Step 9:
Now run "cd ios && pod install"

# Step 10:
After completion run the app using "react-native run-ios"

# Step 11:
If you get any issue in any of dependencies, go to their git repo to check the latest version and compatibility with the react-native version .

# Step 12:
If there is a need to change inside the node_modules after change use https://www.npmjs.com/package/patch-package for patching it. So that after npm install further time no need to update the same in node modules.


# Important Links:

- [React Native Website](https://reactnative.dev/docs/getting-started) - learn more about React Native.
- [React Native Upgrade Helper Website](https://react-native-community.github.io/upgrade-helper/?from=0.69.4&to=0.75.4&package=com.test&name=test) - learn more about React Native Upgrade Helper.
- [React Native Package Compatibility Website](https://microsoft.github.io/rnx-kit/docs/tools/align-deps#:~:text=%40rnx%2Dkit%2Falign%2D,are%20curated%20from%20real%20apps) - learn more about React Native Package Compatibility.
- [React Native Patch Package Website](https://www.npmjs.com/package/patch-package) - learn more about React Native Patch package.

 # Happy Coding!! :grinning: :grinning: :thumbsup:
 
 # If you need any help contact me, always Happy to help . :love_you_gesture::love_you_gesture:
 
 # If you like this documentation give a star and fork it for your future reference . :crossed_fingers: :crossed_fingers: :love_you_gesture:
