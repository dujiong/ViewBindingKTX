# ViewBindingKTX

[English](https://github.com/DylanCaiCoding/ViewBindingKtx) | 中文

[![](https://www.jitpack.io/v/DylanCaiCoding/ViewBindingKTX.svg)](https://www.jitpack.io/#DylanCaiCoding/ViewBindingKTX) [![](https://img.shields.io/badge/License-Apache--2.0-blue.svg)](https://github.com/DylanCaiCoding/ViewBindingKtx/blob/master/LICENSE)

[ViewBinding](https://developer.android.com/topic/libraries/view-binding) 相对于 Kotlin synthetics、ButterKnife、findViewById，能减少 id 写错或类型写错导致的异常，官方和 JakeWharton 都推荐使用。但是 ViewBinding 直接使用会有点繁琐，所以本库能**帮助你在各种使用场景用尽可能少的代码来使用 ViewBinding**。

## Feature

- 支持 Kotlin 和 Java 用法
- 支持多种使用反射和不使用反射的用法
- 支持封装改造自己的基类，使其用上 ViewBinding
- 支持 BaseRecyclerViewAdapterHelper
- 支持 Activity、Fragment、Dialog、Adapter
- 支持在 Fragment 自动释放绑定类的实例对象
- 支持实现自定义组合控件
- 支持 TabLayout 实现自定义标签布局
- 支持 DataBinding 自动设置 lifecycleOwner

## Gradle

在根目录的 build.gradle 添加：

```groovy
allprojects {
    repositories {
        ...
        maven { url 'https://www.jitpack.io' }
    }
}
```

添加配置和依赖：

```groovy
android {
    buildFeatures {
        viewBinding = true
    }
}

dependencies {
    // 以下都是可选，请根据需要进行添加
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-ktx:1.2.1'
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-nonreflection-ktx:1.2.1'
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-base:1.2.1'
    implementation 'com.github.DylanCaiCoding.ViewBindingKTX:viewbinding-brvah:1.2.1'
}
```

## Wiki

#### Kotlin 用法

- [使用拓展函数](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/使用拓展函数)

- [改造基类](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/改造基类-(Kotlin))

- [兼容 BRVAH](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/兼容-BRVAH-(Kotlin))

#### Java 用法

- [改造基类](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/改造基类-(Java))

- [兼容 BRVAH](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/兼容-BRVAH-(Java))

#### 其它

- [Q&A](https://github.com/DylanCaiCoding/ViewBindingKtx/wiki/Q&A)

## 更新日志

[Releases](https://github.com/DylanCaiCoding/ViewBindingKTX/releases)

## 相关文章

讲解本库的封装思路

- [《优雅地封装和使用 ViewBinding，该替代 Kotlin synthetic 和 ButterKnife 了》](https://juejin.cn/post/6906153878312452103)

- [《ViewBinding 巧妙的封装思路，还能这样适配 BRVAH》](https://juejin.cn/post/6950530267547172901)

## Thanks

感谢 [ViewBindingPropertyDelegate](https://github.com/kirich1409/ViewBindingPropertyDelegate) 不使用反射的思路

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
