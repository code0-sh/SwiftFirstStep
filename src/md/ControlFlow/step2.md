```swift
var optionalString: String?
print(optionalString == nil)

var optionalName: String? = "John Appleseed"
var greeting = "Hello!, "
if let name = optionalName { // Optional Binding
  greeting = greeting + name
}
print(greeting)
```