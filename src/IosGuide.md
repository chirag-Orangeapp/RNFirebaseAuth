# React Native IOS Setup

This is guide you to Xcode setup while enabling React Native Firebase Authentication.

=> Add GoogleService-info.plist in Xcode 
  Path : MyApp/GoogleService-info.plist

## Email and Password authentication with firebase

1. Enable Email/Password Auth on Firebase. 
    - No requirements of any Xcode setup.

## Facebook authentication with firebase

1. Follow the step of Facebook developer console.
    - Perfrom step 2,3,4 of setup guide of Facebook

2. In Xcode add follwoing code at AppDelegate.m file
    ```
     #import <FBSDKCoreKit/FBSDKCoreKit.h>

     - (BOOL)application:(UIApplication *)application openURL:(nonnull NSURL *)url options:(nonnull NSDictionary<NSString  ,id> *)options {  return [[FBSDKApplicationDelegate sharedInstance] application:application openURL:url options:options] 
    ```

## Google authentication with firebase

1. Follow the setup guide of firebase for firebase setup.

2. Add URL schemes in Info.plist file in Xcode
    ```
    <key>CFBundleURLTypes</key>
	<array>
		<dict>
			<key>CFBundleTypeRole</key>
			<string>Editor</string>
			<key>CFBundleURLSchemes</key>
			<array>
				<string><YOUR_REVERSE_CLIENT_ID></string>
			</array>
		</dict>
	</array>
    ```

## Phone number authentication with firebase

1. Enable Phone Auth on Firebase. 
    - No requirements of any Xcode setup if you had already added URL schmes otherwise follow the step 2 of google auth.

## Apple authentication with firebase

1. From Signing & Capabilities to add capability.
    - click on + button and add `Sign In with Apple`.
    - After add apple ID Target <YOURAPPName> in Team in `Signing` info.
    - Also add apple ID Target <YOURAPP_Tests> in Team in `Signing` info.

## Resolve conflict @react-native-firebase/auth plugin

1. For ios setup in your app follow all steps of firebase while adding your ios app in firebase.