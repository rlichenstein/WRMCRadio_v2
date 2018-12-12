This is a mobile Radio Streaming application for the radio station WRMC 91.1 FM Middlebury College Radio. 
Below is just a basic guide for navigating our code base.

BRANCHES:
Master: The branch usually up to date with both other branches, and de-facto place to push iOS updates.
androiddev: The branch for the android development if it includes changes to files that are hard to merge (notably package-lock.json and 
package.json). Currently merged into the main master branch.
reid-current: A slight offshot for when we re-initialized the entire directory from expo-eject to only React Native. Manually updated
on the android end and then merged into master. Not currently used.



In the 'android' directory you will find all of the android specific code that includes both code added by us for importing
3rd party libraries and code generated by the React Native environment we worked in. The same can be said for the 'iOS' directory.
Each of these directories can be open and run as projects in their respective native simulators, AndroidStudio and Xcode. 

The key interpretable files are the javascript files found in the 'screens' directory. These are javascript files for the coding
of each screen of our application, shared by both iOS and Android deployments. 
Another directory of interest is the 'assets' directory both in the root folder, and the android/ios folders that contain some imported
assets. 
The 'android/app/src/main/AndroidMainfest.xml' file is also a very important one along with 'android/build.gradle' for understanding some
of the android side's setup and imports. 

The remainder of the files are too long to enumerate on, some have very little changes to them and are pre-generated. 
