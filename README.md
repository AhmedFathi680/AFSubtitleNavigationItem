# AFSubtitleNavigationItem

[![CI Status](https://img.shields.io/travis/ahmedfathi680@gmail.com/AFSubtitleNavigationItem.svg?style=flat)](https://travis-ci.org/ahmedfathi680@gmail.com/AFSubtitleNavigationItem)
[![Version](https://img.shields.io/cocoapods/v/AFSubtitleNavigationItem.svg?style=flat)](https://cocoapods.org/pods/AFSubtitleNavigationItem)
[![License](https://img.shields.io/cocoapods/l/AFSubtitleNavigationItem.svg?style=flat)](https://cocoapods.org/pods/AFSubtitleNavigationItem)
[![Platform](https://img.shields.io/cocoapods/p/AFSubtitleNavigationItem.svg?style=flat)](https://cocoapods.org/pods/AFSubtitleNavigationItem)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements
Requires iOS 9.0 or later.

## Installation

AFSubtitleNavigationItem is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'AFSubtitleNavigationItem'
```

## Usage

Start by importing  `AFSubtitleNavigationItem` in your `AppDelegate`

In your viewController's `viewDidLoad` method write the below:
```swfit
navigationItem.isSubtitleEnabled = true
navigationItem.titleLabel?.text = "Title"
navigationItem.subtitleLabel?.text = "Subtitle"
```

Make sure this view controller actually have a navigationController, i.e. it's not directly presented without being in a navigation controller stack.
You can also your custom navigation item to your presented view controller and use `AFSubtitleNavigationItem` properties directly.

### Appearance allover the app

You customize all your navigationItems allover the application be easily using the below code:

Customizing titles:

```swift
UINavigationItem.appearance.titleTextColor = .darkGray
UINavigationItem.appearance.titleTextFont = UIFont.systemFont(ofSize: 17, weight: .medium)
UINavigationItem.appearance.titleTextShadowColor = UIColor.black.withAlphaComponent(0.05)
UINavigationItem.appearance.titleTextShadowOffset = CGSize(width: 0.5, height: 0.5)
```

Customizing Subtitles:

```swift
UINavigationItem.appearance.subtitleTextColor = .darkGray
UINavigationItem.appearance.subtitleTextFont = UIFont.systemFont(ofSize: 13, weight: .thin)
UINavigationItem.appearance.subtitleTextShadowColor = UIColor.black.withAlphaComponent(0.05)
UINavigationItem.appearance.subtitleTextShadowOffset = CGSize(width: 1, height: 1)
```

## Author

Ahmed Fathi, AhmedFathi680@gmail.com

## License

AFSubtitleNavigationItem is available under the MIT license. See the LICENSE file for more info.