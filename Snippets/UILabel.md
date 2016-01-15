# UILabel

```swift
override func viewDidLoad() {

    super.viewDidLoad()

    let label = UILabel(frame: CGRectMake(0, 20, self.view.bounds.width, 21))
    label.textAlignment = NSTextAlignment.Center
    label.backgroundColor = UIColor.greenColor()
    label.text = "Hello World"
    self.view.addSubview(label)

}
```
