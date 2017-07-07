# UnityCrossPlatformApi
A unity plugin that provides a unified cross-platform API


[Document](https://litefeel.github.io/UnityCrossPlatformApi/Documentation/DoxygenOutput/html/index.html)





## Frequently Asked Questions

#### Crashed when calling the SaveToAlbum () method on iOS 10

> This app has crashed because it attempted to access privacy-sensitive data without a usage description.The app's Info.plist must contain an NSPhotoLibraryUsageDescription key with a string value explaining to the user how the app uses this data.

Add `NSPhotoLibraryUsageDescription` to `Info.plist` file to fix it.
like following code:

~~~ xml
<key>NSPhotoLibraryUsageDescription</key>
<string>Photo Library Access Warning</string>
~~~

[stackoverflow](https://stackoverflow.com/questions/39519773/nsphotolibraryusagedescription-key-must-be-present-in-info-plist-to-use-camera-r)

