# UITableView

```swift
import UIKit

class ViewController: UIViewController, UITableViewDelegate, UITableViewDataSource {

    override func viewDidLoad() {

        super.viewDidLoad()

        let tableView = UITableView(frame: CGRect(x: 0, y: 20, width: self.view.bounds.width, height: self.view.bounds.height - 20), style: UITableViewStyle.Plain)
        tableView.delegate = self
        tableView.dataSource = self
        self.view.addSubview(tableView)

    }

    func tableView(tableView: UITableView, numberOfRowsInSection section: Int) -> Int {

        return 5

    }

    func tableView(tableView: UITableView, cellForRowAtIndexPath indexPath: NSIndexPath) -> UITableViewCell {

        let cell = UITableViewCell(style: UITableViewCellStyle.Default, reuseIdentifier: "Cell")

        cell.textLabel?.text = "Test \(indexPath.row + 1)"

        return cell

    }

    override func viewDidAppear(animated: Bool) {

        self.tableView.reloadData()

    }

}
```

<a href="http://i.imgur.com/1yK2MJI.png"><img src="http://i.imgur.com/1yK2MJI.png" height="400"></a>
