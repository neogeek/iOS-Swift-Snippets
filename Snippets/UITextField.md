# UITextField

```swift
override func viewDidLoad() {

    super.viewDidLoad()

    let textField = UITextField(frame: CGRectMake(0, 20, self.view.bounds.width, 21))
    textField.borderStyle = UITextBorderStyle.Line
    textField.placeholder = "Email address"
    self.view.addSubview(textField)

}
```

<a href="http://i.imgur.com/0Ru6S88.png"><img src="http://i.imgur.com/0Ru6S88.png" height="400"></a>
