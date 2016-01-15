# Loops

## For Loop

```swift
let values = [1, 2, 3, 4, 5]

for value in values {

    print(value)

}

// 1
// 2
// 3
// 4
// 5
```

```swift
let values = [1, 2, 3, 4, 5]

for (key, value) in values.enumerate() {

    print(values[key])

}

// 1
// 2
// 3
// 4
// 5
```

## While Loop

```swift
let values = [1, 2, 3, 4, 5]

var i = 0

while i < values.count {

    print(values[i])

    i++

}

// 1
// 2
// 3
// 4
// 5
```
