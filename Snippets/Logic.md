# Logic

## If Statements

```swift
let scale:Int = 8

if scale < 10 {
    print("Less than 10")
}

// Less than 10
```

```swift
let hat:String = "Fez"

if hat == "Fedora" {
    print("Hat is a Fedora.")
} else {
    print("Hat is not a Fedora.")
}

// Hat is not a Fedora.
```

```swift
let hat:String = "Fez"

if !hat.isEmpty {
    print("You are wearing a hat.")
}

// You are wearing a hat
```

## Case Statements

```swift
let day = NSCalendar(calendarIdentifier: NSCalendarIdentifierGregorian)!.components(NSCalendarUnit.Weekday, fromDate: NSDate()).weekday

print(day)
// 3

switch (day) {

case 1:
    print("Monday")
    break

case 2:
    print("Tuesday")
    break

case 3:
    print("Wednesday")
    break

case 4:
    print("Thursday")
    break

case 5:
    print("Friday")
    break

case 6:
    print("Saturday")
    break

case 7:
    print("Sunday")
    break

default:
    print("Invalid day")

}

// Wednesday
```
