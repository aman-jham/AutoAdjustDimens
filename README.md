<img src=https://raw.githubusercontent.com/aman-jham/AutoAdjustDimens/master/assets/autoadjustdimen.jpg >

Auto Adjust Scalable Dimension Library
========================================

[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)
[![API](https://img.shields.io/badge/API-1%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=1)
[ ![Download](https://api.bintray.com/packages/amanjham/com.auto.adjust/dimens/images/download.svg?version=1.0.8) ](https://bintray.com/amanjham/com.auto.adjust/dimens/1.0.8/link)
<br>

[![Twitter](https://img.shields.io/badge/Twitter-@AmanJham-blue.svg?style=flat)](https://twitter.com/amanjham)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/091df1fb4fbd47b9be970fd7bd1e0e6c)](https://www.codacy.com/manual/aman-jham/AutoAdjustDimens?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=aman-jham/AutoAdjustDimens&amp;utm_campaign=Badge_Grade)

This is an Android library allowing to auto adjust the density pixels.

USAGE
-----

To use this library in your project Using Android Studio and Gradle:

```groovy
implementation 'com.auto.adjust:dimens:1.0.9'
```

XML
-----

```xml

android:layout_width="@dimen/_100adp"
         
android:layout_height="@dimen/_100adp"
         
android:padding="@dimen/_8adp"
         
android:margin="@dimen/_8adp"

android:textSize="@dimen/_11asp"

```

You must use the following properties in your XML.

| Properties                       | Description                                                  |
| -------------------------------- | ------------------------------------------------------------ |
| `@dimen/_100adp`                 | For positive dimens                                          |
| `@dimen/_100_minus_adp`          | For negative dimens                                          |
| `@dimen/_11asp`                  | For text sizes                                               |



KOTLIN
-----

```kotlin

resources.getDimensionPixelSize(R.dimen._100adp)
resources.getDimensionPixelSize(R.dimen._11asp)

```

JAVA
-----

```java

getResources().getDimensionPixelOffset(R.dimen._100adp);
getResources().getDimensionPixelOffset(R.dimen._11asp);

```

COMPARISION
-----

    +---------+-------------+---------------+-------------+--------------------+
    | Unit    | Description | Units Per     | Density     | Same Physical Size |
    |         |             | Physical Inch | Independent | On Every Screen    |
    +---------+-------------+---------------+-------------+--------------------+
    | px      | Pixels      | Varies        | No          | No                 |
    +---------+-------------+---------------+-------------+--------------------+
    | in      | Inches      | 1             | Yes         | Yes                |
    +---------+-------------+---------------+-------------+--------------------+
    | mm      | Millimeters | 25.4          | Yes         | Yes                |
    +---------+-------------+---------------+-------------+--------------------+
    | pt      | Points      | 72            | Yes         | Yes                |
    +---------+-------------+---------------+-------------+--------------------+
    | dp      | Density     | ~160          | Yes         | No                 |
    |         | Independent |               |             |                    |
    |         | Pixels      |               |             |                    |
    +---------+-------------+---------------+-------------+--------------------+
    | sp      | Scale       | ~160          | Yes         | No                 |
    |         | Independent |               |             |                    |
    |         | Pixels      |               |             |                    |
    +---------+-------------+---------------+-------------+--------------------+
    | adp     | Auto        | ~160          | Yes         | Yes                |
    |         | Density     |               |             |                    |
    |         | Independent |               |             |                    |
    |         | Pixels      |               |             |                    |
    +---------+-------------+---------------+-------------+--------------------+
    | asp     | Auto        | ~160          | Yes         | Yes                |
    |         | Scale       |               |             |                    |
    |         | Independent |               |             |                    |
    |         | Pixels      |               |             |                    |
    +---------+-------------+---------------+-------------+--------------------+


More info can be also be found in the [Google Design Documentation](https://www.google.com/design/spec/layout/units-measurements.html#).

LIMITATION
-----
Use it carefully! for example, in most cases you still need to design a different layout for tablets.

SUPPORT ❤️
-----

Find this library useful? Support it by joining [**stargazers**](https://github.com/aman-jham/AutoAdjustDimens/stargazers) for this repository ⭐️
<br/>
And [**follow me**](https://github.com/aman-jham?tab=followers) for my next creations 👍

LICENCE
-----

Auto-Adjust-Dimension by [Aman Jham](https://www.linkedin.com/in/aman-jham-9436276a/) is licensed under a [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).