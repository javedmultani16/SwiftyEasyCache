# SwiftyEasyCache


## General info

The purpose of the library is to abstract the downloading (images, pdf, zip, etc) and caching of remote resources (images, JSON, XML, etc) so that client code can easily "swap" a URL for any kind of files ( JSON, XML, etc) without worrying about any of the details.

<img width="301" alt="Screenshot 2019-05-18 at 3 09 18 PM" src="https://user-images.githubusercontent.com/16849127/57966145-04378400-7981-11e9-8c2a-be34c1d38e1b.png">

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

```ruby
iOS > 10

Swift 4.2 
```
## Installation

SwiftyEasyCache is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'SwiftyEasyCache'
```

## Manully Installation
To use this library in your project manually you may:

just drag SwiftyEasyCache directory to the project tree

## Usage
To load web images:
```ruby
  uploadedImageView.swifty_setImageWithUrl(url: uploadedImageURL!, completion: {(error) in })
  ```
  To load web images with placeholder image:
  ```ruby
  uploadedImageView.swifty_setImageWithUrl(url: uploadedImageURL!, placeholderImage: UIImage(named: "default-placeholder")) { (err) in
            print(err.debugDescription)
        }
 ```

## Author

Javed Multani, javedmultani16@gmail.com

## License

SwiftyEasyCache is available under the MIT license. See the LICENSE file for more info.
