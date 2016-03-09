# NSCoding

*TodoItem.swift*

```swift
struct PropertyKey {

    static let contentkey = "content"
    static let completedkey = "completed"

}

class TodoItem: NSObject, NSCoding {

    var content:String = ""
    var completed:Bool = false

    init(content: String, completed: Bool) {

        self.content = content
        self.completed = completed

    }

    required init(coder aDecoder: NSCoder) {

        self.content = aDecoder.decodeObjectForKey(PropertyKey.contentkey) as! String
        self.completed = aDecoder.decodeObjectForKey(PropertyKey.completedkey) as! Bool

    }

    func encodeWithCoder(aCoder: NSCoder) {

        aCoder.encodeObject(content, forKey: PropertyKey.contentkey)
        aCoder.encodeObject(completed, forKey: PropertyKey.completedkey)

    }

}
```

## Encoding and Storing Data

```swift
let savedTodoItems = NSKeyedArchiver.archivedDataWithRootObject(todoItems)

NSUserDefaults.standardUserDefaults().setObject(savedTodoItems, forKey: "todoItems")
```

## Retrieving and Decoding Data

```swift
let storedTodoItems = NSUserDefaults.standardUserDefaults().objectForKey("todoItems")! as AnyObject

todoItems = NSKeyedUnarchiver.unarchiveObjectWithData(storedTodoItems as! NSData) as! [TodoItem]
```
