
FadeButton
============
***Fading Buttons for iOS***

[![Build Status](https://api.travis-ci.org/inaka/FadeButton.svg)](https://travis-ci.org/inaka/FadeButton) [![Codecov](https://codecov.io/gh/inaka/FadeButton/branch/master/graph/badge.svg)](https://codecov.io/gh/inaka/jayme) [![Swift](https://img.shields.io/badge/Swift-3.0-orange.svg?style=flat)](https://swift.org/) [![Cocoapods](https://img.shields.io/cocoapods/v/FadeButton.svg)](http://cocoadocs.org/docsets/Jayme) [![Twitter](https://img.shields.io/badge/twitter-@inaka-blue.svg?style=flat)](http://twitter.com/inaka)
Overview
--------
This is just a UIButton subclass to get a fading-out effect after touching a button, done in the simplest way possible.

![Sample](https://raw.githubusercontent.com/inaka/FadeButton/master/Assets/V2/sample.gif)


Usage
-----
**1)** Go to interface builder, select your button, open the Identity Inspector tab, and set its custom class to `FadeButton`.

![Sample](https://raw.githubusercontent.com/inaka/FadeButton/master/Assets/V2/screenshot1.png)

**2)** Also, check out the following attributes in the Attributes Inspector tab:

![Sample](https://raw.githubusercontent.com/inaka/FadeButton/master/Assets/V2/screenshot2.png)

- `fadeDuration` for setting how long the fade effect lasts.
- Then, the properties `textColor`, `image` and `backgroundImage` (that can be different for each state config) will be affected by the fading effect when the transitions between `.normal` state and the `.highlighted` state (and vice versa) occur.
  - For instance, if you set `textColor: .white for: .normal` state and `textColor: .yellow for: .highlighted` state, the user will see a fading text effect from yellow to white after releasing the button.


Sample Project
-------
There's a sample project inside this repo that you can check out in order to have a deeper understanding of the usage of this library.

## Setup

- FadeButton is available via [cocoapods](http://cocoapods.org/). In order to install it, add this line to your `Podfile`:
  - `pod 'FadeButton' ~> '2.0'`
  - Remember to add an `import FadeButton` statement in any source file of your project that needs to make use of the library.

## Older Versions Support

- As of its `2.0.0` release, this library works with [**Swift 3.0**](https://swift.org/blog/swift-3-0-released/)
- If you look for older languages version support, you can check out the `1.0.0` release, that contains the old Objective-C version of the library, which is compatible with older Swift versions.

## Contact Us

For **questions** or **general comments** regarding the use of this library, please use our public [hipchat room](http://inaka.net/hipchat).

If you find any **bug**, a **problem** while using this library, or have **suggestions** that can make it better, please [open an issue](https://github.com/inaka/FadeButton/issues/new) in this repo (or a pull request).

You can also check all of our open-source projects at [inaka.github.io](https://github.com/inaka/Jayme/blob/master/inaka.github.io).