# ViewBindingKTX

English | [中文](https://github.com/DylanCaiCoding/ViewBindingKtx/blob/master/README_CN.md)

[![](https://www.jitpack.io/v/DylanCaiCoding/ViewBindingKTX.svg)](https://www.jitpack.io/#DylanCaiCoding/ViewBindingKTX) [![](https://img.shields.io/badge/License-Apache--2.0-blue.svg)](https://github.com/DylanCaiCoding/ViewBindingKtx/blob/master/LICENSE)

[ViewBinding](https://developer.android.com/topic/libraries/view-binding) reduces exceptions caused by id or type errors, which are recommended by both Google officials and Jake Wharton, but it can be a bit cumbersome to use, so this library can **help you use ViewBinding with as little code as possible in any usage scenario**.

## Feature

- Support for the usage of Kotlin and Java
- Support for the usage of reflection and non-reflection
- Support to modify your base class to support ViewBinding
- Support for BaseRecyclerViewAdapterHelper
- Support for Activity, Fragment, Dialog, Adapter
- Support automatic release of binding class instance in Fragment
- Support for custom combination view
- Support for TabLayout to set custom view
- Support for DataBinding to automatically set the lifecycle owner

## Gradle

Add it in your root build.gradle at the end of repositories:
```groovy
allprojects {
    repositories {
        ...
        maven { url 'https://www.jitpack.io' }
    }
}
```

Add dependencies and configurations：

```groovy
android {
    buildFeatures {
        viewBinding = true
    }
}

dependencies {
    // The following are optional, please add as needed
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-ktx:1.2.1'
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-nonreflection-ktx:1.2.1'
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-base:1.2.1'
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-brvah:1.2.1'
}
```

## Wiki

#### Kotlin usage

- [Using the extension function](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/使用拓展函数)

- [Modify base class](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/改造基类-(Kotlin))

- [Compatible with BRVAH](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/兼容-BRVAH-(Kotlin))

#### Java usage

- [Modify base class](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/改造基类-(Java))

- [Compatible with BRVAH](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/兼容-BRVAH-(Java))

#### Others

- [Q&A](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/Q&A)

## Change log

[Releases](https://github.com/DylanCaiCoding/ViewBindingKTX/releases)

## Thanks

Thanks [ViewBindingPropertyDelegate](https://github.com/kirich1409/ViewBindingPropertyDelegate) for providing an idea without reflection

## License

```
Copyright (C) 2020. Dylan Cai

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
