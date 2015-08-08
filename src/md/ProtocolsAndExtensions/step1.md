```swift
protocol ExampleProtocol {
  var simpleDescription: String {get}
  mutating func adjust()
}

class SimpleClass: ExampleProtocol {
  var simpleDescription: String = "A very simple class."
  var anotherProperty: Int = 69105
  func adjust() {
    simpleDescription += " Now 100% adjusted."
  }
}

let simpleClass = SimpleClass()
let simpleClassInitDescription = simpleClass.simpleDescription
simpleClass.adjust()
let simpleClassChangedDescription = simpleClass.simpleDescription


struct SimpleStructure: ExampleProtocol {
  var simpleDescription: String = "A simple structure"
  mutating func adjust() {
    simpleDescription += "(adjusted)"
  }
}

var simpleStructure = SimpleStructure()
let simpleStructureInitDescription = simpleStructure.simpleDescription
simpleStructure.adjust()
let simpleStructureChangedDescription = simpleStructure.simpleDescription
```