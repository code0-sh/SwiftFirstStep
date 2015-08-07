```swift
class Square: NamedShape {
  var sideLength: Double

  init(sideLength: Double, name: String) {
    self.sideLength = sideLength
    super.init(name: name)
    numberOfSides = 4
  }

  func area() -> Double {
    return sideLength * sideLength
  }

  override func simpleDescription() -> String {
    return "A square width sides of length \(sideLength)."
  }
}

let mySquare = Square(sideLength: 5.2, name: "my square")
mySquare.area()
mySquare.simpleDescription()
```