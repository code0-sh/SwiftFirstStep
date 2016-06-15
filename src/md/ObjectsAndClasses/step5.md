```swift
var num: Int = 0

class Person {
  let name: String
  var age: Int = 0 {
    willSet {
      print("\(self.age)歳から\(newValue)歳へ年齢を変更します。")
      num += num + 1
      print(num)
    }
    didSet {
      print("didSet\(oldValue)歳から\(self.age)歳へ年齢を変更しました。")
      num += num + 1
      print(num)
    }
  }
  init(name: String, age: Int) {
    self.name = name
    self.age = age
  }
}

let taro = Person(name: "山田太郎", age: 25)
taro.age = 26
```