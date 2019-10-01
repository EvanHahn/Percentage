# Percent [![Build Status](https://travis-ci.com/sindresorhus/Percent.svg?branch=master)](https://travis-ci.com/sindresorhus/Percent)

> A percentage type for Swift

Makes percentages more readable and type-safe, for example, for APIs that currently accept a fraction `Double`.

```diff
-.opacity(0.45)
+.opacity(45%)
```


## Install

SwiftPM:

```swift
.package(url: "https://github.com/sindresorhus/Percent", from: "0.0.0")
```

Or just copy-paste it.


## Usage

See the [source](Sources/Percent/Percent.swift) for docs.

```swift
import Percent

10% + 5.5%
//=> 15.5%

(40% + 93%) * 3
//=> 399%

50%.of(200)
//=> 100

Percent(50)
//=> 50%

Percent(fraction: 0.5)
//=> 50%

50%.fraction
//=> 0.5

10%.rawValue
//=> 10
```

The type conforms to `Hashable`, `Codable`, `RawRepresentable`, `Comparable`, and supports all the arithmetic operators.


## FAQ

#### Can you support Carthage and CocoaPods?

No, but you can still use SwiftPM for this package even though you mainly use Carthage or CocoaPods.


## Related

- [Defaults](https://github.com/sindresorhus/Defaults) - Swifty and modern UserDefaults
- [Preferences](https://github.com/sindresorhus/Preferences) - Add a preferences window to your macOS app
- [LaunchAtLogin](https://github.com/sindresorhus/LaunchAtLogin) - Add "Launch at Login" functionality to your macOS app
- [DockProgress](https://github.com/sindresorhus/DockProgress) - Show progress in your app's Dock icon
- [CircularProgress](https://github.com/sindresorhus/CircularProgress) - Circular progress indicator for your macOS app
- [More…](https://github.com/search?q=user%3Asindresorhus+language%3Aswift)
