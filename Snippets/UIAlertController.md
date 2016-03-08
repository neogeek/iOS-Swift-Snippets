# UIAlertController

```swift
import UIKit

class ViewController: UIViewController {

    @IBAction func enterName(sender: AnyObject) {

        let alert = UIAlertController(title: "Enter Name", message: nil, preferredStyle: .Alert)

        alert.addTextFieldWithConfigurationHandler({ (textField) -> Void in
            textField.text = ""
            textField.autocapitalizationType = .Sentences;
        })

        alert.addAction(UIAlertAction(title: "OK", style: .Default, handler: { (action) -> Void in
            let textField = alert.textFields![0] as UITextField
            print(textField.text!)
        }))

        alert.addAction(UIAlertAction(title: "Cancel", style: .Cancel, handler: {
            (alertAction: UIAlertAction!) in
            alert.dismissViewControllerAnimated(true, completion: nil)
        }))

        self.presentViewController(alert, animated: true, completion: nil)

    }

}
```

<a href="http://i.imgur.com/8NP8fRJ.png"><img src="http://i.imgur.com/8NP8fRJ.png" height="400"></a>
