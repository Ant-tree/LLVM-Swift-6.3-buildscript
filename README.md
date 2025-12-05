# LLVM-Swift-6.3-buildscript

> **Use XCode 16.4**
> ```
> # Download Xcode 16.4 from https://developer.apple.com/download/all
> xcode-select /Applications/Xcode_16.4.app
> # Check swiftc version
> swiftc --version
> $ swift-driver version: 1.120.5 Apple Swift version 6.1.2 (swiftlang-6.1.2.1.2 clang-1700.0.13.5)
> $ Target: arm64-apple-macosx15.0
> ```
> Can only build arm64 target including toolchain

This repo contains the patch files only.

So just copy and paste them into the swift repo directory.

Referenced repo regards the commit id `35f48306184cd25f1067cfc503e92c8f57b29e89`, so use the command below to download the exact same version tested.

```
git clone https://github.com/apple/swift.git swift-6.3dev
cd swift-6.3dev
git checkout 35f48306184cd25f1067cfc503e92c8f57b29e89
```

After download the swift source, download the submodules using : ```./utils/update-checkout --clone```

For the obfuscation applied llvm source, refer this repository : https://github.com/Ant-tree/LLVM-Swift-6.3
