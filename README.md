# Haikus in Swift

**Haiku** `[hai·​ku]` *(noun)*: an unrhymed verse form of Japanese origin having three lines containing usually five, seven, and five syllables respectively.

Here are some attempts att Haikus in Swift.

### Meta

```Swift
public struct Haiku {
    let contentLines: Array<String>
    let authorName: String
}
```

```Swift
func read(this: Haiku) {
    for line in this.contentLines {
        read(line: line) // TODO
    }
}
```

### Extend

```Swift
extension Haiku {
    var lines: Array<String> { // For short
        return contentLines
    }
}
```

```Swift
extension Haiku {
    var isValidHaiku: Bool {
        return lines.count == 3
    }
}
```

```Swift
func print(this: Haiku) {
    for index in 0...2 {
        print(this.lines[index])
    }
}
```

### Bonus

```Swift
let view = UIView()
view.translatesAutoresizingMaskIntoConstraints = false
// I failed this Haiku
```

