# UILabel

```swift
override func viewDidLoad() {

    super.viewDidLoad()

    let label = UILabel(frame: CGRect(x: 0, y: 20, width: self.view.bounds.width, height: 21))
    label.textAlignment = NSTextAlignment.Center
    label.backgroundColor = UIColor.greenColor()
    label.text = "Hello World"
    self.view.addSubview(label)

}
```

<a href="http://i.imgur.com/gUpys8C.png"><img src="http://i.imgur.com/gUpys8C.png" height="400"></a>
