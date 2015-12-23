CDCodabarView
==================

What is it?
------------------

CDCodabarView is a [Codabar](https://en.wikipedia.org/wiki/Codabar) barcode generator for iOS.

It is written in Swift 2 and uses `IBDesignable`, `IBInspectable` and Core Graphics.


Using Storyboards
------------------

1. Copy the CDCodabarView folder into your project.
2. Drag a UIView into your storyboard.
3. Change the class of the UIView to `CDCodabarView`.
4. Customize your barcode using the inspector.

![alt tag](https://github.com/Coledunsby/CDCodabarView/blob/master/Images/Storyboard.png)

Programmatically
------------------

1. Copy the CDCodabarView folder into your project.

2. Initialize an instance of CDCodaBarViewController using the constructor:

    ```
    let codabarView = CDCodabarView()
    codabarView.frame = CGRect(x: 0, y: 0, width: 200, height: 100)
    codabarView.code = "A12345B"
    codabarView.backgroundColor = .whiteColor()
    ```

4. Customize the barcode.

    ```
    codabarView.barColor = .blueColor()
    codabarView.textColor = .redColor()
    codabarView.padding = 5
    codabarView.hideCode = false
    codabarView.font = UIFont(name: "AvenirNext-Regular", size: 15.0)!
    ```

5. Add the barcode to your view.

    ```
    view.addSubview(codabarView)
    ```




# CDCodabarView

[![CI Status](http://img.shields.io/travis/Cole Dunsby/CDCodabarView.svg?style=flat)](https://travis-ci.org/Cole Dunsby/CDCodabarView)
[![Version](https://img.shields.io/cocoapods/v/CDCodabarView.svg?style=flat)](http://cocoapods.org/pods/CDCodabarView)
[![License](https://img.shields.io/cocoapods/l/CDCodabarView.svg?style=flat)](http://cocoapods.org/pods/CDCodabarView)
[![Platform](https://img.shields.io/cocoapods/p/CDCodabarView.svg?style=flat)](http://cocoapods.org/pods/CDCodabarView)

## Usage

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

CDCodabarView is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "CDCodabarView"
```

## Author

Cole Dunsby, coledunsby@gmail.com

## License

CDCodabarView is available under the MIT license. See the LICENSE file for more info.
