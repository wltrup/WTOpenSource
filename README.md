# WTOpenSource
This repo collects in one place references to all my open-source contributions to iOS development.

## General-purpose libraries

##### (2017) [WTUniquePrimitiveType](https://github.com/wltrup/Swift-WTUniquePrimitiveType)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTUniquePrimitiveType.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTUniquePrimitiveType)
[![Version](https://img.shields.io/cocoapods/v/WTUniquePrimitiveType.svg?style=flat)](http://cocoapods.org/pods/WTUniquePrimitiveType)
[![Platform](https://img.shields.io/cocoapods/p/WTUniquePrimitiveType.svg?style=flat)](http://cocoapods.org/pods/WTUniquePrimitiveType)
[![Swift](https://img.shields.io/badge/Swift-3.1-orange.svg)](https://swift.org)
[![Xcode](https://img.shields.io/badge/Xcode-8.3-blue.svg)](https://developer.apple.com/xcode)
[![License](https://img.shields.io/cocoapods/l/WTUniquePrimitiveType.svg?style=flat)](http://cocoapods.org/pods/WTUniquePrimitiveType)

A library to allow you to create distinct types based on the same primitive value so the compiler will warn you if, for example, you accidentally confuse the user name with the user password or the user email address, since they're all based on the same primitive type, namely, `String`.

##### (2017) [WTAutoLayoutExtensions](https://github.com/wltrup/iOS-Swift-WTAutoLayoutExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/iOS-Swift-WTAutoLayoutExtensions.svg?style=flat)](https://travis-ci.org/iOS-Swift-wltrup/WTAutoLayoutExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTAutoLayoutExtensions.svg?style=flat)](http://cocoapods.org/pods/WTAutoLayoutExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTAutoLayoutExtensions.svg?style=flat)](https://developer.apple.com)
[![Swift](https://img.shields.io/badge/Swift-3.0-orange.svg)](https://swift.org)
[![Xcode](https://img.shields.io/badge/Xcode-8.2-blue.svg)](https://developer.apple.com/xcode)
[![License](https://img.shields.io/cocoapods/l/WTAutoLayoutExtensions.svg?style=flat)](https://github.com/wltrup/iOS-Swift-WTAutoLayoutExtensions/blob/master/LICENSE)

Extensions to `UIView` and `UILayoutGuide` to make it simpler and more natural to use layout guides, layout anchors, and the rest of the auto-layout machinery, with a consistent API and very little code.

##### (2016-2017) [WTUIColorExtensions](https://github.com/wltrup/iOS-Swift-WTUIColorExtensions) [![CI Status](http://img.shields.io/travis/wltrup/iOS-Swift-WTUIColorExtensions.svg?style=flat)](https://travis-ci.org/wltrup/iOS-Swift-WTUIColorExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTUIColorExtensions.svg?style=flat)](http://cocoapods.org/pods/WTUIColorExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTUIColorExtensions.svg?style=flat)](http://cocoapods.org/pods/WTUIColorExtensions)
[![License](https://img.shields.io/cocoapods/l/WTUIColorExtensions.svg?style=flat)](http://cocoapods.org/pods/WTUIColorExtensions)

An extension to `UIColor` adding the ability to generate pseudo-random color instances plus some other goodies. New in **1.1.0** is the support for:
- finding the hexadecimal representation of an RGB color
- finding the approximate luminance of a color
- finding the most contrasting color to a given color

##### (2016) [Typed Notifications](https://github.com/wltrup/Swift-Typed-Notifications)
Not really a library on its own but merely an idea or suggestion on how to handle notifications, especially custom ones, in a more type-safe way.

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

##### (2016) [WTCoreGraphicsExtensions](https://github.com/wltrup/Swift-WTCoreGraphicsExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTCoreGraphicsExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTCoreGraphicsExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)
[![License](https://img.shields.io/cocoapods/l/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)

A collection of useful additions to `CGGradient`, `CGPoint` and, especially, `CGVector`. If you write 2d games
using `CGVector`, you'll definitely love this library.

##### (2016) [WTBinaryFloatingPointExtensions](https://github.com/wltrup/Swift-WTBinaryFloatingPointExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTBinaryFloatingPointExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTBinaryFloatingPointExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTBinaryFloatingPointExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBinaryFloatingPointExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTBinaryFloatingPointExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBinaryFloatingPointExtensions)
[![License](https://img.shields.io/cocoapods/l/WTBinaryFloatingPointExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBinaryFloatingPointExtensions)

An extension to all types conforming to the `BinaryFloatingPoint` protocol, adding the ability to generate pseudo-random values and to convert between degrees and radians.

##### (2016) [WTIntExtensions](https://github.com/wltrup/Swift-WTIntExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTIntExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTIntExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTIntExtensions.svg?style=flat)](http://cocoapods.org/pods/WTIntExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTIntExtensions.svg?style=flat)](http://cocoapods.org/pods/WTIntExtensions)
[![License](https://img.shields.io/cocoapods/l/WTIntExtensions.svg?style=flat)](http://cocoapods.org/pods/WTIntExtensions)

An extension to `Int` to generate uniformly-distributed pseudo-random integers.

##### (2016) [WTBoolExtensions](https://github.com/wltrup/Swift-WTBoolExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTBoolExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTBoolExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTBoolExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBoolExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTBoolExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBoolExtensions)
[![License](https://img.shields.io/cocoapods/l/WTBoolExtensions.svg?style=flat)](http://cocoapods.org/pods/WTBoolExtensions)

An extension to `Bool` adding a method to generate uniformly-distributed pseudo-random booleans.

##### (2014) [CGExtensions](https://github.com/wltrup/iOS-Swift-CGExtensions) - **DEPRECATED**
A `Swift` collection of useful extensions to `CGFloat`, `CGPoint`, and `CGVector`, plus test suites. If you need 2-dimensional vectors then you'll want this.

This library has been deprecated and replaced by separate libraries compatible with Swift 3.0. Please refer to the more recent ones listed above.

## iOS demo apps

##### (2016) [WTOnlineLinearRegression demo app](https://github.com/wltrup/iOS-Swift-WTOnlineLinearRegressionDemo)
An app showing the [`WTOnlineLinearRegression`](https://github.com/wltrup/Swift-WTOnlineLinearRegression) library.

![demo](https://github.com/wltrup/WTOpenSource/blob/master/LinearRegressionDemo.gif)

##### (2016) [Kaleidoscope](https://github.com/wltrup/iOS-Swift-Kaleidoscope)
A simulation of a [**kaleidoscope**](https://en.wikipedia.org/wiki/Kaleidoscope), using `UIKit Dynamics`. Something I wrote in a few days when I was bored.

![demo](https://github.com/wltrup/WTOpenSource/blob/master/KalDemo.gif)

## iOS UI contributions

##### (2015) [Circular Progress View](https://github.com/wltrup/iOS-Swift-Circular-Progress-View) - **DEPRECATED**
A fully customisable `Swift` class for a progress view similar to what the _Apple Watch_ has.
This is probably still useful as a learning reference but not for actual use in an app.

