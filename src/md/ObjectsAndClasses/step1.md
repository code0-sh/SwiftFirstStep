```swift
class Shap {
  var numberOfSides = 0
  func simpleDescription() -> String {
    return "A shape with \(numberOfSides) sides."
  }
}

var shape = Shap()
shape.numberOfSides = 7
var shapeDescription = shape.simpleDescription()
```