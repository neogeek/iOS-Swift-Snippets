# NSUserDefaults

```swift
NSUserDefaults.standardUserDefaults().setObject("Fez", forKey: "hat")

let hat = NSUserDefaults.standardUserDefaults().objectForKey("hat")!

print(hat)

// Fez
```
