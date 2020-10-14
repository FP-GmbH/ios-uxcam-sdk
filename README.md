# UXCam iOS SDK

This is the UXCam iOS SDK

# To install

## Using [Cocoapods](https://cocoapods.org/)

Add the following to your Podfile:

`pod 'UXCam`

and run `pod update` and you should be good to go.



# Integration

Get your App key from the dashboard at UXCam.com

## Objective-C

In your `AppDelegate.m` file:

	#import <UXCam/UXCam.h>

and in your `application:didFinishLaunchingWithOptions:` method add:

```objective-c
	[UXCam optIntoSchematicRecordings];
	[UXCam startWithKey:@"App-key from UXCam"]; 
```

## Swift

In your `AppDelegate.swift` file:

	import UXCam
	
and in your `func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool` function add:

```swift
	UXCam.optIntoSchematicRecordings()
	UXCam.start(withKey:"App-key from UXCam")
```


## Developer Documentation

Documentation on using the various API methods can be found [here](https://help.uxcam.com/hc/en-us/categories/115000129131-Developer-Guide)



## Acknowledgements

Thanks to [Anurag Ajwani](https://medium.com/@anuragajwani) for a series of excellent articles on building and distributing XCFrameworks