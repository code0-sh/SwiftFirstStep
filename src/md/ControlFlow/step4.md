```swift
let fruit = "mikan"
switch fruit {
case "apple":
  print("What color is this apple?")
case "orange", "kiwi":
  print("sour taste")
case let x where x.hasSuffix("n"):
  print("The last character is n")
default:
  print("default statement")
}
```