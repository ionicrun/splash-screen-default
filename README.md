## Setup

__Important:__ if want to run the App on the __iOS simulator__, it is best to add the iOS platform in a different way or alternatively update the `ios-sim` package. There currently is a small issue with `cordova-ios@4.4.0`, which could cause an error like `Cannot read property 'replace' of undefined`, when executing the `ionic cordova run ios` command.

## Step by step

```bash
$ git clone https://github.com/ionicrun/splash-screen-default.git
$ cd splash-screen-default

$ ionic cordova platform add android https://github.com/apache/cordova-ios.git#4.4.0-ios-sim

# alternative: cd platforms/ios/cordova/ && npm install ios-sim&latest
```

If any prompts show up, e.g. `[? Looks like a fresh checkout! ... ]`, answer them with `Y` (yes). 

## Done

You're all set! Go ahead and run the App and see the default splash screen in action.

```bash
$ ionic cordova run ios
# or
$ ionic cordova run android
```