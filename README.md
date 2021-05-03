# Flutter Vancouver Meetup
### Oct 28th 2020

## iOS 14 Major Updates

- Cupertino Icons
- App Clips

### Cupertino Icons

- Natively called as [SF Symbols](https://developer.apple.com/design/human-interface-guidelines/sf-symbols/overview/) and in Flutter its [Cupertino Icons](https://pub.dev/packages/cupertino_icons)
- Previously only few icons were available but now most if not all of the SF Symbols are availabe as part of Cupertino Icons
- Flutter Version >= 1.22 and there should be dependency on CupertinoIcons package
- You can find all the available symbols in two ways
  - Flutter maintains a list in their [repo](https://flutter.github.io/cupertino_icons/)
  - Install [SFSymbols app](https://developer.apple.com/sf-symbols/) but you need a mac
  - Use the test app that I have created(but I won't be updating it)
  - Alternative: [flutter_sfsymbols](https://pub.dev/packages/flutter_sfsymbols)

### App Clips

- Landing page of [App Clip](https://developer.apple.com/app-clips/)
- If you are an Android user, similar to instant apps
- Allows you load your app without actually installing the app
  - QR Code
  - NFC 
  - and few more
- Has to be part of a full iOS application
- App Clip is called a target and a single app can have multiple targets
  - For example, a restaurant app can have multiple app clips for each restaurant it manages
- Its still fairly new in Flutter and there is a lot of [manual process](https://flutter.dev/docs/development/platform-integration/ios-app-clip) in trying to configure app clip
- Still experimental and will keep changing. Its going to be a challenge because Apple themselves launched this recently, so they will be coming up with fixes.
- I tried creating an App Clip but nothing shows up, its just a blank screen unfortunately
- Make sure your Cocoapods is 1.10 version
  - ```sudo gem install cocoapods``` to update your cocoapods
  - ```sudo gem install ffi -- --disable-system-libffi``` if you get an error that library ```ffi``` could not be found
- The code for the app clips can be different
- Its not production ready, I would highly recommend waiting until the process is automated or atleast Flutter team tell us that its ready
