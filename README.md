# WTOpenSource
This repo collects in one place references to all my open-source contributions to iOS development.

## General-purpose libraries

##### (2020) [UIViewPreview](https://github.com/wltrup/UIViewPreview)

`UIViewPreview` is a Swift Package Manager package for iOS 13.0 and above, tvOS 13.0 and above, watchOS 6.0 and above, and macOS 10.15 and above, that enables `UIKit` development on *macOS Catalina* to take advantage of `SwiftUI` previews in Xcode 11 and above. It's entirely *not* my idea but, rather, just a wrapper for the [code written by matt, of NSHipster fame](https://nshipster.com/swiftui-previews/).

---

##### (2020) [ColorExtensions](https://github.com/wltrup/ColorExtensions)

`ColorExtensions` is a Swift Package Manager package for iOS 10.0 and above, iPadOS 10.0 and above, and watchOS 5.0 and above providing a variety of useful extensions to UIColor.

---

##### (2020) [Assets](https://github.com/wltrup/Assets) and [AssetsPre13](https://github.com/wltrup/AssetsPre13)

`Assets` is an iOS framework that makes concrete use of [AssetCatalogAware](https://github.com/wltrup/AssetCatalogAware) to provide a self-contained collection of assets and easy access to them. UIKit and SwiftUI example projects are included. The *pre13* variant supports legacy systems with versions below 13.0.

---

##### (2020) [AssetCatalogAware](https://github.com/wltrup/AssetCatalogAware) and [AssetCatalogAwarePre13](https://github.com/wltrup/AssetCatalogAwarePre13)

`AssetCatalogAware` is a Swift Package Manager package for iOS defining a collection of protocols and associated protocol extensions to access various kinds of assets, such as colors, images, strings, and fonts, in a type-safe manner. The *pre13* variant supports legacy systems with versions below 13.0.

---

##### (2017) [DrawerKit](https://github.com/Babylonpartners/DrawerKit)
[![Carthage](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)
[![Version](https://img.shields.io/cocoapods/v/DrawerKit.svg?style=flat)](http://cocoapods.org/pods/DrawerKit)
[![Platform](https://img.shields.io/cocoapods/p/DrawerKit.svg?style=flat)](http://cocoapods.org/pods/DrawerKit)
[![Swift 4.0.x](https://img.shields.io/badge/Swift-4.0.x-orange.svg)](https://swift.org)
[![Xcode](https://img.shields.io/badge/Xcode-9.x-blue.svg)](https://developer.apple.com/xcode)
[![License](https://img.shields.io/cocoapods/l/DrawerKit.svg?style=flat)](http://cocoapods.org/pods/DrawerKit)

`DrawerKit` lets an arbitrary view controller modally present another arbitrary view controller in a manner similar to the way the Maps app works. I wrote this
as part of a much bigger project we're working on at [Babylon](https://github.com/Babylonpartners).

(2019) Please note that I am no longer actively involved with this project.

---

##### (2017) [WTAutoLayoutExtensions](https://github.com/wltrup/iOS-Swift-WTAutoLayoutExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/iOS-Swift-WTAutoLayoutExtensions.svg?style=flat)](https://travis-ci.org/iOS-Swift-wltrup/WTAutoLayoutExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTAutoLayoutExtensions.svg?style=flat)](http://cocoapods.org/pods/WTAutoLayoutExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTAutoLayoutExtensions.svg?style=flat)](https://developer.apple.com)
[![Swift](https://img.shields.io/badge/Swift-3.0-orange.svg)](https://swift.org)
[![Xcode](https://img.shields.io/badge/Xcode-8.2-blue.svg)](https://developer.apple.com/xcode)
[![License](https://img.shields.io/cocoapods/l/WTAutoLayoutExtensions.svg?style=flat)](https://github.com/wltrup/iOS-Swift-WTAutoLayoutExtensions/blob/master/LICENSE)

Extensions to `UIView` and `UILayoutGuide` to make it simpler and more natural to use layout guides, layout anchors, and the rest of the auto-layout machinery, with a consistent API and very little code.

---

##### (2016) [Typed Notifications](https://github.com/wltrup/Swift-Typed-Notifications)
Not really a library on its own but merely an idea or suggestion on how to handle notifications, especially custom ones, in a more type-safe way.

---

##### (2016) [WTOnlineLinearRegression](https://github.com/wltrup/Swift-WTOnlineLinearRegression)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTOnlineLinearRegression.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTOnlineLinearRegression)
[![Version](https://img.shields.io/cocoapods/v/WTOnlineLinearRegression.svg?style=flat)](http://cocoapods.org/pods/WTOnlineLinearRegression)
[![Platform](https://img.shields.io/cocoapods/p/WTOnlineLinearRegression.svg?style=flat)](http://cocoapods.org/pods/WTOnlineLinearRegression)
[![Swift](https://img.shields.io/badge/Swift-3.0-orange.svg)](https://swift.org)
[![Xcode](https://img.shields.io/badge/Xcode-8.2-blue.svg)](https://developer.apple.com/xcode)
[![License](https://img.shields.io/cocoapods/l/WTOnlineLinearRegression.svg?style=flat)](http://cocoapods.org/pods/WTOnlineLinearRegression)

`WTOnlineLinearRegression` lets you perform linear regression on one-dimensional data, with or without
variances in the dependent quantity, with the option to maintain a history of all observations as full
snapshots of the results of the regression at the time the items were added to, or removed from, the data set.

---

##### (2016) [WTCoreGraphicsExtensions](https://github.com/wltrup/Swift-WTCoreGraphicsExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTCoreGraphicsExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTCoreGraphicsExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)
[![License](https://img.shields.io/cocoapods/l/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)

A collection of useful additions to `CGGradient`, `CGPoint` and, especially, `CGVector`. If you write 2d games
using `CGVector`, you'll definitely love this library.

## iOS demo apps

##### (2016) [WTOnlineLinearRegression demo app](https://github.com/wltrup/iOS-Swift-WTOnlineLinearRegressionDemo)
An app showing the [`WTOnlineLinearRegression`](https://github.com/wltrup/Swift-WTOnlineLinearRegression) library.

![demo](https://github.com/wltrup/WTOpenSource/blob/master/LinearRegressionDemo.gif)

##### (2016) [Kaleidoscope](https://github.com/wltrup/iOS-Swift-Kaleidoscope)
A simulation of a [**kaleidoscope**](https://en.wikipedia.org/wiki/Kaleidoscope), using `UIKit Dynamics`. Something I wrote in a few days when I was bored.

![demo](https://github.com/wltrup/WTOpenSource/blob/master/KalDemo.gif)

## Deprecated projects

##### (2016-2017) [WTUIColorExtensions](https://github.com/wltrup/iOS-Swift-WTUIColorExtensions) - **DEPRECATED**
[![CI Status](http://img.shields.io/travis/wltrup/iOS-Swift-WTUIColorExtensions.svg?style=flat)](https://travis-ci.org/wltrup/iOS-Swift-WTUIColorExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTUIColorExtensions.svg?style=flat)](http://cocoapods.org/pods/WTUIColorExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTUIColorExtensions.svg?style=flat)](http://cocoapods.org/pods/WTUIColorExtensions)
[![License](https://img.shields.io/cocoapods/l/WTUIColorExtensions.svg?style=flat)](http://cocoapods.org/pods/WTUIColorExtensions)

An extension to `UIColor` adding the ability to generate pseudo-random color instances plus some other goodies. New in **1.1.0** is the support for:
- finding the hexadecimal representation of an RGB color
- finding the approximate luminance of a color
- finding the most contrasting color to a given color

As of 2020.02.21, this project is deprecated and is replaced by [ColorExtensions](https://github.com/wltrup/ColorExtensions).

---

##### (2017) [WTUniquePrimitiveType](https://github.com/wltrup/Swift-WTUniquePrimitiveType) - **DEPRECATED**
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTUniquePrimitiveType.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTUniquePrimitiveType)
[![Version](https://img.shields.io/cocoapods/v/WTUniquePrimitiveType.svg?style=flat)](http://cocoapods.org/pods/WTUniquePrimitiveType)
[![Platform](https://img.shields.io/cocoapods/p/WTUniquePrimitiveType.svg?style=flat)](http://cocoapods.org/pods/WTUniquePrimitiveType)
[![Swift](https://img.shields.io/badge/Swift-3.1-orange.svg)](https://swift.org)
[![Xcode](https://img.shields.io/badge/Xcode-8.3-blue.svg)](https://developer.apple.com/xcode)
[![License](https://img.shields.io/cocoapods/l/WTUniquePrimitiveType.svg?style=flat)](http://cocoapods.org/pods/WTUniquePrimitiveType)

A library to allow you to create distinct types based on the same primitive value so the compiler will warn you if, for example, you accidentally confuse the user name with the user password or the user email address, since they're all based on the same primitive type, namely, `String`.

(2019.11.30) Please note that I've deprecated this project. A much better approach - [Tagged](https://github.com/pointfreeco/swift-tagged) - was devised by Brandon Williams and Stephen Celis, the folks at [pointfree](https://www.pointfree.co). You can watch the episode on it [here](https://www.pointfree.co/episodes/ep12-tagged).

---

##### (2016) [WTBinaryFloatingPointExtensions](https://github.com/wltrup/Swift-WTBinaryFloatingPointExtensions) - **DEPRECATED**
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTBinaryFloatingPointExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTBinaryFloatingPointExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTBinaryFloatingPointExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBinaryFloatingPointExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTBinaryFloatingPointExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBinaryFloatingPointExtensions)
[![License](https://img.shields.io/cocoapods/l/WTBinaryFloatingPointExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBinaryFloatingPointExtensions)

An extension to all types conforming to the `BinaryFloatingPoint` protocol, adding the ability to generate pseudo-random values and to convert between degrees and radians.

2019.11.30: This project has been **deprecated** since the Swift Standard Library now has (part of) the functionality that this library provides. The remaining functionality - the trigonometry-associated one - isn't so hard to implement on a case-by-case basis.

---

##### (2016) [WTIntExtensions](https://github.com/wltrup/Swift-WTIntExtensions) - **DEPRECATED**
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTIntExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTIntExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTIntExtensions.svg?style=flat)](http://cocoapods.org/pods/WTIntExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTIntExtensions.svg?style=flat)](http://cocoapods.org/pods/WTIntExtensions)
[![License](https://img.shields.io/cocoapods/l/WTIntExtensions.svg?style=flat)](http://cocoapods.org/pods/WTIntExtensions)

An extension to `Int` to generate uniformly-distributed pseudo-random integers.

2019.11.30: This project has been **deprecated** since the Swift Standard Library now has precisely the functionality that this library provides.

---

##### (2016) [WTBoolExtensions](https://github.com/wltrup/Swift-WTBoolExtensions) - **DEPRECATED**
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTBoolExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTBoolExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTBoolExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBoolExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTBoolExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBoolExtensions)
[![License](https://img.shields.io/cocoapods/l/WTBoolExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBoolExtensions)

An extension to `Bool` adding a method to generate uniformly-distributed pseudo-random booleans.

2019.11.30: This project has been **deprecated** since the Swift Standard Library now has precisely the functionality that this library provides.

---

##### (2014) [CGExtensions](https://github.com/wltrup/iOS-Swift-CGExtensions) - **DEPRECATED**
A `Swift` collection of useful extensions to `CGFloat`, `CGPoint`, and `CGVector`, plus test suites. If you need 2-dimensional vectors then you'll want this.

This library has been deprecated and replaced by separate libraries compatible with Swift 3.0. Please refer to the more recent ones listed above.

---

##### (2015) [Circular Progress View](https://github.com/wltrup/iOS-Swift-Circular-Progress-View) - **DEPRECATED**
A fully customisable `Swift` class for a progress view similar to what the _Apple Watch_ has.
This is probably still useful as a learning reference but not for actual use in an app.
