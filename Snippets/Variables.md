# Variables

## Constant

```swift
let maxHealth:Int = 100
```

## String

```swift
var fullName:String = "Scott Doxey"
```

## Number

```swift
var currentHealth:Int = 100
```

```swift
var currentLevel:Double = 31.5
```

## Array

```swift
var food:[String] = ["French Fries", "Pizza", "Pasta"]
```

### Deleting by Index

```swift
food.removeAtIndex(1)
```

## Dictionary

```swift
var programmingSkillLevels:[String: Int] = ["JavaScript": 11, "HTML": 10, "CSS": 10, "Swift": 1]
```

### Return Array of Keys

```swift
print(Array(programmingSkillLevels).keys)
```

### Deleting by Key

```swift
programmingSkillLevels.removeValueForKey("JavaScript")
```

## ENUM

```swift
enum daysOfTheWeek {
    case Monday
    case Tuesday
    case Wednesday
    case Thursday
    case Friday
    case Saturday
    case Sunday
}

print(daysOfTheWeek.Monday)
```
