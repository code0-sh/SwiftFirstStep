```swift
func makeArray<Item>(item: Item, numberOfTimes: Int) -> [Item] {
  var result = [Item]()
  for _ in 0..<numberOfTimes {
    result.append(item)
  }
  return result
}
makeArray("knock", numberOfTimes:4)
// Swift3.0
makeArray(item: "knock", numberOfTimes:4)
```