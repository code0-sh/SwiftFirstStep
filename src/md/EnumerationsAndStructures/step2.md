```swift
class ClassAnimal {
  var name: String = ""
  var age: Int = 0
  init(name: String, age: Int) {
    self.name = name
    self.age = age
  }
}

let classALion = ClassAnimal(name: "ライオン", age: 5)
let classBLion = classALion
classBLion.name = "らいおん"
classALion.name // らいおん

struct StructAnimal {
  var name: String = ""
  var age: Int = 0
  init(name: String, age: Int) {
    self.name = name
    self.age = age
  }
}

let structALion = StructAnimal(name: "ライオン", age: 5)
var structBLion = structALion
structBLion.name = "らいおん"
structALion.name //ライオン
```