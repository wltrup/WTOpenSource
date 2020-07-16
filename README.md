# WTOpenSource
This repo collects in one place references to all my open-source contributions to iOS development.

## Main Sections

* [SwiftUI](https://github.com/wltrup/WTOpenSource#swiftui)
* [General-purpose libraries](https://github.com/wltrup/WTOpenSource#general-purpose-libraries)
* [iOS demo apps](https://github.com/wltrup/WTOpenSource#ios-demo-apps)
* [Deprecated projects](https://github.com/wltrup/WTOpenSource#deprecated-projects)

## SwiftUI [top](https://github.com/wltrup/WTOpenSource#main-sections)]

##### (2020)-(**SwiftUI**) [Animated Tab Bar](https://github.com/wltrup/TabBarExample)

## General-purpose libraries [top](https://github.com/wltrup/WTOpenSource#main-sections)]

##### (2020)-(**Math**) [CubicLookupTable](https://github.com/wltrup/CubicLookupTable)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/CubicLookupTable)
![GitHub](https://img.shields.io/github/license/wltrup/CubicLookupTable)

**CubicLookupTable** is a Swift Package Manager package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  that efficiently implements a generic (in the Swift sense) *cubic*-interpolated and dynamically-sampled look-up table: given a function `f(x)` and its derivative `f'(x)`, a table is built that stores values of `x`,  `f(x)`, and `f'(x)` at specific points in some interval `[a,b]` provided by the client code. The derivative is necessary to dynamically determine  where to sample `f(x)` for maximum efficiency and accuracy.

For a *linearly*-interpolated version of this package, head to [LinearLookupTable](https://github.com/wltrup/LinearLookupTable).

Which one should you choose to use? That depends entirely on your needs. The main advantage of a linearly-interpolated table is that it's cheaper, both computationally and memory-wise, than a cubic-interpolated table but it's also less accurate for the same table size. Also, linear interpolation does not preserve the continuity of the interpolated function's derivative. If that's important to you, you should use a cubic-interpolated table.

As a useful example in itself, the package also provides the `CubicTrigTable` type, which implements look-up tables for both `sin(x)` and `cos(x)`.

Lastly, for a mathematical description of the details involved in building these tables, you may want to take a look at [Designing and building efficient look-up tables](./lookup_tables.pdf).

---

##### (2020)-(**Math**) [LinearLookupTable](https://github.com/wltrup/LinearLookupTable)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/LinearLookupTable)
![GitHub](https://img.shields.io/github/license/wltrup/LinearLookupTable)

**LinearLookupTable** is a Swift Package Manager package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  that efficiently implements a generic (in the Swift sense) *linearly*-interpolated and dynamically-sampled look-up table: given a function `f(x)` and its derivative `f'(x)`, a table is built that stores values of `x` and `f(x)` at specific points in some interval `[a,b]` provided by the client code. The derivative is necessary to dynamically determine  where to sample `f(x)` for maximum efficiency and accuracy.

For a *cubic*-interpolated version of this package, head to [CubicLookupTable](https://github.com/wltrup/CubicLookupTable).

Which one should you choose to use? That depends entirely on your needs. The main advantage of a linearly-interpolated table is that it's cheaper, both computationally and memory-wise, than a cubic-interpolated table but it's also less accurate for the same table size. Also, linear interpolation does not preserve the continuity of the interpolated function's derivative. If that's important to you, you should use a cubic-interpolated table.

As a useful example in itself, the package also provides the `LinearTrigTable` type, which implements look-up tables for both `sin(x)` and `cos(x)`.

Lastly, for a mathematical description of the details involved in building these tables, you may want to take a look at [Designing and building efficient look-up tables](./lookup_tables.pdf).

---

##### (2020)-(**Foundation**) [RandomAccessCollectionBinarySearch](https://github.com/wltrup/RandomAccessCollectionBinarySearch)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/RandomAccessCollectionBinarySearch)
![GitHub](https://img.shields.io/github/license/wltrup/RandomAccessCollectionBinarySearch)

**RandomAccessCollectionBinarySearch** is a Swift Package Manager package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  implementing an extension to `RandomAccessCollection` to add support for performing binary searches on sorted collections.

In particular, in addition to the "normal" binary search, the package provides a version that also returns the indices of the values "bracketing" the value being searched for, with sensible results in all possible situations.

---

##### (2020)-(**UI**) [TabularView](https://github.com/wltrup/TabularView) and [TabularViewDemo](https://github.com/wltrup/TabularViewDemo)
![](https://img.shields.io/badge/platforms-iOS/iPadOS%2013%20-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.2-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/TabularView)
![GitHub](https://img.shields.io/github/license/wltrup/TabularView)

![](https://img.shields.io/badge/platforms-iOS/iPadOS%2013%20-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.2-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/TabularViewDemo)
![GitHub](https://img.shields.io/github/license/wltrup/TabularViewDemo)

**TabularView** is a Swift package for iOS/iPadOS (13.0 and above) to display tabular data in a view, in a manner similar to how `UICollectionView` can display unidimensional data in a grid.

The package supports multiple columns, each with their own optional header and optional footer, indexed by an enumeration type, that *you* define, rather than an integer, so your code is clearer about which column or columns it refers to. There's also built-in support for sorting rows by a selected column.

The design philosophy is inspired heavily by how `UICollectionView` works. There are separate data source and delegate protocols (in fact, *two* delegate protocols, one for layout and another for sorting), and the data source is managed using the new (as of 2019) `UICollectionView` [*Diffable Data Source*](https://developer.apple.com/documentation/uikit/uicollectionviewdiffabledatasource) API.

---

##### (2019)-(**Math**) [BiasedDie](https://github.com/wltrup/BiasedDie)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/BiasedDie)
![GitHub](https://img.shields.io/github/license/wltrup/BiasedDie)

**BiasedDie** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  defining a generator of pseudo-random numbers based on a discrete distribution of probabilities.

In less formal terms, imagine that you have a die with `N` faces and that each face has a potentially different probability of being landed on than other faces. In other words, the `k`-th face has a probablity `pk` of being landed on, for `1 ≤ k ≤ N`. Of course, the sum of all of these probabilities must equal 1. This is referred to as a *biased die*. Now imagine that you throw this biased die many times, recording each time the number of the face the die lands on. This package lets you generate a sequence of such numbers as if you had actually thrown such a die, and does so as efficiently as possible, using a method known as the *alias method*. An excellent exposition of this method can be found [here](http://www.keithschwarz.com/darts-dice-coins/).

The package lets you initialise the biased die in multiple ways, depending on the kind of data you have or want to produce.

---

##### (2019)-(**Math**) [Combinatorics](https://github.com/wltrup/Combinatorics)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/Combinatorics)
![GitHub](https://img.shields.io/github/license/wltrup/Combinatorics)

**Combinatorics** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining functions to efficiently compute permutations and combinations of given elements, as well as factorials and binomial coefficients.

---

##### (2019)-(**Math**) [NumberTheory](https://github.com/wltrup/NumberTheory)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/NumberTheory)
![GitHub](https://img.shields.io/github/license/wltrup/NumberTheory)

**NumberTheory** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining a few simple functions to perform common number-theoretic operations, such as *gcd* and *lcm*.

---

##### (2019)-(**Foundation**) [ArrayTransposition](https://github.com/wltrup/ArrayTransposition)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/ArrayTransposition)
![GitHub](https://img.shields.io/github/license/wltrup/ArrayTransposition)

**ArrayTransposition** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, adding an extension to `Array` to allow the computation of *matrix transpositions*.

---

##### (2019)-(**Foundation**) [StringFormatting](https://github.com/wltrup/StringFormatting)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/StringFormatting)
![GitHub](https://img.shields.io/github/license/wltrup/StringFormatting)

**StringFormatting** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining some useful functions for formatting strings.

---

##### (2019)-(**Foundation**) [BinaryIntegerFormatting](https://github.com/wltrup/BinaryIntegerFormatting)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/BinaryIntegerFormatting)
![GitHub](https://img.shields.io/github/license/wltrup/BinaryIntegerFormatting)

**BinaryIntegerFormatting** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining some useful functions for formatting integers.

Ordinarily, one should use `NumberFormatter` to format numbers but I've found use cases where this package has been more useful, especially when localisation isn't an issue.

---

##### (2019)-(**Foundation** | **Experimental**) [NumericScalar](https://github.com/wltrup/NumericScalar)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/NumericScalar)
![GitHub](https://img.shields.io/github/license/wltrup/NumericScalar)

**NumericScalar** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining two protocols, `NumericScalar` and `ValueConvertibleNumericScalar`.

`NumericScalar` adds a number of useful static computed properties that allow for the identification of a numeric type in terms of its explicit type. This is useful in generic algorithms that, nonetheless, sometimes need to behave differently depending on the specific numeric type at hand.

`ValueConvertibleNumericScalar` adds a function to convert an instance of a type conforming  to `NumericScalar` into another. This is easier to use and more uniform than trying to figure out which initialiser to use in any particular case.

Note: This is an *experimental* package.

---

##### (2019)-(**Foundation**) [CollectionSplitting](https://github.com/wltrup/CollectionSplitting)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/CollectionSplitting)
![GitHub](https://img.shields.io/github/license/wltrup/CollectionSplitting)

**CollectionSplitting** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, adding an extension to `Collection` in order to define a function that splits the collection into an array of sub-sequences of equal length.

---

##### (2019)-(**Foundation**) [CollectionDuplicateRemoval](https://github.com/wltrup/CollectionDuplicateRemoval)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/CollectionDuplicateRemoval)
![GitHub](https://img.shields.io/github/license/wltrup/CollectionDuplicateRemoval)

**CollectionDuplicateRemoval** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, adding protocol extensions to `Collection` in order to define a function that returns an array of the elements of the collection, with duplicates removed.

---

##### (2019)-(**Foundation**) [CollectionComparable](https://github.com/wltrup/CollectionComparable)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/CollectionComparable)
![GitHub](https://img.shields.io/github/license/wltrup/CollectionComparable)

**CollectionComparable** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, adding a protocol extension to `Collection` so that it's `Comparable` when its `Element` type is `Comparable`.

---

##### (2019)-(**Foundation**) [CollectionConvenience](https://github.com/wltrup/CollectionConvenience)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/CollectionConvenience)
![GitHub](https://img.shields.io/github/license/wltrup/CollectionConvenience)

**CollectionConvenience** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, adding a protocol extension to `Collection` to define the computed property `isNotEmpty`. It may seem redundant but it sometimes does make for cleaner code.

---

##### (2019)-(**Foundation**) [BoolConvenience](https://github.com/wltrup/BoolConvenience)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/BoolConvenience)
![GitHub](https://img.shields.io/github/license/wltrup/BoolConvenience)

**BoolConvenience** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, adding an extension to `Bool` to define two computed properties, `isTrue` and `isFalse`. These may seem redundant but they sometimes do make for cleaner code.

---

##### (2019)-(**Foundation**) [DictionarySorting](https://github.com/wltrup/DictionarySorting)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/DictionarySorting)
![GitHub](https://img.shields.io/github/license/wltrup/DictionarySorting)

**DictionarySorting** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, implementing an extension to `Dictionary` that provides an easy-to-use and ergonomic "swifty" way to sort a dictionary, as easy as:
```swift
let data = /* ... */ // a dictionary of some kind
let sorted = data.sorted(by: .keys(.ascending)) // returns an array of the elements stored in the
                                                // dictionary, sorted in ascending order of their keys
```

The package provides several such ```sorted(by:)``` functions, depending on whether one or both the dictionary's `Key` and `Value` types conform to `Comparable`.

---

##### (2019)-(**Foundation**) [DictionarySlicing](https://github.com/wltrup/DictionarySlicing)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/DictionarySlicing)
![GitHub](https://img.shields.io/github/license/wltrup/DictionarySlicing)

**DictionarySlicing** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  implementing an extension to `Dictionary` to convert a dictionary into its slice or into an array of its key-value pairs.

---

##### (2019)-(**Other**) [SortOrder](https://github.com/wltrup/SortOrder)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/SortOrder)
![GitHub](https://img.shields.io/github/license/wltrup/SortOrder)

**SortOrder** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  implementing a simple `SortOrder` type.

---

##### (2019)-(**Other**) [JsonSupport](https://github.com/wltrup/JsonSupport)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/JsonSupport)
![GitHub](https://img.shields.io/github/license/wltrup/JsonSupport)

**JsonSupport** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining a few simple functions to perform common operations associated with encoding and decoding **local** JSON files.

---

##### (2019)-(**Other**) [ValueRestriction](https://github.com/wltrup/ValueRestriction)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/ValueRestriction)
![GitHub](https://img.shields.io/github/license/wltrup/ValueRestriction)

**ValueRestriction** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining an enumeration to easily test a numerical value against some condition.

---

##### (2019)-(**Other**) [OperationResult](https://github.com/wltrup/OperationResult)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/OperationResult)
![GitHub](https://img.shields.io/github/license/wltrup/OperationResult)

**OperationResult** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining an enumeration similar to `Result` but with `Array<String>` in place of an error type.

One neat use for this type is when considering a long sequence of numerical operations, some of which may fail. For example, division by zero, logarithm of a non-positive number, arc-sine or arc-cosine of a number with a magnitude larger than 1, and so on. Rather than stop the execution with throw-catches or risk runtime errors, the `OperationResult<A>` type allows a clean progression to the end, accumulating error messages along the way.

---

##### (2019)-(**Other**) [Counter](https://github.com/wltrup/Counter)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/Counter)
![GitHub](https://img.shields.io/github/license/wltrup/Counter)

**Counter** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining a model type to represent an integer counter.

---

##### (2019)-(**Other**) [Either](https://github.com/wltrup/Either)
![](https://img.shields.io/badge/platforms-iOS%2011%20%7C%20tvOS%2011%20%7C%20watchOS%205%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/Either)
![GitHub](https://img.shields.io/github/license/wltrup/Either)

**Either** is a Swift package for iOS/tvOS (11.0 and above), watchOS (5.0 and above), and macOS (10.14 and above), under Swift 5.0 and above,  implementing a simple `Either` type, with a few built-in and useful properties and protocol conformances.

---

##### (2019)-(**Other**) [BinaryChoice](https://github.com/wltrup/BinaryChoice)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%204%20%7C%20macOS%2010.14-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.0-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/BinaryChoice)
![GitHub](https://img.shields.io/github/license/wltrup/BinaryChoice)

**BinaryChoice** is a Swift package for iOS/tvOS (10.0 and above), watchOS (4.0 and above), and macOS (10.14 and above), under Swift 5.0 and above, defining protocols for types that can be initialised from a boolean value and/or can be represented by a boolean value.

---

##### (2019)-(**UI**) [UIViewPreview](https://github.com/wltrup/UIViewPreview)
![](https://img.shields.io/badge/platforms-iOS%2013%20%7C%20tvOS%2013%20%7C%20watchOS%206%20%7C%20macOS%2010.15-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.1-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/UIViewPreview)
![GitHub](https://img.shields.io/github/license/wltrup/UIViewPreview)

`UIViewPreview` is a Swift package enabling `UIKit` development on *macOS Catalina* to take advantage of `SwiftUI` previews in Xcode 11 and above. It's entirely *not* my idea but, rather, just a wrapper for the [code written by matt, of NSHipster fame](https://nshipster.com/swiftui-previews/).

---

##### (2019)-(**UI**) [ColorExtensions](https://github.com/wltrup/ColorExtensions)
![](https://img.shields.io/badge/platforms-iOS%2010%20%7C%20tvOS%2010%20%7C%20watchOS%205-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.1-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/ColorExtensions)
![GitHub](https://img.shields.io/github/license/wltrup/ColorExtensions)

`ColorExtensions` is a Swift package for iOS/tvOS (10.0 and above) and watchOS (5.0 and above) providing a variety of useful extensions to `UIColor`.

---

##### (2019)-(**UI**) [Assets](https://github.com/wltrup/Assets) and [AssetsPre13](https://github.com/wltrup/AssetsPre13)
![](https://img.shields.io/badge/platforms-iOS%2013-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.1-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/Assets)
![GitHub](https://img.shields.io/github/license/wltrup/Assets)

![](https://img.shields.io/badge/platforms-iOS%2011-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.1-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/AssetsPre13)
![GitHub](https://img.shields.io/github/license/wltrup/AssetsPre13)

`Assets` is an iOS framework that makes concrete use of [AssetCatalogAware](https://github.com/wltrup/AssetCatalogAware) to provide a self-contained collection of assets and easy access to them. UIKit and SwiftUI example projects are included. The *pre13* variant supports legacy systems with iOS versions from 11.0 up to but *not* including 13.0.

---

##### (2019)-(**UI**) [AssetCatalogAware](https://github.com/wltrup/AssetCatalogAware) and [AssetCatalogAwarePre13](https://github.com/wltrup/AssetCatalogAwarePre13)
![](https://img.shields.io/badge/platforms-iOS%2013%20%7C%20tvOS%2013%20%7C%20watchOS%206-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.1-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/AssetCatalogAware)
![GitHub](https://img.shields.io/github/license/wltrup/AssetCatalogAware)

![](https://img.shields.io/badge/platforms-iOS%2011%20%7C%20tvOS%2011%20%7C%20watchOS%204-red)
[![Xcode](https://img.shields.io/badge/Xcode-11-blueviolet.svg)](https://developer.apple.com/xcode)
[![Swift](https://img.shields.io/badge/Swift-5.1-orange.svg)](https://swift.org)
![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/wltrup/AssetCatalogAwarePre13)
![GitHub](https://img.shields.io/github/license/wltrup/AssetCatalogAwarePre13)

`AssetCatalogAware` is a Swift package for iOS defining a collection of protocols and associated protocol extensions to access various kinds of assets, such as colors, images, strings, and fonts, in a type-safe manner. The *pre13* variant supports legacy systems with iOS/tvOS versions from 11.0 up to but *not* including 13.0 and watchOS versions from 4.0 up to but *not* including 6.0.

---

##### (2017)-(**UI**) [DrawerKit](https://github.com/Babylonpartners/DrawerKit)
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

##### (2017)-(**UI**) [WTAutoLayoutExtensions](https://github.com/wltrup/iOS-Swift-WTAutoLayoutExtensions)
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

##### (2016)-(**Math**) [WTOnlineLinearRegression](https://github.com/wltrup/Swift-WTOnlineLinearRegression)
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

##### (2016)-(**UI**) [WTCoreGraphicsExtensions](https://github.com/wltrup/Swift-WTCoreGraphicsExtensions)
[![CI Status](http://img.shields.io/travis/wltrup/Swift-WTCoreGraphicsExtensions.svg?style=flat)](https://travis-ci.org/wltrup/Swift-WTCoreGraphicsExtensions)
[![Version](https://img.shields.io/cocoapods/v/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)
[![Platform](https://img.shields.io/cocoapods/p/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)
[![License](https://img.shields.io/cocoapods/l/WTCoreGraphicsExtensions.svg?style=flat)](http://cocoapods.org/pods/WTCoreGraphicsExtensions)

A collection of useful additions to `CGGradient`, `CGPoint` and, especially, `CGVector`. If you write 2d games
using `CGVector`, you'll definitely love this library.

## iOS demo apps [top](https://github.com/wltrup/WTOpenSource#main-sections)]

##### (2016) [WTOnlineLinearRegression demo app](https://github.com/wltrup/iOS-Swift-WTOnlineLinearRegressionDemo)
An app showing the [`WTOnlineLinearRegression`](https://github.com/wltrup/Swift-WTOnlineLinearRegression) library.

![demo](https://github.com/wltrup/WTOpenSource/blob/master/LinearRegressionDemo.gif)

##### (2016) [Kaleidoscope](https://github.com/wltrup/iOS-Swift-Kaleidoscope)
A simulation of a [**kaleidoscope**](https://en.wikipedia.org/wiki/Kaleidoscope), using `UIKit Dynamics`. Something I wrote in a few days when I was bored.

![demo](https://github.com/wltrup/WTOpenSource/blob/master/KalDemo.gif)

## Deprecated projects [top](https://github.com/wltrup/WTOpenSource#main-sections)]

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

##### (2015) [Circular Progress View](https://github.com/wltrup/iOS-Swift-Circular-Progress-View) - **DEPRECATED**
A fully customisable `Swift` class for a progress view similar to what the _Apple Watch_ has.
This is probably still useful as a learning reference but not for actual use in an app.

---

##### (2014) [CGExtensions](https://github.com/wltrup/iOS-Swift-CGExtensions) - **DEPRECATED**
A `Swift` collection of useful extensions to `CGFloat`, `CGPoint`, and `CGVector`, plus test suites. If you need 2-dimensional vectors then you'll want this.

This library has been deprecated and replaced by separate libraries compatible with Swift 3.0. Please refer to the more recent ones listed above.
