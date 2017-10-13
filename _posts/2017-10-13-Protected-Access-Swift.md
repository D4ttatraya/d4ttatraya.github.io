---
layout: post
comments: true
title: Quickie&#58; Protected Properties and Methods in Swift - An Alternative
---

It's always been a quite demand from swift developers to add `protected` access in [Swift's access control](https://developer.apple.com/library/content/documentation/Swift/Conceptual/Swift_Programming_Language/AccessControl.html). Lot of times it's been asked on stack-overflow that how to write protected methods in swift. But still swift hasn't provided any direct way to do it. Can we really achieve protected access in Swift? Yes, we can!

Apple has already published a blog [Access Control and protected](https://developer.apple.com/swift/blog/?id=11) in 2014 regarding this demand and how unnecessary it is. But still I believe there are lot of situations in projects where we need to hide some properties and methods from outside classes but only accessible to children. So here's what I have come up with:

```swift
//Animal.swift file
class Animal {
    fileprivate var protectedVar: Int = 0
    fileprivate func protectedFunc() {//do stuff}
}

class Dog: Animal {
    func doSomething() {
        protectedVar = 1
        protectedFunc()
    }
}
```

If we try to access `protectedVar` or `protectedFunc()` from outside of *Animal.swift* file then compiler will throw an error.  
To achieve protected access like this only thing we need to keep in mind that **children must be declared in same file as parent declared in**.

Have you any time stuck searching for protected access in Swift? Then tell me how you got through it in comments below.  
Also if you have any other solutions, please post those here or [Twitter @d4ttatraya](https://twitter.com/D4ttatraya)

*References:  
[Apple's Developer Guide](https://developer.apple.com/library/content/documentation/Swift/Conceptual/Swift_Programming_Language/AccessControl.html)*

