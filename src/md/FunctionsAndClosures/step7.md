```swift
func hasAnyMatches(list: [Int], condition: Int -> Bool) -> Bool {
  for item in list {
    if condition(item) {
      return true
    }
  }
  return false
}
// Swift3.0
func hasAnyMatches(list: [Int], condition: (Int) -> Bool) -> Bool {
  for item in list {
    if condition(item) {
      return true
    }
  }
  return false
}
func lessThanTen(number: Int) -> Bool {
  return number < 10
}
var numbers = [20, 19, 7, 12]
hasAnyMatches(numbers, condition: lessThanTen)
// Swift3.0
hasAnyMatches(list: numbers, condition: lessThanTen)
```