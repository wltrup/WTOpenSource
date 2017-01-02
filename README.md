# WTOpenSource
This repo collects in one place references to all my open-source contributions.

## General-purpose libraries

##### (2016) [Typed Notifications](https://github.com/wltrup/Swift-Typed-Notifications)
Not really a library on its own but merely an idea or suggestion on how to handle notifications, especially custom ones, in a more type-safe way.

##### (2016) [WTOnlineLinearRegression](https://github.com/wltrup/Swift-WTOnlineLinearRegression) **1.0.3**
`WTOnlineLinearRegression` lets you perform linear regression on one-dimensional data, with or without
variances in the dependent quantity, with the option to maintain a history of all observations as full
snapshots of the results of the regression at the time the items were added to, or removed from, the data set.

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

## Swift Extensions

##### (2016-2017) [WTUIColorExtensions](https://github.com/wltrup/iOS-Swift-WTUIColorExtensions) **1.1.0**
An extension to `UIColor` adding the ability to generate pseudo-random color instances plus some other goodies. New in **1.1.0** is the support for:
- finding the hexadecimal representation of an RGB color
- finding the approximate luminance of a color
- finding the most contrasting color to a given color

##### (2016) [WTCoreGraphicsExtensions](https://github.com/wltrup/Swift-WTCoreGraphicsExtensions) **1.0.4**
A collection of useful additions to `CGGradient`, `CGPoint` and, especially, `CGVector`. If you write 2d games
using `CGVector`, you'll definitely love this library.

##### (2016) [WTBinaryFloatingPointExtensions](https://github.com/wltrup/Swift-WTBinaryFloatingPointExtensions) **1.0.2**
An extension to all types conforming to the `BinaryFloatingPoint` protocol, adding the ability to generate pseudo-random values and to convert between degrees and radians.

##### (2016) [WTIntExtensions](https://github.com/wltrup/Swift-WTIntExtensions) **1.0.3**
An extension to `Int` to generate uniformly-distributed pseudo-random integers.

##### (2016) [WTBoolExtensions](https://github.com/wltrup/Swift-WTBoolExtensions) **1.0.2**
An extension to `Bool` adding a method to generate uniformly-distributed pseudo-random booleans.

##### (2014) [CGExtensions](https://github.com/wltrup/iOS-Swift-CGExtensions) - **DEPRECATED**
A `Swift` collection of useful extensions to `CGFloat`, `CGPoint`, and `CGVector`, plus test suites. If you need 2-dimensional vectors then you'll want this.

This library has been deprecated and replaced by separate libraries compatible with Swift 3.0. Please refer to the more recent ones listed above.
