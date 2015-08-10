```swift
enum OptionalValue<T> {
  case None
  case Some(T)
}
var possibleInteger: OptionalValue<Int> = .None
possibleInteger = .Some(100)
```