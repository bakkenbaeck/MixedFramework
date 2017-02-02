# MixedFramework

A framework that combines both Objective-C and Swift.

```swift
import UIKit
import MixedFramework

@UIApplicationMain
class AppDelegate: UIResponder {
    var window: UIWindow?
}

extension AppDelegate: UIApplicationDelegate {

    func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplicationLaunchOptionsKey: Any]?) -> Bool {
        SwiftSource.helloFromSwift()
        ObjectiveCSource.helloFromObjectiveC()

        return true
    }
}
```
