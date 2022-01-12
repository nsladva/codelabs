# Building the app for iOS Simulator
These are directions to build on an M1 Macbook Air
1. Start a Terminal instance in `Working_Copy`
1. Initiate an iOS simulator instance with `open -a Simulator`
1. To execute the app use `flutter run`. If this succeeds and runs, you're done! If it spits an error, continue down
1. Go to the ios directory by using `cd /ios`
1. Delete `Podfile` and `Podfile.lock` from the `/ios` folder
1. Sometimes you'll need to run `sudo arch -x86_64 gem install ffi`, idk why though
1. Reinit the `Podfile` by running `arch -x86_64 pod install`. If there's an error, re-run step 3.
1. Open `Podfile` and uncomment the line `# platform :ios, '9.0'` and replace the ios version with the latest version in all json files in `\Pods\`
1. Run `flutter run`

