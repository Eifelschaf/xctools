<img src="Assets/header.png" width="400"/><br/>

<img src="https://img.shields.io/badge/package%20managers-SwiftPM-yellow.svg"/>
<a href="https://github.com/xcodeswift/xctools/releases">
  <img src="https://img.shields.io/github/release/xcodeswift/xcode.svg"/>
</a>
<a href="https://travis-ci.org/xcodeswift/xctools">
  <img src="https://img.shields.io/travis/xcodeswift/xctools/master.svg?style=flat"/>
</a>
<a href="https://github.com/xcodeswift/xctools/blob/master/LICENSE">
  <img src="https://img.shields.io/github/license/mashape/apistatus.svg"/>
</a>
<a href="http://xcodeswift.herokuapp.com/">
  <img src="https://xcodeswift.herokuapp.com/badge.svg">
</a>
<a href="https://twitter.com/xcodedotswift">
  <img src="https://img.shields.io/badge/contact-@xcodedotswift-blue.svg?style=flat" alt="Twitter: @xcodedotswift" />
</a>

A set of command line tools to interact with your Xcode projects.

## Install

You can easily install xctools with Homebrew:

```
brew tap xcodeswift/xctools git@github.com:xcodeswift/xctools.git
brew install xctools
```

You can also easily run the tool using [🌱 Mint](https://github.com/yonaskolb/mint):

```bash
mint run xcodeswift/xctools
```

## Setup

1. Git clone the repository `git clone git@github.com:xcodeswift/xctools.git`
2. Build with `swift build`

## Usage

You can check the available commands by just running `xctools` from the console.

#### Frameworks

##### Embed
It embeds your frameworks, their symbols, and the bcsymbolmap files into your built product stripping all the unnecessary architectures. This command should be used from a Xcode build phase as shown in the screenshot below:

![Xcode build phase using the command to embed the frameworks](Assets/Frameworks-Embed.png)

##### Strip
It strips architectures from your frameworks:

```
xctools frameworks strip MyFramework.framework --archs armv7
```

## References

- [Speeding Up Custom Script Phases](http://indiestack.com/2014/12/speeding-up-custom-script-phases/)
- [Carthage copy frameworks](https://github.com/Carthage/Carthage/blob/master/Source/carthage/CopyFrameworks.swift)
- [CocoaPods embed frameworks script](https://github.com/CocoaPods/CocoaPods/blob/master/lib/cocoapods/generator/embed_frameworks_script.rb)
- [Commander](https://github.com/kylef/Commander)
- [PlistBuddy](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man8/PlistBuddy.8.html)

## Contributors :heart:

[<img alt="pepibumur" src="https://avatars3.githubusercontent.com/u/663605?v=4&s=117" width="117">](https://github.com/pepibumur)

## License

```
MIT License

Copyright (c) 2017 xcode.swift

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
