# UIButton

```swift
override func viewDidLoad() {

    super.viewDidLoad()

    let button = UIButton(frame: CGRect(x: 0, y: 20, width: 100, height: 21))
    button.setTitle("Hello World!", forState: UIControlState.Normal)
    button.setTitleColor(UIColor.blackColor(), forState: UIControlState.Normal)
    button.backgroundColor = UIColor.greenColor()
    button.addTarget(self, action: "pressed:", forControlEvents: UIControlEvents.TouchUpInside)
    self.view.addSubview(button)

}

func pressed(sender: UIButton!) {

    print(sender.titleLabel!.text!)

}
```

<a href="http://i.imgur.com/TVPFB8j.png"><img src="http://i.imgur.com/TVPFB8j.png" height="400"></a>
