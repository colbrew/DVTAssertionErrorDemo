Demo project of DVTAssertions: 'missing IDE Target' Warning - FB13695124

To reproduce:
1. Use Xcode 15.1 version 15C65 or Xcode 15.2 version 15C500b

2. Run `xcodebuild -workspace DVTAssertionErrorDemo.xcworkspace -scheme DVTAssertionErrorDemo -destination 'platform=iOS Simulator,name=iPhone 15,OS=17.2' build-for-testing -quiet` from terminal


This will produce:
```
2024-04-01 11:12:09.311 xcodebuild[9258:111966] [MT] DVTAssertions: Warning in DevToolsCore/Xcode3Core/LegacyProjects/Frameworks/DevToolsCore/DevToolsCore/ProjectModel/Xcode3Model/Xcode3TargetBuildable.m:411
Details:  missing IDE target for <Xcode3TargetProduct:0x600000da16e0:DVTAssertionErrorDemo.app blueprint:<Xcode3Target:0x7f87d2117940:DVTAssertionErrorDemo>>'s dependency: (null)
Object:   <Xcode3TargetProduct: 0x600000da16e0>
Method:   -directDependenciesForBuildParameters:
Thread:   <_NSMainThread: 0x600003cf0380>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2024-04-01 11:12:09.312 xcodebuild[9258:111966] [MT] DVTAssertions: Warning in DevToolsCore/Xcode3Core/LegacyProjects/Frameworks/DevToolsCore/DevToolsCore/ProjectModel/Xcode3Model/Xcode3TargetBuildable.m:411
Details:  missing IDE target for <Xcode3TargetProduct:0x600000da16e0:DVTAssertionErrorDemo.app blueprint:<Xcode3Target:0x7f87d2117940:DVTAssertionErrorDemo>>'s dependency: (null)
Object:   <Xcode3TargetProduct: 0x600000da16e0>
Method:   -directDependenciesForBuildParameters:
Thread:   <_NSMainThread: 0x600003cf0380>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2024-04-01 11:12:09.318 xcodebuild[9258:111966] [MT] DVTAssertions: Warning in DevToolsCore/Xcode3Core/LegacyProjects/Frameworks/DevToolsCore/DevToolsCore/ProjectModel/Xcode3Model/Xcode3TargetBuildable.m:411
Details:  missing IDE target for <Xcode3TargetProduct:0x600000da16e0:DVTAssertionErrorDemo.app blueprint:<Xcode3Target:0x7f87d2117940:DVTAssertionErrorDemo>>'s dependency: (null)
Object:   <Xcode3TargetProduct: 0x600000da16e0>
Method:   -directDependenciesForBuildParameters:
Thread:   <_NSMainThread: 0x600003cf0380>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
2024-04-01 11:12:09.319 xcodebuild[9258:111966] [MT] DVTAssertions: Warning in DevToolsCore/Xcode3Core/LegacyProjects/Frameworks/DevToolsCore/DevToolsCore/ProjectModel/Xcode3Model/Xcode3TargetBuildable.m:411
Details:  missing IDE target for <Xcode3TargetProduct:0x600000da16e0:DVTAssertionErrorDemo.app blueprint:<Xcode3Target:0x7f87d2117940:DVTAssertionErrorDemo>>'s dependency: (null)
Object:   <Xcode3TargetProduct: 0x600000da16e0>
Method:   -directDependenciesForBuildParameters:
Thread:   <_NSMainThread: 0x600003cf0380>{number = 1, name = main}
Please file a bug at https://feedbackassistant.apple.com with this warning message and any useful information you can provide.
```
