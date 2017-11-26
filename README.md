# PostgreSQL libpq system module

Add *Clibpq* as a [dependency](https://github.com/apple/swift-package-manager/blob/master/Documentation/PackageDescriptionV4.md#dependencies) in your Package.swift file:

```swift
// swift-tools-version:4.0
// The swift-tools-version declares the minimum version of Swift required to build this package.

import PackageDescription

let package = Package(
    name: "foo-bar",
    products: [
        .executable(name: "foo-bar", targets: ["foo-bar"]),
    ],
    dependencies: [
        .package(url: "https://github.com/ManuW/Clibpq", from: "0.0.3")
    ],
    targets: [
        // Targets are the basic building blocks of a package. A target can define a module or a test suite.
        // Targets can depend on other targets in this package, and on products in packages which this package depends on.
        .target(
            name: "foo-bar",
            dependencies: []
        ),
    ]
)
```
