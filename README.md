##### **Note: iOS Build is currently not supported due to unresolved bugs (still in development)**

# Unity-Flutter-AR-Foundation-example
This project aims to enable users to have AR experiences for iOS and for Android. This is made possible by the game engine Unity and its package: AR Foundation. 
To bring the AR experience from Unity to Flutter, the plugin "flutter_unity" from [Glartek](https://github.com/Glartek/flutter-unity/commits?author=cookiejarlid) is used. 
In the example scene, the user can test an AR scene with an printed reference image which is an example of image tracking. 
Have fun

## First things first and nice to know

To setup this example, please follow these instructions in Unity and Android Studio. If you didn't download them yet, please download theme here for free: 
* [Download Unity](https://unity3d.com/de/get-unity/download) 
* [Download Android Studio](https://developer.android.com/studio) 

Supported devices: 
  * [ARCore supported smartphones and tablets (Android)](https://developers.google.com/ar/devices) 
  * [ARKit supported smartphones and tablets (Apple)](https://developer.apple.com/documentation/arkit/verifying_device_support_and_user_permission)

Unity Versions: 
* Unity version build: **2019.4.25f1**
* Unity version tested: **2019.4.25f1**

**Note: You can only test this example with an real mobile device. No simulator supported.**

## Common and Unity Setup

##### 1. First you have to create two new folders for the unity export files. 
For **Android** create one in `<flutter-project-root>/android/` and call it `unityExport`.
For **iOS** create one in `<flutter-project-root>/ios/` and call it `UnityProject`.
   
##### 2. Now open the example unity project in `(<flutter-project-root>/unity/Flutter-Unity-ARFoundation-Example)` with **Unity 2019.4.*^**

##### 3. Please print out the reference image in `<unity-project-root>/Assets/`  called `please_print_me.png` so you have an reference image for image tracking. 
##### 4. Now you have to setup your build settings.

## Build settings (Android) 
* `File > Build Settings`  
* Select **Android** platform on the left and switch platform (if neccessary)
* Check **"Export project"** on the right sided checkbox
* Click Export and export the client to the previously created export folder in your flutter project `<flutter-project-root>/android/unityExport`

## Build settings (iOS) 
_**Currently not supported due to unresolved bugs (still in development)**_

## Flutter Setup in Android Studio
After exporting the files, open your downloaded flutter project in android studio and configure it as described in the following instructions. 
### Android
[Configuring your Flutter project (Android) from Glartek](https://github.com/Glartek/flutter-unity#configuring-your-flutter-project) 

### iOS
_**Currently not supported due to unresolved bugs (still in development).**_
 

## Support
If you have any questions or problems, please post an issue or contact me at: [martin.haferanke@gmail.com](mailto:martin.haferanke@gmail.com)
 
 
## Troubleshooting

#### 1. 'pubspec.yaml not found' - Error after trying to `flutter pub get`
* Solution: 
  * Try  `flutter pub cache repair`
  * Type  `flutter pub get` again


#### 2. No iOS support 
* Solution: 
  * Due to some bugs in xCode and Android Studio there is currently no support for iOS. Issues will still being created later.